## Impact
Malicious user is able to DoS the function `depositAsset`, by increasing the balance of `LRTDepositPool` for an underlying asset.

## Proof of Concept
There is a condition inside `depositAsset` which checks if the balance of the protocol for an underlying token is reached to the depositLimit (limit will be set by MANAGER role), then `depositAssets` doesn't let anyone to deposit that underlying asset:
```solidity
if (depositAmount > getAssetCurrentLimit(asset)) {
     revert MaximumDepositLimitReached();
}
```
So imagine this scenario (See also getAssetCurrentLimit(), getTotalAssetDeposits(), getAssetDistributionData() and you see how `getAssetCurrentLimit` depends on balance of `LRTDepositPool`):
- MANAGER inserts a new supported assets `X` and sets `depositLimit` of asset `X` to 10 (not real number, just an example).
- Attacker transfers `10 X` directly to `LRTDepositPool` (without calling `depositAsset`).
- now `X`.balanceOf(`LRTDepositPool`) returns 10 and also `getTotalAssetDeposits()` returns 10.
- `getAssetCurrentLimit` returns 0, because:
```solidity
lrtConfig.depositLimitByAsset(asset) - getTotalAssetDeposits(asset); // <--- (10 - 10) = 0
```
- Bob calls `depositAssets` and wants to mint some amount of `rsETH`.
- Bob gets a revert `MaximumDepositLimitReached` because the balance of protocol for asset `X` is reached to `depositLimit` and no one is able to mint any rsETH until the MANAGER calls `updateAssetDepositLimit`.


## Tools Used
Manual Review

## Recommended Mitigation Steps
Consider adding a mapping:
```solidity
mapping(address asset => uint256 amount)
```
which stores how much asset is deposited through `depositAsset`.











