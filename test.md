# Report


## Medium Issues


Total <b>87</b> instances over <b>2</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | Unsafe use of ERC20 `transfer()`/`transferFrom()`/`approve()` | 4 |
| [M-2](#M-2) | Centralization Risk for trusted owners | 83 |

## Low Issues


Total <b>187</b> instances over <b>14</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | `approve()`/`safeApprove()` may revert if the current approval is not zero | 23 |
| [L-2](#L-2) | Check division by zero is prevented | 52 |
| [L-3](#L-3) | Enum values should be used instead of constant array indexes | 6 |
| [L-4](#L-4) | Governance functions should be controlled by time locks | 2 |
| [L-5](#L-5) | Loss of precision in divisions | 52 |
| [L-6](#L-6) | `SafeTransferLib` does not ensure that the token contract exists | 1 |
| [L-7](#L-7) | Some tokens may revert when large transfers are made | 1 |
| [L-8](#L-8) | Some tokens may revert when zero value transfers are made | 1 |
| [L-9](#L-9) | Timestamp may be manipulation | 19 |
| [L-10](#L-10) |  `abi.encodePacked()` should not be used with dynamic types when passing the result to a hash function such as `keccak256()` | 3 |
| [L-11](#L-11) | `decimals()` is not a part of the ERC-20 standard | 1 |
| [L-12](#L-12) | Do not use deprecated library functions | 21 |
| [L-13](#L-13) | Empty Function Body - Consider commenting why | 1 |
| [L-14](#L-14) | `safeApprove()` is deprecated | 4 |

## Non Critical Issues


Total <b>183</b> instances over <b>18</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, for readability | 1 |
| [NC-2](#NC-2) | Consider adding formal verification proofs | 1 |
| [NC-3](#NC-3) | Constants should be put on the left side of comparisons | 56 |
| [NC-4](#NC-4) | Contracts should have full test coverage | 1 |
| [NC-5](#NC-5) | Events that mark critical parameter changes should contain both the old and the new value | 37 |
| [NC-6](#NC-6) | Custom errors should be used rather than `revert()`/`require()` | 8 |
| [NC-7](#NC-7) | Enable IR-based code generation | 1 |
| [NC-8](#NC-8) | Import declarations should import specific identifiers, rather than the whole file | 6 |
| [NC-9](#NC-9) | Large or complicated code bases should implement invariant tests | 1 |
| [NC-10](#NC-10) | Consider moving `msg.sender` checks to `modifier`s | 1 |
| [NC-11](#NC-11) | Named mappings are recommended | 13 |
| [NC-12](#NC-12) | There is no need to initialize variables with 0 | 10 |
| [NC-13](#NC-13) | Put all system-wide constants in one file | 14 |
| [NC-14](#NC-14) | Consider using `delete` rather than assigning zero to clear values | 1 |
| [NC-15](#NC-15) | Expressions for constant values should use `immutable` rather than `constant` | 14 |
| [NC-16](#NC-16) | Use of `override` is unnecessary | 2 |
| [NC-17](#NC-17) | Whitespace in Expressions | 3 |
| [NC-18](#NC-18) | Return values of `approve()` not checked | 13 |

## Gas Optimizations


Total <b>356</b> instances over <b>24</b> issues:

|ID|Issue|Instances|Gas|
|-|:-|:-:|:-:|
| [GAS-1](#GAS-1) | Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, where appropriate | 1 | - |
| [GAS-2](#GAS-2) | Consider activating via-ir for deploying | 1 | - |
| [GAS-3](#GAS-3) | Divisions can be `unchecked` to save gas | 52 | 1040 |
| [GAS-4](#GAS-4) | Don't transfer with zero amount to save gas | 1 | - |
| [GAS-5](#GAS-5) | Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables | 41 | 4633 |
| [GAS-6](#GAS-6) | `keccak256()` hash of literals should only be computed once | 9 | 378 |
| [GAS-7](#GAS-7) | Operator `>=`/`<=` costs less gas than operator `>`/`<` | 38 | 114 |
| [GAS-8](#GAS-8) | Use assembly to compute hashes to save gas | 12 | 960 |
| [GAS-9](#GAS-9) | Use assembly to emit events | 45 | 1710 |
| [GAS-10](#GAS-10) | Using a double `if` statement instead of a logical AND (`&&`) | 14 | 420 |
| [GAS-11](#GAS-11) | Use `storage` instead of `memory` for structs/arrays | 4 | 16800 |
| [GAS-12](#GAS-12) | Using bitmap to store bool states can save gas | 2 | - |
| [GAS-13](#GAS-13) | Using bools for storage incurs overhead | 4 | - |
| [GAS-14](#GAS-14) | Cache array length outside of loop | 11 | - |
| [GAS-15](#GAS-15) | Use Custom Errors | 8 | 400 |
| [GAS-16](#GAS-16) | Don't use `SafeMath` once the solidity version is 0.8.0 or greater | 3 | - |
| [GAS-17](#GAS-17) | Don't initialize variables with default value | 10 | - |
| [GAS-18](#GAS-18) | Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead | 14 | 770 |
| [GAS-19](#GAS-19) | Constructors can be marked as `payable` to save deployment gas | 6 | 126 |
| [GAS-20](#GAS-20) | Functions guaranteed to revert when called by normal users can be marked `payable` | 22 | 462 |
| [GAS-21](#GAS-21) | `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too) | 12 | 60 |
| [GAS-22](#GAS-22) | Using `private` rather than `public` for constants, saves gas | 14 | - |
| [GAS-23](#GAS-23) | Use shift Right/Left instead of division/multiplication if possible | 13 | - |
| [GAS-24](#GAS-24) | Use `!= 0` instead of `> 0` for unsigned integer comparison | 19 | 76 |

## Medium Issues

<a name="M-1"></a> 
### [M-1] Unsafe use of ERC20 `transfer()`/`transferFrom()`/`approve()`
Some tokens do not implement the ERC20 standard properly. For example Tether (USDT)'s `transfer()` and `transferFrom()` functions do not return booleans as the ERC20 specification requires, and instead have no return value. When these sorts of tokens are cast to IERC20/ERC20, their function signatures do not match and therefore the calls made will revert.It is recommended to use the [`SafeERC20`](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/f347b410cf6aeeaaf5197e1fece139c793c03b2b/contracts/token/ERC20/utils/SafeERC20.sol#L19)'s `safeTransfer()` and `safeTransferFrom()` from OpenZeppelin instead.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

106:     collateral.approve(_perpetualAtlanticVault, type(uint256).max);

107:     ERC20(rdpx).approve(_perpetualAtlanticVault, type(uint256).max);

128:     collateral.transferFrom(msg.sender, address(this), assets);

170:     collateral.transfer(receiver, assets);

```

</details>

---

<a name="M-2"></a> 
### [M-2] Centralization Risk for trusted owners
Contracts have owners with privileged rights to perform admin tasks and need to be trusted to not perform malicious updates or drain funds.

<details>
<summary>
There are <b>83</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

5: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

22: contract UniV2LiquidityAMO is AccessControl {

82:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

111:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

130:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

144:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

195:     external

263:     external

308:   ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 token2Amount) {

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

5: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

28: contract UniV3LiquidityAMO is AccessControl, ERC721Holder {

119:   function collectFees() external onlyRole(DEFAULT_ADMIN_ROLE) {

144:   ) public onlyRole(DEFAULT_ADMIN_ROLE) {

157:   ) public onlyRole(DEFAULT_ADMIN_ROLE) {

217:   ) public onlyRole(DEFAULT_ADMIN_ROLE) {

281:   ) public onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256) {

316:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

327:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

343:   ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (bool, bytes memory) {

```

```solidity
File: contracts/core/RdpxV2Bond.sol

7: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

15:   AccessControl,

29:   function pause() public onlyRole(DEFAULT_ADMIN_ROLE) {

33:   function unpause() public onlyRole(DEFAULT_ADMIN_ROLE) {

39:   ) public onlyRole(MINTER_ROLE) returns (uint256 tokenId) {

```

```solidity
File: contracts/core/RdpxV2Core.sol

5: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

35:   AccessControl,

144:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

152:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

163:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

182:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

195:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

206:   function setIsreLP(bool _isReLPActive) external onlyRole(DEFAULT_ADMIN_ROLE) {

218:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

230:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

243:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

272:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

315:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

361:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

378:   function addAMOAddress(address _addr) external onlyRole(DEFAULT_ADMIN_ROLE) {

390:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

407:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

421:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

432:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

443:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

457:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

767:     external

791:     external

1054:   ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 wethReceived) {

1085:   ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 dpxEthReceived) {

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

12: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

70:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

76:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

95:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

118:   ) external onlyRole(MINTER_ROLE) {

142:   ) public onlyRole(RDPXV2CORE_ROLE) {

151:   function getBondsOwned(

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

7: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

16:   AccessControl,

29:   function pause() public onlyRole(PAUSER_ROLE) {

33:   function unpause() public onlyRole(PAUSER_ROLE) {

37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {

43:   ) public override(ERC20Burnable, IDpxEthToken) onlyRole(BURNER_ROLE) {

50:   ) public override onlyRole(BURNER_ROLE) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

13: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

35:   AccessControl,

136:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

144:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

155:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

166:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

189:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

221:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

239:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

243:   function setLpAllowance(bool increase) external onlyRole(DEFAULT_ADMIN_ROLE) {

261:     onlyRole(RDPXV2CORE_ROLE)

320:     onlyRole(RDPXV2CORE_ROLE)

372:   function payFunding() external onlyRole(RDPXV2CORE_ROLE) returns (uint256) {

```

```solidity
File: contracts/reLP/ReLPContract.sol

5: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

25: contract ReLPContract is AccessControl {

92:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

125:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

173:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

188:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

202:   function reLP(uint256 _amount) external onlyRole(RDPXV2CORE_ROLE) {

```

</details>

---


## Low Issues

<a name="L-1"></a> 
### [L-1] `approve()`/`safeApprove()` may revert if the current approval is not zero
Calling `approve()` without first calling `approve(0)` if the current approval is non-zero will revert with some tokens, such as Tether (USDT). While Tether is known to do this, it applies to other tokens as well, which are trying to protect against [this attack vector](https://docs.google.com/document/d/1YLPtQxZu1UAvO9cZ1O2RPXBbT0mooh4DYKjA_jp-RLM/edit). `safeApprove()` itself also implements this protection. Always reset the approval to zero before changing it to a new value (`SafeERC20.forceApprove()` does this for you), or use `safeIncreaseAllowance()`/`safeDecreaseAllowance()`

<details>
<summary>
There are <b>23</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

134:     IERC20WithBurn(_token).approve(_spender, _amount);

200:     IERC20WithBurn(addresses.tokenA).safeApprove(

204:     IERC20WithBurn(addresses.tokenB).safeApprove(

268:     IERC20WithBurn(addresses.pair).safeApprove(addresses.ammRouter, lpAmount);

328:     IERC20WithBurn(token1).safeApprove(addresses.ammRouter, token1Amount);

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

148:       TransferHelper.safeApprove(_token, _target, _amount);

150:       IERC20WithBurn(_token).approve(_target, _amount);

169:     IERC20WithBurn(params._tokenA).approve(

173:     IERC20WithBurn(params._tokenB).approve(

302:     TransferHelper.safeApprove(_tokenA, address(univ3_router), _amountAtoB);

```

```solidity
File: contracts/core/RdpxV2Core.sol

339:     IERC20WithBurn(weth).approve(

343:     IERC20WithBurn(weth).approve(addresses.dopexAMMRouter, type(uint256).max);

344:     IERC20WithBurn(weth).approve(addresses.dpxEthCurvePool, type(uint256).max);

345:     IERC20WithBurn(weth).approve(

411:     IERC20WithBurn(_token).approve(_spender, _amount);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

207:     collateralToken.safeApprove(

245:       ? collateralToken.approve(

249:       : collateralToken.approve(addresses.perpetualAtlanticVaultLP, 0);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

106:     collateral.approve(_perpetualAtlanticVault, type(uint256).max);

107:     ERC20(rdpx).approve(_perpetualAtlanticVault, type(uint256).max);

```

```solidity
File: contracts/reLP/ReLPContract.sol

150:     IERC20WithBurn(addresses.pair).safeApprove(

155:     IERC20WithBurn(addresses.tokenA).safeApprove(

160:     IERC20WithBurn(addresses.tokenB).safeApprove(

```

</details>

---

<a name="L-2"></a> 
### [L-2] Check division by zero is prevented

<details>
<summary>
There are <b>52</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

373:     return (lpTokenBalance * getLpPrice()) / 1e8;

```

```solidity
File: contracts/core/RdpxV2Core.sol

535:           ethBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

539:           dpxEthBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

546:       ? (((_amount * getDpxEthPrice()) / 1e8) -

547:         (((_amount * getDpxEthPrice()) * slippageTolerance) / 1e16))

548:       : (((_amount * getEthPrice()) / 1e8) -

549:         (((_amount * getEthPrice()) * slippageTolerance) / 1e16));

570:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= _amount / 2;

574:       _amount / 2

579:       .deposit(_amount / 2);

605:     uint256 rdpxRequiredInWeth = (_rdpxRequired * getRdpxPrice()) / 1e8;

608:     amount1 = ((rdpxRequiredInWeth * _amount) /

612:     amount1 = (amount1 * (100e8 - _delegateFee)) / 1e10;

658:         (_rdpxAmount * rdpxBurnPercentage) / 1e10

665:           (_rdpxAmount * rdpxFeePercentage) / 1e10

669:       uint256 rdpxAmountInWeth = (_rdpxAmount * getRdpxPrice()) / 1e8;

673:       uint256 extraRdpxToWithdraw = (discountReceivedInWeth * 1e8) /

1165:         1e2) / (Math.sqrt(1e18)); // 1e8 precision

1170:         ((RDPX_RATIO_PERCENTAGE - (bondDiscount / 2)) *

1172:           DEFAULT_PRECISION) /

1176:         ((ETH_RATIO_PERCENTAGE - (bondDiscount / 2)) * _amount) /

1176:         ((ETH_RATIO_PERCENTAGE - (bondDiscount / 2)) * _amount) /

1181:         (RDPX_RATIO_PERCENTAGE * _amount * DEFAULT_PRECISION) /

1185:         (ETH_RATIO_PERCENTAGE * _amount) /

1190:       .roundUp(rdpxPrice - (rdpxPrice / 4)); // 25% below the current price

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

270:     uint256 strike = roundUp(currentPrice - (currentPrice / 4)); // 25% below the current price

276:     uint256 requiredCollateral = (amount * strike) / 1e8;

335:       ethAmount += (amount * strike) / 1e8;

475:           (currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

481:             (currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

487:           ((currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

512:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

516:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

521:       ((currentFundingRate * (block.timestamp - startTime)) / 1e18),

550:     ) * _amount) / 1e8);

559:     return strike > price ? ((strike - price) * amount) / 1e8 : 0;

604:         (amount * 1e18) /

612:         ((amount * 1e18) / (endTime - startTime));

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

281:       ((_rdpxCollateral * rdpxPriceInAlphaToken) / 1e8);

```

```solidity
File: contracts/reLP/ReLPContract.sol

230:       1e2) / (Math.sqrt(1e18)); // 1e6 precision

232:     uint256 tokenAToRemove = ((((_amount * 4) * 1e18) /

235:       baseReLpRatio) / (1e18 * DEFAULT_PRECISION * 1e2);

239:     uint256 lpToRemove = (tokenAToRemove * totalLpSupply) /

251:       ((tokenAToRemove * liquiditySlippageTolerance) / 1e8);

252:     uint256 mintokenBAmount = ((tokenAToRemove * tokenAInfo.tokenAPrice) /

254:       ((tokenAToRemove * tokenAInfo.tokenAPrice) * liquiditySlippageTolerance) /

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

279:         amountB / 2,

290:       amountB / 2,

```

</details>

---

<a name="L-3"></a> 
### [L-3] Enum values should be used instead of constant array indexes
Create a commented enum value to use instead of constant array indexes, this makes the code far easier to understand.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

332:     path[0] = token1;

333:     path[1] = token2;

```

```solidity
File: contracts/core/RdpxV2Core.sol

1094:       path[0] = reserveAsset[reservesIndex["RDPX"]].tokenAddress;

1095:       path[1] = weth;

```

```solidity
File: contracts/reLP/ReLPContract.sol

269:     path[0] = addresses.tokenB;

270:     path[1] = addresses.tokenA;

```

</details>

---

<a name="L-4"></a> 
### [L-4] Governance functions should be controlled by time locks
Governance functions (such as upgrading contracts, setting critical parameters) should be controlled using time locks to introduce a delay between a proposal and its execution. This gives users time to exit before a potentially dangerous or malicious operation is applied.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/core/RdpxV2Core.sol

206:   function setIsreLP(bool _isReLPActive) external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

243:   function setLpAllowance(bool increase) external onlyRole(DEFAULT_ADMIN_ROLE) {

```

</details>

---

<a name="L-5"></a> 
### [L-5] Loss of precision in divisions
Division by large numbers may result in the result being zero, due to solidity not supporting fractions. Consider requiring a minimum amount for the numerator to ensure that it is always larger than the denominator.

<details>
<summary>
There are <b>52</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

373:     return (lpTokenBalance * getLpPrice()) / 1e8;

```

```solidity
File: contracts/core/RdpxV2Core.sol

535:           ethBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

539:           dpxEthBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

546:       ? (((_amount * getDpxEthPrice()) / 1e8) -

547:         (((_amount * getDpxEthPrice()) * slippageTolerance) / 1e16))

548:       : (((_amount * getEthPrice()) / 1e8) -

549:         (((_amount * getEthPrice()) * slippageTolerance) / 1e16));

570:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= _amount / 2;

574:       _amount / 2

579:       .deposit(_amount / 2);

605:     uint256 rdpxRequiredInWeth = (_rdpxRequired * getRdpxPrice()) / 1e8;

608:     amount1 = ((rdpxRequiredInWeth * _amount) /

612:     amount1 = (amount1 * (100e8 - _delegateFee)) / 1e10;

658:         (_rdpxAmount * rdpxBurnPercentage) / 1e10

665:           (_rdpxAmount * rdpxFeePercentage) / 1e10

669:       uint256 rdpxAmountInWeth = (_rdpxAmount * getRdpxPrice()) / 1e8;

673:       uint256 extraRdpxToWithdraw = (discountReceivedInWeth * 1e8) /

1165:         1e2) / (Math.sqrt(1e18)); // 1e8 precision

1170:         ((RDPX_RATIO_PERCENTAGE - (bondDiscount / 2)) *

1172:           DEFAULT_PRECISION) /

1176:         ((ETH_RATIO_PERCENTAGE - (bondDiscount / 2)) * _amount) /

1176:         ((ETH_RATIO_PERCENTAGE - (bondDiscount / 2)) * _amount) /

1181:         (RDPX_RATIO_PERCENTAGE * _amount * DEFAULT_PRECISION) /

1185:         (ETH_RATIO_PERCENTAGE * _amount) /

1190:       .roundUp(rdpxPrice - (rdpxPrice / 4)); // 25% below the current price

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

270:     uint256 strike = roundUp(currentPrice - (currentPrice / 4)); // 25% below the current price

276:     uint256 requiredCollateral = (amount * strike) / 1e8;

335:       ethAmount += (amount * strike) / 1e8;

475:           (currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

481:             (currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

487:           ((currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

512:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

516:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

521:       ((currentFundingRate * (block.timestamp - startTime)) / 1e18),

550:     ) * _amount) / 1e8);

559:     return strike > price ? ((strike - price) * amount) / 1e8 : 0;

604:         (amount * 1e18) /

612:         ((amount * 1e18) / (endTime - startTime));

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

281:       ((_rdpxCollateral * rdpxPriceInAlphaToken) / 1e8);

```

```solidity
File: contracts/reLP/ReLPContract.sol

230:       1e2) / (Math.sqrt(1e18)); // 1e6 precision

232:     uint256 tokenAToRemove = ((((_amount * 4) * 1e18) /

235:       baseReLpRatio) / (1e18 * DEFAULT_PRECISION * 1e2);

239:     uint256 lpToRemove = (tokenAToRemove * totalLpSupply) /

251:       ((tokenAToRemove * liquiditySlippageTolerance) / 1e8);

252:     uint256 mintokenBAmount = ((tokenAToRemove * tokenAInfo.tokenAPrice) /

254:       ((tokenAToRemove * tokenAInfo.tokenAPrice) * liquiditySlippageTolerance) /

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

279:         amountB / 2,

290:       amountB / 2,

```

</details>

---

<a name="L-6"></a> 
### [L-6] `SafeTransferLib` does not ensure that the token contract exists

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

172:     IERC20WithBurn(rdpx).safeTransfer(receiver, rdpxAmount);

```

</details>

---

<a name="L-7"></a> 
### [L-7] Some tokens may revert when large transfers are made
Tokens such as COMP or UNI will revert when an address' balance reaches `type(uint96).max`. Ensure that the calls below can be broken up into smaller batches if necessary.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

170:     collateral.transfer(receiver, assets);

```

</details>

---

<a name="L-8"></a> 
### [L-8] Some tokens may revert when zero value transfers are made
Despite the fact that [EIP-20 states](https://github.com/ethereum/EIPs/blob/7500ac4fc1bbdfaf684e7ef851f798f6b667b2fe/EIPS/eip-20.md?plain=1#L116) that zero-value transfers must be accepted, some tokens, such as LEND, will revert if this is attempted, which may cause transactions that involve other tokens (such as batch operations) to fully revert. Consider skipping the transfer if the amount is zero, which will also save gas.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

170:     collateral.transfer(receiver, assets);

```

</details>

---

<a name="L-9"></a> 
### [L-9] Timestamp may be manipulation
The `block.timestamp` can be manipulated by miners to perform MEV profiting or other time-based attacks.

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

231:         block.timestamp + 1

279:         block.timestamp + 1

342:         block.timestamp + 1

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

250:           block.timestamp

```

```solidity
File: contracts/core/RdpxV2Core.sol

502:       maturity: block.timestamp + bondMaturity,

503:       timestamp: block.timestamp

636:       _validate(expiry >= block.timestamp, 2);

1023:     _validate(block.timestamp > bonds[id].maturity, 7);

1103:           block.timestamp + 10

1194:     ).nextFundingPaymentTimestamp() - block.timestamp;

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

283:     uint256 timeToExpiry = nextFundingPaymentTimestamp() - block.timestamp;

463:     while (block.timestamp >= nextFundingPaymentTimestamp()) {

508:     lastUpdateTime = block.timestamp;

512:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

516:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

521:       ((currentFundingRate * (block.timestamp - startTime)) / 1e18),

```

```solidity
File: contracts/reLP/ReLPContract.sol

264:       block.timestamp + 10

283:         block.timestamp + 10

294:       block.timestamp + 10

```

</details>

---

<a name="L-10"></a> 
### [L-10]  `abi.encodePacked()` should not be used with dynamic types when passing the result to a hash function such as `keccak256()`
Use `abi.encode()` instead which will pad items to 32 bytes, which will [prevent hash collisions](https://docs.soliditylang.org/en/v0.8.13/abi-spec.html#non-standard-packed-mode) (e.g. `abi.encodePacked(0x123,0x456)` => `0x123456` => `abi.encodePacked(0x1,0x23456)`, but `abi.encode(0x123,0x456)` => `0x0...1230...456`). "Unless there is a compelling reason, `abi.encode` should be preferred". If there is only one argument to `abi.encodePacked()` it can often be cast to `bytes()` or `bytes32()` [instead](https://ethereum.stackexchange.com/questions/30912/how-to-compare-strings-in-solidity#answer-82739).
If all arguments are strings and or bytes, `bytes.concat()` should be used instead

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

106:       keccak256(abi.encodePacked(address(this), _tickLower, _tickUpper))

```

```solidity
File: contracts/core/RdpxV2Core.sol

1141:       keccak256(abi.encodePacked(asset.tokenSymbol)) ==

1142:         keccak256(abi.encodePacked(_token)),

```

</details>

---

<a name="L-11"></a> 
### [L-11] `decimals()` is not a part of the ERC-20 standard
The `decimals()` function is not a part of the ERC-20 standard, and was added later as an optional extension. As such, some valid ERC20 tokens do not support this interface, so it is unsafe to blindly cast all tokens to this interface, and then call this function.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

91:       ERC20(_collateral).decimals()

```

</details>

---

<a name="L-12"></a> 
### [L-12] Do not use deprecated library functions

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

58:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

200:     IERC20WithBurn(addresses.tokenA).safeApprove(

204:     IERC20WithBurn(addresses.tokenB).safeApprove(

268:     IERC20WithBurn(addresses.pair).safeApprove(addresses.ammRouter, lpAmount);

328:     IERC20WithBurn(token1).safeApprove(addresses.ammRouter, token1Amount);

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

80:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

148:       TransferHelper.safeApprove(_token, _target, _amount);

302:     TransferHelper.safeApprove(_tokenA, address(univ3_router), _amountAtoB);

```

```solidity
File: contracts/core/RdpxV2Bond.sol

25:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

26:     _setupRole(MINTER_ROLE, msg.sender);

```

```solidity
File: contracts/core/RdpxV2Core.sol

125:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

61:     _setupRole(MINTER_ROLE, msg.sender);

62:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

126:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

127:     _setupRole(MANAGER_ROLE, msg.sender);

207:     collateralToken.safeApprove(

```

```solidity
File: contracts/reLP/ReLPContract.sol

80:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

81:     _setupRole(RDPXV2CORE_ROLE, msg.sender);

150:     IERC20WithBurn(addresses.pair).safeApprove(

155:     IERC20WithBurn(addresses.tokenA).safeApprove(

160:     IERC20WithBurn(addresses.tokenB).safeApprove(

```

</details>

---

<a name="L-13"></a> 
### [L-13] Empty Function Body - Consider commenting why

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

235:   ) internal virtual {}

```

</details>

---

<a name="L-14"></a> 
### [L-14] `safeApprove()` is deprecated
[Deprecated](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/bfff03c0d2a59bcd8e2ead1da9aed9edf0080d05/contracts/token/ERC20/utils/SafeERC20.sol#L38-L45) in favor of `safeIncreaseAllowance()` and `safeDecreaseAllowance()`. If only setting the initial allowance to the value that means infinite, `safeIncreaseAllowance()` can be used instead. The function may currently work, but if a bug is found in this version of OpenZeppelin, and the version that you're forced to upgrade to no longer has this function, you'll encounter unnecessary delays in porting and testing replacement contracts.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

268:     IERC20WithBurn(addresses.pair).safeApprove(addresses.ammRouter, lpAmount);

328:     IERC20WithBurn(token1).safeApprove(addresses.ammRouter, token1Amount);

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

148:       TransferHelper.safeApprove(_token, _target, _amount);

302:     TransferHelper.safeApprove(_tokenA, address(univ3_router), _amountAtoB);

```

</details>

---


## Non Critical Issues

<a name="NC-1"></a> 
### [NC-1] Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, for readability
Well-organized data structures make code reviews easier, which may lead to fewer bugs. Consider combining related mappings into mappings to structs, so it's clear what data is related

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

69:   mapping(uint256 => mapping(uint256 => uint256))

```

</details>

---

<a name="NC-2"></a> 
### [NC-2] Consider adding formal verification proofs
Formal verification is the act of proving or disproving the correctness of intended algorithms underlying a system with respect to a certain formal specification/property/invariant, using formal methods of mathematics.

Some tools that are currently available to perform these tests on smart contracts are [SMTChecker](https://docs.soliditylang.org/en/latest/smtchecker.html) and [Certora Prover](https://www.certora.com/).

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-3"></a> 
### [NC-3] Constants should be put on the left side of comparisons
Putting constants on the left side of comparison statements is a best practice known as [Yoda conditions](https://en.wikipedia.org/wiki/Yoda_conditions). Although solidity's static typing system prevents accidental assignments within conditionals, adopting this practice can improve code readability and consistency, especially when working across multiple languages.

<details>
<summary>
There are <b>56</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

84:       _tokenA != address(0) &&

85:         _tokenB != address(0) &&

86:         _pair != address(0) &&

87:         _rdpxV2Core != address(0) &&

88:         _rdpxOracle != address(0) &&

89:         _ammFactory != address(0) &&

90:         _ammRouter != address(0),

131:     require(_token != address(0), "reLPContract: token cannot be 0");

132:     require(_spender != address(0), "reLPContract: spender cannot be 0");

```

```solidity
File: contracts/core/RdpxV2Core.sol

244:     require(_asset != address(0), "RdpxV2Core: asset cannot be 0 address");

274:     _validate(index != 0, 18);

316:     _validate(_dopexAMMRouter != address(0), 17);

317:     _validate(_dpxEthCurvePool != address(0), 17);

318:     _validate(_rdpxDecayingBonds != address(0), 17);

319:     _validate(_perpetualAtlanticVault != address(0), 17);

320:     _validate(_perpetualAtlanticVaultLP != address(0), 17);

321:     _validate(_rdpxReserve != address(0), 17);

322:     _validate(_rdpxV2ReceiptToken != address(0), 17);

323:     _validate(_feeDistributor != address(0), 17);

324:     _validate(_reLPContract != address(0), 17);

325:     _validate(_receiptTokenBonds != address(0), 17);

362:     _validate(_rdpxPriceOracle != address(0), 17);

363:     _validate(_dpxEthPriceOracle != address(0), 17);

379:     _validate(_addr != address(0), 17);

408:     _validate(_token != address(0), 17);

409:     _validate(_spender != address(0), 17);

630:     if (_bondId != 0) {

1091:     if (_rdpxAmount != 0) {

1162:     if (_rdpxBondId == 0) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

119:     _validate(_collateralToken != address(0), 1);

190:     _validate(_optionPricing != address(0), 1);

191:     _validate(_assetPriceOracle != address(0), 1);

192:     _validate(_volatilityOracle != address(0), 1);

193:     _validate(_feeDistributor != address(0), 1);

194:     _validate(_rdpx != address(0), 1);

195:     _validate(_perpetualAtlanticVaultLP != address(0), 1);

196:     _validate(_rdpxV2Core != address(0), 1);

467:         uint256 startTime = lastUpdateTime == 0

505:     uint256 startTime = lastUpdateTime == 0

578:     if (remainder == 0) {

595:     if (fundingRates[latestFundingPaymentPointer] == 0) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

95:       _perpetualAtlanticVault != address(0) || _rdpx != address(0),

95:       _perpetualAtlanticVault != address(0) || _rdpx != address(0),

123:     require((shares = previewDeposit(assets)) != 0, "ZERO_SHARES");

162:     require(assets != 0, "ZERO_ASSETS");

223:       (supply == 0)

283:       supply == 0 ? assets : assets.mulDivDown(supply, totalVaultCollateral);

```

```solidity
File: contracts/reLP/ReLPContract.sol

127:       _tokenA != address(0) &&

128:         _tokenB != address(0) &&

129:         _pair != address(0) &&

130:         _rdpxV2Core != address(0) &&

131:         _tokenAReserve != address(0) &&

132:         _amo != address(0) &&

133:         _rdpxOracle != address(0) &&

134:         _ammFactory != address(0) &&

135:         _ammRouter != address(0),

```

</details>

---

<a name="NC-4"></a> 
### [NC-4] Contracts should have full test coverage
While 100% code coverage does not guarantee that there are no bugs, it often will catch easy-to-find bugs, and will ensure that there are fewer regressions when the code invariably has to be modified. Furthermore, in order to get full coverage, code authors will often have to re-organize their code so that it is more modular, so that each component can be tested separately, which reduces interdependencies between modules and layers, and makes for code that is easier to reason about and audit.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-5"></a> 
### [NC-5] Events that mark critical parameter changes should contain both the old and the new value
This should especially be done if the new value is not required to be different from the old value.

<details>
<summary>
There are <b>37</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

152:     emit LogEmergencyWithdraw(msg.sender, tokens);

177:     emit LogAssetsTransfered(msg.sender, tokenABalance, tokenBBalance);

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

268:     emit log(positions_array.length);

269:     emit log(positions_mapping[pos.token_id].token_id);

321:     emit RecoveredERC20(tokenAddress, tokenAmount);

335:     emit RecoveredERC721(tokenAddress, token_id);

363:     emit LogAssetsTransfered(tokenABalance, tokenBBalance, tokenA, tokenB);

```

```solidity
File: contracts/core/RdpxV2Core.sol

172:     emit LogEmergencyWithdraw(msg.sender, tokens);

185:     emit LogSetRdpxBurnPercentage(_rdpxBurnPercentage);

198:     emit LogSetRdpxFeePercentage(_rdpxFeePercentage);

208:     emit LogSetIsReLPActive(_isReLPActive);

220:     emit LogSetputOptionsRequired(_putOptionsRequired);

233:     emit LogSetBondMaturity(_bondMaturity);

263:     emit LogAssetAddedTotokenReserves(_asset, _assetSymbol);

289:     emit LogAssetRemovedFromtokenReserves(_assetSymbol, index);

349:     emit LogSetAddresses(addresses);

370:     emit LogSetPricingOracleAddresses(pricingOracleAddresses);

447:     emit LogSetBondDiscountFactor(_bondDiscountFactor);

461:     emit LogSetSlippageTolerance(_slippageTolerance);

782:     emit LogSettle(optionIds);

807:     emit LogProvideFunding(pointer, fundingAmount);

932:     emit LogBond(rdpxRequired, wethRequired, receiptTokenAmount);

966:     emit LogAddToDelegate(_amount, _fee, delegates.length - 1);

989:     emit LogDelegateWithdraw(delegateId, amountWithdrawn);

1007:     emit LogSync();

1041:     emit LogRedeem(to, receiptTokenAmount);

1069:     emit LogUpperDepeg(_amount, wethReceived);

1123:     emit LogLowerDepeg(_rdpxAmount, _wethAmount, dpxEthReceived);

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

124:     emit BondMinted(to, bondId, expiry, rdpxAmount);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

211:     emit AddressesSet(addresses);

230:     emit EmergencyWithdraw(msg.sender, tokens);

311:     emit Purchase(strike, amount, premium, to, msg.sender);

368:     emit Settle(ethAmount, rdpxAmount, optionIds);

494:       emit FundingPaymentPointerUpdated(latestFundingPaymentPointer);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

134:     emit Deposit(msg.sender, receiver, assets, shares);

174:     emit Withdraw(msg.sender, receiver, owner, assets, shares);

```

```solidity
File: contracts/reLP/ReLPContract.sol

99:     emit LogSetReLpFactor(_reLPFactor);

```

</details>

---

<a name="NC-6"></a> 
### [NC-6] Custom errors should be used rather than `revert()`/`require()`
Custom errors are available from solidity version 0.8.4. Custom errors are more easily processed in try-catch blocks, and are easier to re-use and maintain.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

131:     require(_token != address(0), "reLPContract: token cannot be 0");

132:     require(_spender != address(0), "reLPContract: spender cannot be 0");

133:     require(_amount > 0, "reLPContract: amount must be greater than 0");

```

```solidity
File: contracts/core/RdpxV2Core.sol

244:     require(_asset != address(0), "RdpxV2Core: asset cannot be 0 address");

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

99:       require(success, "RdpxReserve: transfer failed");

120:     require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter");

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

123:     require((shares = previewDeposit(assets)) != 0, "ZERO_SHARES");

162:     require(assets != 0, "ZERO_ASSETS");

```

</details>

---

<a name="NC-7"></a> 
### [NC-7] Enable IR-based code generation
The IR-based code generator was introduced with an aim to not only allow code generation to be more transparent and auditable but also to enable more powerful optimization passes that span across functions. You can enable it on the command line using `--via-ir` or with the option `{"viaIR": true}`. This will take longer to compile, but you can just simple test it before deploying and if you got a better benchmark then you can add --via-ir to your deploy command More on: https://docs.soliditylang.org/en/v0.8.17/ir-breaking-changes.html

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-8"></a> 
### [NC-8] Import declarations should import specific identifiers, rather than the whole file
Using import declarations of the form `import {<identifier_name>} from "some/file.sol"` avoids polluting the symbol namespace making flattened files smaller, and speeds up compilation (but does not save any gas).

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

12: import "../uniswap_V3/IUniswapV3Factory.sol";

13: import "../uniswap_V3/libraries/TickMath.sol";

14: import "../uniswap_V3/libraries/LiquidityAmounts.sol";

15: import "../uniswap_V3/periphery/interfaces/INonfungiblePositionManager.sol";

16: import "../uniswap_V3/IUniswapV3Pool.sol";

17: import "../uniswap_V3/ISwapRouter.sol";

```

</details>

---

<a name="NC-9"></a> 
### [NC-9] Large or complicated code bases should implement invariant tests
This includes: large code bases, or code with lots of inline-assembly, complicated math, or complicated interactions between multiple contracts. Invariant fuzzers such as Echidna require the test writer to come up with invariants which should not be violated under any circumstances, and the fuzzer tests various inputs and function calls to ensure that the invariants always hold. Even code with 100% code coverage can still have bugs due to the order of the operations a user performs, and invariant fuzzers may help significantly.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="NC-10"></a> 
### [NC-10] Consider moving `msg.sender` checks to `modifier`s
If some functions are only allowed to be called by some specific users, consider using a modifier instead of checking with a require statement, especially if this check is done in multiple functions.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

120:     require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter");

```

</details>

---

<a name="NC-11"></a> 
### [NC-11] Named mappings are recommended
[Named mappings](https://docs.soliditylang.org/en/v0.8.18/types.html#mapping-types) (with syntax `mapping(KeyType KeyName? => ValueType ValueName?)`) are recommended.It can make the mapping variables clearer, more readable and easier to maintain.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

66:   mapping(uint256 => Position) public positions_mapping;

```

```solidity
File: contracts/core/RdpxV2Core.sol

73:   mapping(string => uint256) public reservesIndex;

76:   mapping(uint256 => Bond) public bonds;

79:   mapping(uint256 => bool) public optionsOwned;

82:   mapping(uint256 => bool) public fundingPaidFor;

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

37:   mapping(uint256 => Bond) public bonds;

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

63:   mapping(uint256 => OptionPosition) public optionPositions;

66:   mapping(uint256 => uint256) public fundingPaymentsAccountedFor;

69:   mapping(uint256 => mapping(uint256 => uint256))

73:   mapping(uint256 => uint256) public totalFundingForEpoch;

76:   mapping(uint256 => uint256) public optionsPerStrike;

79:   mapping(uint256 => uint256) public latestFundingPerStrike;

82:   mapping(uint256 => uint256) public fundingRates;

```

</details>

---

<a name="NC-12"></a> 
### [NC-12] There is no need to initialize variables with 0
Since the variables are automatically set to 0 when created, it is redundant to initialize it with 0 again.

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

89:   uint256 public latestFundingPaymentPointer = 0;

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```

</details>

---

<a name="NC-13"></a> 
### [NC-13] Put all system-wide constants in one file
Putting all the system-wide constants in a single file improves code readability, makes it easier to understand the basic configuration and limitations of the system, and makes maintenance easier.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

48:   uint256 public constant DEFAULT_PRECISION = 1e8;

```

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```

```solidity
File: contracts/core/RdpxV2Core.sol

85:   uint256 public constant DEFAULT_PRECISION = 1e8;

88:   uint256 public constant RDPX_RATIO_PERCENTAGE = 25 * DEFAULT_PRECISION;

91:   uint256 public constant ETH_RATIO_PERCENTAGE = 75 * DEFAULT_PRECISION;

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/reLP/ReLPContract.sol

67:   uint256 public constant DEFAULT_PRECISION = 1e8;

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

</details>

---

<a name="NC-14"></a> 
### [NC-14] Consider using `delete` rather than assigning zero to clear values
The `delete` keyword more closely matches the semantics of what is being done, and draws more attention to the changing of state, which may lead to a more thorough audit of its associated logic.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

343:       optionPositions[optionIds[i]].strike = 0;

```

</details>

---

<a name="NC-15"></a> 
### [NC-15] Expressions for constant values should use `immutable` rather than `constant`
While it doesn't save any gas because the compiler knows that developers often make this mistake, it's still best to use the right tool for the task at hand. There is a difference between `constant` variables and `immutable` variables, and they should each be used in their appropriate contexts. `constants` should be used for literal values written into the code, and `immutable` variables should be used for expressions, or values calculated in, or passed into the constructor.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

48:   uint256 public constant DEFAULT_PRECISION = 1e8;

```

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```

```solidity
File: contracts/core/RdpxV2Core.sol

85:   uint256 public constant DEFAULT_PRECISION = 1e8;

88:   uint256 public constant RDPX_RATIO_PERCENTAGE = 25 * DEFAULT_PRECISION;

91:   uint256 public constant ETH_RATIO_PERCENTAGE = 75 * DEFAULT_PRECISION;

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/reLP/ReLPContract.sol

67:   uint256 public constant DEFAULT_PRECISION = 1e8;

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

</details>

---

<a name="NC-16"></a> 
### [NC-16] Use of `override` is unnecessary
Starting with Solidity version [0.8.8](https://docs.soliditylang.org/en/v0.8.20/contracts.html#function-overriding), using the `override` keyword when the function solely overrides an interface function, and the function doesn't exist in multiple base contracts, is unnecessary.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/dpxETH/DpxEthToken.sol

50:   ) public override onlyRole(BURNER_ROLE) {

59:   ) internal override {

```

</details>

---

<a name="NC-17"></a> 
### [NC-17] Whitespace in Expressions
See the [Whitespace in Expressions](https://docs.soliditylang.org/en/latest/style-guide.html#whitespace-in-expressions) section of the Solidity Style Guide.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

105:     (uint128 liquidity, , , , ) = get_pool.positions(

193:     (uint256 tokenId, uint128 amountLiquidity, , ) = univ3_positions.mint(

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

98:       (bool success, ) = to.call{ value: amount, gas: gas }("");

```

</details>

---

<a name="NC-18"></a> 
### [NC-18] Return values of `approve()` not checked
Not all IERC20 implementations `revert()` when there's a failure in `approve()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually approving anything

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

134:     IERC20WithBurn(_token).approve(_spender, _amount);

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

150:       IERC20WithBurn(_token).approve(_target, _amount);

169:     IERC20WithBurn(params._tokenA).approve(

173:     IERC20WithBurn(params._tokenB).approve(

```

```solidity
File: contracts/core/RdpxV2Core.sol

339:     IERC20WithBurn(weth).approve(

343:     IERC20WithBurn(weth).approve(addresses.dopexAMMRouter, type(uint256).max);

344:     IERC20WithBurn(weth).approve(addresses.dpxEthCurvePool, type(uint256).max);

345:     IERC20WithBurn(weth).approve(

411:     IERC20WithBurn(_token).approve(_spender, _amount);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

245:       ? collateralToken.approve(

249:       : collateralToken.approve(addresses.perpetualAtlanticVaultLP, 0);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

106:     collateral.approve(_perpetualAtlanticVault, type(uint256).max);

107:     ERC20(rdpx).approve(_perpetualAtlanticVault, type(uint256).max);

```

</details>

---


## Gas Optimizations

<a name="GAS-1"></a> 
### [GAS-1] Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, where appropriate
Saves a storage slot for the mapping. Depending on the circumstances and sizes of types, can avoid a Gsset (20000 gas) per mapping combined. Reads and subsequent writes can also be cheaper when a function requires both values and they both fit in the same storage slot. Finally, if both fields are accessed in the same function, can save ~42 gas per access due to not having to [recalculate the key's keccak256 hash](https://gist.github.com/IllIllI000/ec23a57daa30a8f8ca8b9681c8ccefb0) (Gkeccak256 - 30 gas) and that calculation's associated stack operations.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

69:   mapping(uint256 => mapping(uint256 => uint256))

```

</details>

---

<a name="GAS-2"></a> 
### [GAS-2] Consider activating via-ir for deploying
By using `--via-ir` or `{"viaIR": true}`, the compiler is able to use more advanced [multi-function optimizations](https://docs.soliditylang.org/en/v0.8.17/ir-breaking-changes.html#solidity-ir-based-codegen-changes), for extra gas savings.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity

Global finding

```

</details>

---

<a name="GAS-3"></a> 
### [GAS-3] Divisions can be `unchecked` to save gas
The expression `type(int).min/(-1)` is the only case where division causes an overflow. Therefore, uncheck can be used to [save gas](https://gist.github.com/DadeKuma/3bc597338ae774b8b3bd43280d55271f) in scenarios where it is certain that such an overflow will not occur.

<details>
<summary>
There are <b>52</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

373:     return (lpTokenBalance * getLpPrice()) / 1e8;

```

```solidity
File: contracts/core/RdpxV2Core.sol

535:           ethBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

539:           dpxEthBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

546:       ? (((_amount * getDpxEthPrice()) / 1e8) -

547:         (((_amount * getDpxEthPrice()) * slippageTolerance) / 1e16))

548:       : (((_amount * getEthPrice()) / 1e8) -

549:         (((_amount * getEthPrice()) * slippageTolerance) / 1e16));

570:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= _amount / 2;

574:       _amount / 2

579:       .deposit(_amount / 2);

605:     uint256 rdpxRequiredInWeth = (_rdpxRequired * getRdpxPrice()) / 1e8;

608:     amount1 = ((rdpxRequiredInWeth * _amount) /

612:     amount1 = (amount1 * (100e8 - _delegateFee)) / 1e10;

658:         (_rdpxAmount * rdpxBurnPercentage) / 1e10

665:           (_rdpxAmount * rdpxFeePercentage) / 1e10

669:       uint256 rdpxAmountInWeth = (_rdpxAmount * getRdpxPrice()) / 1e8;

673:       uint256 extraRdpxToWithdraw = (discountReceivedInWeth * 1e8) /

1165:         1e2) / (Math.sqrt(1e18)); // 1e8 precision

1170:         ((RDPX_RATIO_PERCENTAGE - (bondDiscount / 2)) *

1172:           DEFAULT_PRECISION) /

1176:         ((ETH_RATIO_PERCENTAGE - (bondDiscount / 2)) * _amount) /

1176:         ((ETH_RATIO_PERCENTAGE - (bondDiscount / 2)) * _amount) /

1181:         (RDPX_RATIO_PERCENTAGE * _amount * DEFAULT_PRECISION) /

1185:         (ETH_RATIO_PERCENTAGE * _amount) /

1190:       .roundUp(rdpxPrice - (rdpxPrice / 4)); // 25% below the current price

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

270:     uint256 strike = roundUp(currentPrice - (currentPrice / 4)); // 25% below the current price

276:     uint256 requiredCollateral = (amount * strike) / 1e8;

335:       ethAmount += (amount * strike) / 1e8;

475:           (currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

481:             (currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

487:           ((currentFundingRate * (nextFundingPaymentTimestamp() - startTime)) /

512:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

516:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

521:       ((currentFundingRate * (block.timestamp - startTime)) / 1e18),

550:     ) * _amount) / 1e8);

559:     return strike > price ? ((strike - price) * amount) / 1e8 : 0;

604:         (amount * 1e18) /

612:         ((amount * 1e18) / (endTime - startTime));

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

281:       ((_rdpxCollateral * rdpxPriceInAlphaToken) / 1e8);

```

```solidity
File: contracts/reLP/ReLPContract.sol

230:       1e2) / (Math.sqrt(1e18)); // 1e6 precision

232:     uint256 tokenAToRemove = ((((_amount * 4) * 1e18) /

235:       baseReLpRatio) / (1e18 * DEFAULT_PRECISION * 1e2);

239:     uint256 lpToRemove = (tokenAToRemove * totalLpSupply) /

251:       ((tokenAToRemove * liquiditySlippageTolerance) / 1e8);

252:     uint256 mintokenBAmount = ((tokenAToRemove * tokenAInfo.tokenAPrice) /

254:       ((tokenAToRemove * tokenAInfo.tokenAPrice) * liquiditySlippageTolerance) /

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

279:         amountB / 2,

290:       amountB / 2,

```

</details>

---

<a name="GAS-4"></a> 
### [GAS-4] Don't transfer with zero amount to save gas
In Solidity, unnecessary operations can waste gas. For example, a transfer function without a zero amount check uses gas even if called with a zero amount, since the contract state remains unchanged. Implementing a zero amount check avoids these unnecessary function calls, saving gas and improving efficiency.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

170:     collateral.transfer(receiver, assets);

```

</details>

---

<a name="GAS-5"></a> 
### [GAS-5] Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables

<details>
<summary>
There are <b>41</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

235:     lpTokenBalance += lpReceived;

283:     lpTokenBalance -= lpAmount;

```

```solidity
File: contracts/core/RdpxV2Core.sol

486:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= premium;

570:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= _amount / 2;

650:       reserveAsset[reservesIndex["RDPX"]].tokenBalance += _rdpxAmount;

681:       reserveAsset[reservesIndex["RDPX"]].tokenBalance +=

711:     reserveAsset[reservesIndex["WETH"]].tokenBalance += wethRequired;

717:     delegate.activeCollateral += wethRequired;

720:     totalWethDelegated -= wethRequired;

779:     reserveAsset[reservesIndex["WETH"]].tokenBalance += amountOfWeth;

780:     reserveAsset[reservesIndex["RDPX"]].tokenBalance -= rdpxAmount;

803:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= fundingAmount;

851:       userTotalBondAmount += returnValues.bondAmountForUser;

852:       totalBondAmount += _amounts[i];

916:     reserveAsset[reservesIndex["WETH"]].tokenBalance += wethRequired;

964:     totalWethDelegated += _amount;

1067:     reserveAsset[reservesIndex["WETH"]].tokenBalance += wethReceived;

1106:       reserveAsset[reservesIndex["RDPX"]].tokenBalance -= _rdpxAmount;

1110:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= _wethAmount;

1196:       wethRequired += IPerpetualAtlanticVault(addresses.perpetualAtlanticVault)

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

302:     totalActiveOptions += amount;

303:     fundingPaymentsAccountedFor[latestFundingPaymentPointer] += amount;

304:     optionsPerStrike[strike] += amount;

309:     ] += amount;

335:       ethAmount += (amount * strike) / 1e8;

336:       rdpxAmount += amount;

337:       optionsPerStrike[strike] -= amount;

338:       totalActiveOptions -= amount;

437:       fundingAmount += premium;

440:       fundingPaymentsAccountedFor[latestFundingPaymentPointer] += amount;

445:       ] += amount;

449:       totalFundingForEpoch[latestFundingPaymentPointer] += premium;

493:       latestFundingPaymentPointer += 1;

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

132:     _totalCollateral += assets;

164:     _rdpxCollateral -= rdpxAmount;

181:     _activeCollateral += amount;

186:     _activeCollateral -= amount;

195:     _totalCollateral += proceeds;

204:     _totalCollateral -= loss;

213:     _rdpxCollateral += amount;

291:     _totalCollateral -= assets;

```

</details>

---

<a name="GAS-6"></a> 
### [GAS-6] `keccak256()` hash of literals should only be computed once
The result of the hash should be stored in an immutable variable, and the variable should be used instead. If the hash is being used as a part of a function selector, the cast to `bytes4` should also only be done once.

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/reLP/ReLPContract.sol

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

</details>

---

<a name="GAS-7"></a> 
### [GAS-7] Operator `>=`/`<=` costs less gas than operator `>`/`<`
The compiler uses opcodes `GT` and `ISZERO` for code that uses `>`, but only requires `LT` for `>=`. A similar behavior applies for `>`, which uses opcodes `LT` and `ISZERO`, but only requires `GT` for `<=`. It can save 3 gas for each. It should be converted to the `<=`/`>=` equivalent when comparing against integer literals.

<details>
<summary>
There are <b>38</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

113:       _slippageTolerance > 0,

133:     require(_amount > 0, "reLPContract: amount must be greater than 0");

147:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

183:     _validate(_rdpxBurnPercentage > 0, 3);

196:     _validate(_rdpxFeePercentage > 0, 3);

231:     _validate(_bondMaturity > 0, 3);

246:     for (uint256 i = 1; i < reserveAsset.length; i++) {

391:     _validate(_index < amoAddresses.length, 18);

410:     _validate(_amount > 0, 17);

444:     _validate(_bondDiscountFactor > 0, 3);

458:     _validate(_slippageTolerance > 0, 3);

556:       minAmount > 0 ? minAmount : minOut

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

901:     _validate(_amount > 0, 4);

947:     _validate(_fee < 100e8, 8);

949:     _validate(_amount > 1e16, 4);

979:     _validate(delegateId < delegates.length, 14);

984:     _validate(amountWithdrawn > 0, 15);

996:     for (uint256 i = 1; i < reserveAsset.length; i++) {

1021:     _validate(bonds[id].timestamp > 0, 6);

1023:     _validate(block.timestamp > bonds[id].maturity, 7);

1167:       _validate(bondDiscount < 100e8, 14);

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

156:     for (uint256 i; i < ownerTokenCount; i++) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

225:     for (uint256 i = 0; i < tokens.length; i++) {

265:     _validate(amount > 0, 2);

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

464:       if (lastUpdateTime < nextFundingPaymentTimestamp()) {

547:       _price > 0 ? _price : getUnderlyingPrice(),

559:     return strike > price ? ((strike - price) * amount) / 1e8 : 0;

597:       if (lastUpdateTime > nextFundingPaymentTimestamp() - fundingDuration) {

```

```solidity
File: contracts/reLP/ReLPContract.sol

94:       _reLPFactor > 0,

175:       _liquiditySlippageTolerance > 0,

190:       _slippageTolerance > 0,

```

</details>

---

<a name="GAS-8"></a> 
### [GAS-8] Use assembly to compute hashes to save gas
If the arguments to the encode call can fit into the scratch space (two words or fewer), then it's more efficient to use assembly to generate the hash (80 gas):

`keccak256(abi.encodePacked(x, y)) -> assembly {mstore(0x00, a); mstore(0x20, b); let hash := keccak256(0x00, 0x40); }`

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

106:       keccak256(abi.encodePacked(address(this), _tickLower, _tickUpper))

```

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```

```solidity
File: contracts/core/RdpxV2Core.sol

1141:       keccak256(abi.encodePacked(asset.tokenSymbol)) ==

1142:         keccak256(abi.encodePacked(_token)),

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/reLP/ReLPContract.sol

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

</details>

---

<a name="GAS-9"></a> 
### [GAS-9] Use assembly to emit events
To efficiently emit events, it's possible to utilize assembly by making use of scratch space and the free memory pointer. This approach has the advantage of potentially avoiding the costs associated with memory expansion.

However, it's important to note that in order to safely optimize this process, it is preferable to cache and restore the free memory pointer.

A good example of such practice can be seen in [Solady's](https://github.com/Vectorized/solady/blob/main/src/tokens/ERC1155.sol#L167) codebase.

<details>
<summary>
There are <b>45</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

152:     emit LogEmergencyWithdraw(msg.sender, tokens);

177:     emit LogAssetsTransfered(msg.sender, tokenABalance, tokenBBalance);

240:     emit LogAddLiquidity(

288:     emit LogRemoveLiquidity(

348:     emit LogSwap(

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

268:     emit log(positions_array.length);

269:     emit log(positions_mapping[pos.token_id].token_id);

321:     emit RecoveredERC20(tokenAddress, tokenAmount);

335:     emit RecoveredERC721(tokenAddress, token_id);

363:     emit LogAssetsTransfered(tokenABalance, tokenBBalance, tokenA, tokenB);

```

```solidity
File: contracts/core/RdpxV2Core.sol

172:     emit LogEmergencyWithdraw(msg.sender, tokens);

185:     emit LogSetRdpxBurnPercentage(_rdpxBurnPercentage);

198:     emit LogSetRdpxFeePercentage(_rdpxFeePercentage);

208:     emit LogSetIsReLPActive(_isReLPActive);

220:     emit LogSetputOptionsRequired(_putOptionsRequired);

233:     emit LogSetBondMaturity(_bondMaturity);

263:     emit LogAssetAddedTotokenReserves(_asset, _assetSymbol);

289:     emit LogAssetRemovedFromtokenReserves(_assetSymbol, index);

349:     emit LogSetAddresses(addresses);

370:     emit LogSetPricingOracleAddresses(pricingOracleAddresses);

447:     emit LogSetBondDiscountFactor(_bondDiscountFactor);

461:     emit LogSetSlippageTolerance(_slippageTolerance);

782:     emit LogSettle(optionIds);

807:     emit LogProvideFunding(pointer, fundingAmount);

875:     emit LogBondWithDelegate(

932:     emit LogBond(rdpxRequired, wethRequired, receiptTokenAmount);

966:     emit LogAddToDelegate(_amount, _fee, delegates.length - 1);

989:     emit LogDelegateWithdraw(delegateId, amountWithdrawn);

1007:     emit LogSync();

1041:     emit LogRedeem(to, receiptTokenAmount);

1069:     emit LogUpperDepeg(_amount, wethReceived);

1123:     emit LogLowerDepeg(_rdpxAmount, _wethAmount, dpxEthReceived);

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

124:     emit BondMinted(to, bondId, expiry, rdpxAmount);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

211:     emit AddressesSet(addresses);

230:     emit EmergencyWithdraw(msg.sender, tokens);

311:     emit Purchase(strike, amount, premium, to, msg.sender);

368:     emit Settle(ethAmount, rdpxAmount, optionIds);

389:     emit PayFunding(

451:       emit CalculateFunding(

485:         emit FundingPaid(

494:       emit FundingPaymentPointerUpdated(latestFundingPaymentPointer);

519:     emit FundingPaid(

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

134:     emit Deposit(msg.sender, receiver, assets, shares);

174:     emit Withdraw(msg.sender, receiver, owner, assets, shares);

```

```solidity
File: contracts/reLP/ReLPContract.sol

99:     emit LogSetReLpFactor(_reLPFactor);

```

</details>

---

<a name="GAS-10"></a> 
### [GAS-10] Using a double `if` statement instead of a logical AND (`&&`)
Using a double `if` statement instead of a logical AND (`&&`) can provide similar short-circuiting behavior whereas double if is slightly [more gas efficient](https://gist.github.com/DadeKuma/931ce6794a050201ec6544dbcc31316c).

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

84:       _tokenA != address(0) &&

85:         _tokenB != address(0) &&

86:         _pair != address(0) &&

87:         _rdpxV2Core != address(0) &&

88:         _rdpxOracle != address(0) &&

89:         _ammFactory != address(0) &&

```

```solidity
File: contracts/reLP/ReLPContract.sol

127:       _tokenA != address(0) &&

128:         _tokenB != address(0) &&

129:         _pair != address(0) &&

130:         _rdpxV2Core != address(0) &&

131:         _tokenAReserve != address(0) &&

132:         _amo != address(0) &&

133:         _rdpxOracle != address(0) &&

134:         _ammFactory != address(0) &&

```

</details>

---

<a name="GAS-11"></a> 
### [GAS-11] Use `storage` instead of `memory` for structs/arrays
When fetching data from a storage location, assigning the data to a `memory` variable causes all fields of the struct/array to be read from storage, which incurs a Gcoldsload (**2100 gas**) for *each* field of the struct/array. If the fields are read from the new memory variable, they incur an additional `MLOAD` rather than a cheap stack read. Instead of declaring the variable with the `memory` keyword, declaring the variable with the `storage` keyword and caching any fields that need to be re-read in stack variables, will be much cheaper, only incurring the Gcoldsload for the fields actually read. The only time it makes sense to read the whole struct/array into a `memory` variable, is if the full struct/array is being returned by the function, is being passed to a function that requires `memory`, or if the array/struct is being read from another `memory` array/struct.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

121:       Position memory current_position = positions_array[i];

218:     Position memory pos = positions_array[positionIndex];

```

```solidity
File: contracts/core/RdpxV2Core.sol

1138:     ReserveAsset memory asset = reserveAsset[reservesIndex[_token]];

1272:     Delegate memory delegatePosition = delegates[_delegateId];

```

</details>

---

<a name="GAS-12"></a> 
### [GAS-12] Using bitmap to store bool states can save gas
Using a bitmap instead of a bool array or a bool mapping to store boolean states can save gas fees. This is because the bitmap can store 256 boolean values in a single slot instead of 256 slots, which can save gas when writing bool values or when reading multiple bool values from the same slot.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/core/RdpxV2Core.sol

79:   mapping(uint256 => bool) public optionsOwned;

82:   mapping(uint256 => bool) public fundingPaidFor;

```

</details>

---

<a name="GAS-13"></a> 
### [GAS-13] Using bools for storage incurs overhead
Use uint256(1) and uint256(2) for true/false to avoid a Gwarmaccess (100 gas), and to avoid Gsset (20000 gas) when changing from ‘false’ to ‘true’, after having been ‘true’ in the past. See [source](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/58f635312aa21f947cae5f8578638a85aa2519f5/contracts/security/ReentrancyGuard.sol#L23-L27).

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/core/RdpxV2Core.sol

79:   mapping(uint256 => bool) public optionsOwned;

82:   mapping(uint256 => bool) public fundingPaidFor;

115:   bool public isReLPActive;

118:   bool public putOptionsRequired;

```

</details>

---

<a name="GAS-14"></a> 
### [GAS-14] Cache array length outside of loop
If not cached, the solidity compiler will always read the length of the array during each iteration. That is, if it is a storage array, this is an extra sload operation (100 additional extra gas for each iteration except for the first) and if it is a memory array, this is an extra mload operation (3 additional gas for each iteration except for the first).

<details>
<summary>
There are <b>11</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

246:     for (uint256 i = 1; i < reserveAsset.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

996:     for (uint256 i = 1; i < reserveAsset.length; i++) {

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```

</details>

---

<a name="GAS-15"></a> 
### [GAS-15] Use Custom Errors
[Source](https://blog.soliditylang.org/2021/04/21/custom-errors/)
Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

131:     require(_token != address(0), "reLPContract: token cannot be 0");

132:     require(_spender != address(0), "reLPContract: spender cannot be 0");

133:     require(_amount > 0, "reLPContract: amount must be greater than 0");

```

```solidity
File: contracts/core/RdpxV2Core.sol

244:     require(_asset != address(0), "RdpxV2Core: asset cannot be 0 address");

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

99:       require(success, "RdpxReserve: transfer failed");

120:     require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter");

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

123:     require((shares = previewDeposit(assets)) != 0, "ZERO_SHARES");

162:     require(assets != 0, "ZERO_ASSETS");

```

</details>

---

<a name="GAS-16"></a> 
### [GAS-16] Don't use `SafeMath` once the solidity version is 0.8.0 or greater
Solidity 0.8.0 introduces internal overflow checks, so using SafeMath is redundant and adds overhead.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

6: import { SafeMath } from "@openzeppelin/contracts/utils/math/SafeMath.sol";

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

7: import { SafeMath } from "@openzeppelin/contracts/utils/math/SafeMath.sol";

```

```solidity
File: contracts/reLP/ReLPContract.sol

6: import { SafeMath } from "@openzeppelin/contracts/utils/math/SafeMath.sol";

```

</details>

---

<a name="GAS-17"></a> 
### [GAS-17] Don't initialize variables with default value

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

89:   uint256 public latestFundingPaymentPointer = 0;

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```

</details>

---

<a name="GAS-18"></a> 
### [GAS-18] Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead
Using `int`s/`uint`s smaller than 32 bytes may cost more gas. This is because the EVM operates on 32 bytes at a time, so if an element is smaller than 32 bytes, the EVM must perform more operations to reduce the size of the element from 32 bytes to the desired size.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

43:     uint128 liquidity; // the liquidity of the position

99:   ) public view returns (uint128) {

105:     (uint128 liquidity, , , , ) = get_pool.positions(

126:           type(uint128).max,

127:           type(uint128).max

193:     (uint256 tokenId, uint128 amountLiquidity, , ) = univ3_positions.mint(

223:         type(uint128).max,

224:         type(uint128).max

235:       uint128 liquidity,

280:     uint160 _sqrtPriceLimitX96

```

```solidity
File: contracts/core/RdpxV2Core.sol

553:       _ethToDpxEth ? int128(int256(a)) : int128(int256(b)),

553:       _ethToDpxEth ? int128(int256(a)) : int128(int256(b)),

554:       _ethToDpxEth ? int128(int256(b)) : int128(int256(a)),

554:       _ethToDpxEth ? int128(int256(b)) : int128(int256(a)),

```

</details>

---

<a name="GAS-19"></a> 
### [GAS-19] Constructors can be marked as `payable` to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. A constructor can be safely marked as payable, because only the deployer would be able to pass funds, and the project itself would not pass any funds.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

57:   constructor() {

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

76:   constructor(address _rdpx, address _rdpxV2Core) {

```

```solidity
File: contracts/core/RdpxV2Bond.sol

24:   constructor() ERC721("rDPX V2 Bond", "rDPXV2Bond") {

```

```solidity
File: contracts/core/RdpxV2Core.sol

124:   constructor(address _weth) {

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

23:   constructor() ERC20("Dopex Synthetic ETH", "dpxETH") {

```

```solidity
File: contracts/reLP/ReLPContract.sol

79:   constructor() {

```

</details>

---

<a name="GAS-20"></a> 
### [GAS-20] Functions guaranteed to revert when called by normal users can be marked `payable`
If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function. Marking the function as `payable` will lower the gas cost for legitimate callers because the compiler will not include checks for whether a payment was provided.

<details>
<summary>
There are <b>22</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

119:   function collectFees() external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/core/RdpxV2Bond.sol

29:   function pause() public onlyRole(DEFAULT_ADMIN_ROLE) {

33:   function unpause() public onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/core/RdpxV2Core.sol

144:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

152:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

206:   function setIsreLP(bool _isReLPActive) external onlyRole(DEFAULT_ADMIN_ROLE) {

378:   function addAMOAddress(address _addr) external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

70:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

76:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

29:   function pause() public onlyRole(PAUSER_ROLE) {

33:   function unpause() public onlyRole(PAUSER_ROLE) {

37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

136:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

144:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

243:   function setLpAllowance(bool increase) external onlyRole(DEFAULT_ADMIN_ROLE) {

372:   function payFunding() external onlyRole(RDPXV2CORE_ROLE) returns (uint256) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

180:   function lockCollateral(uint256 amount) public onlyPerpVault {

185:   function unlockLiquidity(uint256 amount) public onlyPerpVault {

190:   function addProceeds(uint256 proceeds) public onlyPerpVault {

199:   function subtractLoss(uint256 loss) public onlyPerpVault {

208:   function addRdpx(uint256 amount) public onlyPerpVault {

```

```solidity
File: contracts/reLP/ReLPContract.sol

202:   function reLP(uint256 _amount) external onlyRole(RDPXV2CORE_ROLE) {

```

</details>

---

<a name="GAS-21"></a> 
### [GAS-21] `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too)
*Saves 5 gas per loop*

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

246:     for (uint256 i = 1; i < reserveAsset.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

996:     for (uint256 i = 1; i < reserveAsset.length; i++) {

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

156:     for (uint256 i; i < ownerTokenCount; i++) {

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```

</details>

---

<a name="GAS-22"></a> 
### [GAS-22] Using `private` rather than `public` for constants, saves gas
If needed, the values can be read from the verified contract source code, or if there are multiple values there can be a single getter function that [returns a tuple](https://github.com/code-423n4/2022-08-frax/blob/90f55a9ce4e25bceed3a74290b854341d8de6afa/src/contracts/FraxlendPair.sol#L156-L178) of the values of all currently-public constants. Saves **3406-3606 gas** in deployment gas due to the compiler not having to create non-payable getter functions for deployment calldata, not having to store the bytes of the value outside of where it's used, and not adding another entry to the method ID table

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

48:   uint256 public constant DEFAULT_PRECISION = 1e8;

```

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```

```solidity
File: contracts/core/RdpxV2Core.sol

85:   uint256 public constant DEFAULT_PRECISION = 1e8;

88:   uint256 public constant RDPX_RATIO_PERCENTAGE = 25 * DEFAULT_PRECISION;

91:   uint256 public constant ETH_RATIO_PERCENTAGE = 75 * DEFAULT_PRECISION;

```

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

```solidity
File: contracts/reLP/ReLPContract.sol

67:   uint256 public constant DEFAULT_PRECISION = 1e8;

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```

</details>

---

<a name="GAS-23"></a> 
### [GAS-23] Use shift Right/Left instead of division/multiplication if possible

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/core/RdpxV2Core.sol

535:           ethBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

539:           dpxEthBalance + _amount <= (ethBalance + dpxEthBalance) / 2,

570:     reserveAsset[reservesIndex["WETH"]].tokenBalance -= _amount / 2;

574:       _amount / 2

579:       .deposit(_amount / 2);

1170:         ((RDPX_RATIO_PERCENTAGE - (bondDiscount / 2)) *

1176:         ((ETH_RATIO_PERCENTAGE - (bondDiscount / 2)) * _amount) /

1190:       .roundUp(rdpxPrice - (rdpxPrice / 4)); // 25% below the current price

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

270:     uint256 strike = roundUp(currentPrice - (currentPrice / 4)); // 25% below the current price

```

```solidity
File: contracts/reLP/ReLPContract.sol

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

279:         amountB / 2,

290:       amountB / 2,

```

</details>

---

<a name="GAS-24"></a> 
### [GAS-24] Use `!= 0` instead of `> 0` for unsigned integer comparison
Using `== 0`, `!= 0` instead of `> 0`, `>= 1`, `< 1`, `<= 0` can save gas.

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

113:       _slippageTolerance > 0,

133:     require(_amount > 0, "reLPContract: amount must be greater than 0");

```

```solidity
File: contracts/core/RdpxV2Core.sol

183:     _validate(_rdpxBurnPercentage > 0, 3);

196:     _validate(_rdpxFeePercentage > 0, 3);

231:     _validate(_bondMaturity > 0, 3);

410:     _validate(_amount > 0, 17);

444:     _validate(_bondDiscountFactor > 0, 3);

458:     _validate(_slippageTolerance > 0, 3);

556:       minAmount > 0 ? minAmount : minOut

838:       _validate(_amounts[i] > 0, 4);

901:     _validate(_amount > 0, 4);

984:     _validate(amountWithdrawn > 0, 15);

1021:     _validate(bonds[id].timestamp > 0, 6);

```

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

265:     _validate(amount > 0, 2);

414:       _validate(optionsPerStrike[strikes[i]] > 0, 4);

547:       _price > 0 ? _price : getUnderlyingPrice(),

```

```solidity
File: contracts/reLP/ReLPContract.sol

94:       _reLPFactor > 0,

175:       _liquiditySlippageTolerance > 0,

190:       _slippageTolerance > 0,

```

</details>

---

