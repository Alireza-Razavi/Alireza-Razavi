## Impact
Attacker is able transfer some amount of an underlying asset directly to `LRTDepositPool` (or a NodeDelegator, the goal of attacker is to increase the balance of protocol for an underlying asset) and inflate the rsETH price.

## Proof of Concept
Note: getTotalAssetDeposits returns the total asset (from token `X` for example) present in protocol:
(`contract balance of LRTDepositPool for asset X` + `amount of asset X that are transferred to NodeDelegators` + `amount of asset X that are deposited into strategies`)

This is how the price of rsETH is calculated (see LRTOracle#getRSETHPrice):
```solidity
    for (uint16 asset_idx; asset_idx < supportedAssetCount;) { // <-- Assume supportedAssetCount is 1 and there is only 1 asset `X`
            address asset = supportedAssets[asset_idx]; // <-- address of asset `X`
            uint256 assetER = getAssetPrice(asset); // <-- price of asset `X`

            uint256 totalAssetAmt = ILRTDepositPool(lrtDepositPoolAddr).getTotalAssetDeposits(asset); // <-- amount of asset `X` owned by Protocol (Attacker can directly transfer some amount of asset `X` to LRTDepositPool, this increases balance of LRTDepositPool contract, so when LRTDepositPool's balance increases, as a result, Protocol's balance also increases and rsETH price will be manipulated)

            totalETHInPool += totalAssetAmt * assetER; // <-- (number of asset `X` owned by Protocol) * (price of asset `X`)

            unchecked {
                ++asset_idx;
            }
    }

    return totalETHInPool / rsEthSupply; // <-- (value of asset `X` (value in $dollar) owned by the Protocol) / (number of rsETH minted) = rsETH_price
```
(Everything is commented in code)
So what will happen if attacker transfers some amount of asset `X` (for example 1000) directly to LRTDepositPool (without minting any rsETH) ? 
The answer is: totalSupply of rsETH will remain the same, but the `totalETHInPool` will be a higher amount (because `totalETHInPool` depends on `getTotalAssetDeposits` and getTotalAssetDeposits depends on the contract balance of `LRTDepositPool` for asset `X`) -> which means the rsETH price will be higher than before and inflated.
Let's imagine an example:
- Assume there is one supported asset `X` and price of `X` is $2.
- Assume LRTDepositPool owns 1000 tokens of `X` (`getTotalAssetDeposits` returns 1000) and minted 2 rsETH (totalSupply of rsETH is 2).

Now:
`totalETHInPool = 2000$ (because 1000 * 2$)`
`rsEthSupply = 2`
`rsETH_price = totalETHInPool / rsEthSupply = $2000 / 2 = $1000`

- Attacker transfers 1000 `X` directly to LRTDepositPool and increases the balance of LRTDepositPool for asset `X`.

Now:
`totalETHInPool = 4000$ (because 2000 * 2$)`
`rsEthSupply = 2`
`rsETH_price = totalETHInPool / rsEthSupply = $4000 / 2 = $2000`

## Tools Used
Manual Review

## Recommended Mitigation Steps
getTotalAssetDeposits() should not be dependent of contract balance for an underlying asset, consider adding a state variable which tracks how much balance is deposited through protocol.



































