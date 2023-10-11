# Report


## Medium Issues


Total <b>108</b> instances over <b>5</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | The remaining ETH may be locked in the contract after call | 2 |
| [M-2](#M-2) | Return values of `approve()` not checked | 13 |
| [M-3](#M-3) | Return values of `transfer()`/`transferFrom()` not checked | 6 |
| [M-4](#M-4) | Unsafe use of ERC20 `transfer()`/`transferFrom()`/`approve()` | 4 |
| [M-5](#M-5) | Centralization Risk for trusted owners | 83 |

## Low Issues


Total <b>235</b> instances over <b>24</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | `approve()`/`safeApprove()` may revert if the current approval is not zero | 23 |
| [L-2](#L-2) | Array is `push()`ed but not `pop()`ed | 1 |
| [L-3](#L-3) | Check division by zero is prevented | 52 |
| [L-4](#L-4) | Constructor / initialization function lacks parameter validation | 5 |
| [L-5](#L-5) | Enum values should be used instead of constant array indexes | 6 |
| [L-6](#L-6) | External call recipient can consume all remaining gas | 1 |
| [L-7](#L-7) | Governance functions should be controlled by time locks | 2 |
| [L-8](#L-8) | Loss of precision in divisions | 52 |
| [L-9](#L-9) | Missing contract existence checks before low-level calls | 2 |
| [L-10](#L-10) | Missing zero address check in constructor | 3 |
| [L-11](#L-11) | Consider some checks for `address(0)` when setting address state variables | 4 |
| [L-12](#L-12) | prevent re-setting a state variable with the same value | 21 |
| [L-13](#L-13) | `SafeTransferLib` does not ensure that the token contract exists | 1 |
| [L-14](#L-14) | Some tokens may revert when large transfers are made | 1 |
| [L-15](#L-15) | Some tokens may revert when zero value transfers are made | 1 |
| [L-16](#L-16) | Timestamp may be manipulation | 19 |
| [L-17](#L-17) | Tokens may be minted to `address(0)` | 3 |
| [L-18](#L-18) | Unsafe solidity low-level call can cause gas grief attack | 2 |
| [L-19](#L-19) | Using zero as a parameter | 6 |
| [L-20](#L-20) |  `abi.encodePacked()` should not be used with dynamic types when passing the result to a hash function such as `keccak256()` | 3 |
| [L-21](#L-21) | `decimals()` is not a part of the ERC-20 standard | 1 |
| [L-22](#L-22) | Do not use deprecated library functions | 21 |
| [L-23](#L-23) | Empty Function Body - Consider commenting why | 1 |
| [L-24](#L-24) | `safeApprove()` is deprecated | 4 |

## Non Critical Issues


Total <b>611</b> instances over <b>50</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Add inline comments for unnamed variables | 2 |
| [NC-2](#NC-2) | Contract declarations should have NatSpec `@author` annotations | 2 |
| [NC-3](#NC-3) | Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, for readability | 1 |
| [NC-4](#NC-4) | Consider adding a block/deny-list | 10 |
| [NC-5](#NC-5) | Consider adding formal verification proofs | 1 |
| [NC-6](#NC-6) | Consider bounding input array length | 7 |
| [NC-7](#NC-7) | Constants should be put on the left side of comparisons | 56 |
| [NC-8](#NC-8) | Contract uses both `require()`/`revert()` as well as custom errors | 1 |
| [NC-9](#NC-9) | Contracts should have full test coverage | 1 |
| [NC-10](#NC-10) | Convert simple `if` statements to ternary expressions | 1 |
| [NC-11](#NC-11) | Events that mark critical parameter changes should contain both the old and the new value | 37 |
| [NC-12](#NC-12) | Custom errors should be used rather than `revert()`/`require()` | 8 |
| [NC-13](#NC-13) | `else` block not required | 1 |
| [NC-14](#NC-14) | Empty bytes check is missing | 1 |
| [NC-15](#NC-15) | Enable IR-based code generation | 1 |
| [NC-16](#NC-16) | Names of structs, events, enums and errors should use CapWords style | 1 |
| [NC-17](#NC-17) | Events are emitted without the sender information | 29 |
| [NC-18](#NC-18) | Import declarations should import specific identifiers, rather than the whole file | 6 |
| [NC-19](#NC-19) | Invalid NatSpec comment style | 1 |
| [NC-20](#NC-20) | Large or complicated code bases should implement invariant tests | 1 |
| [NC-21](#NC-21) | Long functions should be refactored into multiple, smaller, functions | 11 |
| [NC-22](#NC-22) | Magic numbers should be replaced with constants | 41 |
| [NC-23](#NC-23) | Missing zero address check in functions with address parameters | 34 |
| [NC-24](#NC-24) | Consider moving `msg.sender` checks to `modifier`s | 1 |
| [NC-25](#NC-25) | Named mappings are recommended | 13 |
| [NC-26](#NC-26) | NatSpec documentation for contract is missing | 2 |
| [NC-27](#NC-27) | Event declarations should have NatSpec descriptions | 14 |
| [NC-28](#NC-28) | NatSpec documentation for function is missing | 39 |
| [NC-29](#NC-29) | Modifier declarations should have NatSpec descriptions | 1 |
| [NC-30](#NC-30) | Missing NatSpec `@param` | 89 |
| [NC-31](#NC-31) | Public variable declarations should have NatSpec descriptions | 15 |
| [NC-32](#NC-32) | NatSpec `@return` is missing | 34 |
| [NC-33](#NC-33) | There is no need to initialize variables with 0 | 10 |
| [NC-34](#NC-34) | Put all system-wide constants in one file | 14 |
| [NC-35](#NC-35) | Contract declarations should have NatSpec `@title` annotations | 1 |
| [NC-36](#NC-36) | Unused named return | 8 |
| [NC-37](#NC-37) | Unused contract variables | 1 |
| [NC-38](#NC-38) | Consider using `delete` rather than assigning zero to clear values | 1 |
| [NC-39](#NC-39) | Expressions for constant values should use `immutable` rather than `constant` | 14 |
| [NC-40](#NC-40) | Use the latest solidity version for deployment | 9 |
| [NC-41](#NC-41) | Use of `override` is unnecessary | 2 |
| [NC-42](#NC-42) | Visibility of state variables is not explicitly defined | 1 |
| [NC-43](#NC-43) | Whitespace in Expressions | 3 |
| [NC-44](#NC-44) | Missing checks for `address(0)` when assigning values to address state variables | 4 |
| [NC-45](#NC-45) | Common functions should be refactored to a common base contract | 8 |
| [NC-46](#NC-46) | Names of `private`/`internal` functions should be prefixed with an underscore | 1 |
| [NC-47](#NC-47) | Return values of `approve()` not checked | 13 |
| [NC-48](#NC-48) | Variables should be named in mixedCase style | 14 |
| [NC-49](#NC-49) | Event is missing `indexed` fields | 13 |
| [NC-50](#NC-50) | Functions not used internally could be marked `external` | 32 |

## Gas Optimizations


Total <b>518</b> instances over <b>40</b> issues:

|ID|Issue|Instances|Gas|
|-|:-|:-:|:-:|
| [GAS-1](#GAS-1) | Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, where appropriate | 1 | - |
| [GAS-2](#GAS-2) | Consider activating via-ir for deploying | 1 | - |
| [GAS-3](#GAS-3) | Divisions can be `unchecked` to save gas | 52 | 1040 |
| [GAS-4](#GAS-4) | Don't transfer with zero amount to save gas | 1 | - |
| [GAS-5](#GAS-5) | Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables | 41 | 4633 |
| [GAS-6](#GAS-6) | `internal` functions only called once can be inlined to save gas | 5 | 150 |
| [GAS-7](#GAS-7) | `keccak256()` hash of literals should only be computed once | 9 | 378 |
| [GAS-8](#GAS-8) | Low level `call` can be optimized with assembly | 2 | 496 |
| [GAS-9](#GAS-9) | Multiple accesses of the same mapping/array key/index should be cached | 17 | 714 |
| [GAS-10](#GAS-10) | Newer versions of solidity are more gas efficient | 9 | - |
| [GAS-11](#GAS-11) | Operator `>=`/`<=` costs less gas than operator `>`/`<` | 38 | 114 |
| [GAS-12](#GAS-12) | Redundant state variable getters | 3 | - |
| [GAS-13](#GAS-13) | Remove or replace unused state variables | 1 | - |
| [GAS-14](#GAS-14) | `require()`/`revert()` strings longer than 32 bytes cost extra gas | 12 | 36 |
| [GAS-15](#GAS-15) | The result of a function call should be cached rather than re-calling the function | 4 | 400 |
| [GAS-16](#GAS-16) | Unlimited gas consumption risk due to external call recipients | 1 | - |
| [GAS-17](#GAS-17) | Unused named return variables without optimizer waste gas | 8 | 72 |
| [GAS-18](#GAS-18) | Use assembly to compute hashes to save gas | 12 | 960 |
| [GAS-19](#GAS-19) | Use assembly to emit events | 45 | 1710 |
| [GAS-20](#GAS-20) | Using a double `if` statement instead of a logical AND (`&&`) | 14 | 420 |
| [GAS-21](#GAS-21) | Use a more recent version of solidity | 9 | - |
| [GAS-22](#GAS-22) | Use `storage` instead of `memory` for structs/arrays | 4 | 16800 |
| [GAS-23](#GAS-23) | Use `unchecked` block for safe subtractions | 4 | 340 |
| [GAS-24](#GAS-24) | Using bitmap to store bool states can save gas | 2 | - |
| [GAS-25](#GAS-25) | `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants) | 1 | - |
| [GAS-26](#GAS-26) | Using bools for storage incurs overhead | 4 | - |
| [GAS-27](#GAS-27) | Cache array length outside of loop | 11 | - |
| [GAS-28](#GAS-28) | State variables should be cached in stack variables rather than re-reading them from storage | 16 | 1552 |
| [GAS-29](#GAS-29) | Use `calldata` instead of `memory` for function arguments that do not get mutated | 14 | - |
| [GAS-30](#GAS-30) | Use Custom Errors | 8 | 400 |
| [GAS-31](#GAS-31) | Don't use `SafeMath` once the solidity version is 0.8.0 or greater | 3 | - |
| [GAS-32](#GAS-32) | Don't initialize variables with default value | 10 | - |
| [GAS-33](#GAS-33) | Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead | 14 | 770 |
| [GAS-34](#GAS-34) | Constructors can be marked as `payable` to save deployment gas | 6 | 126 |
| [GAS-35](#GAS-35) | Functions guaranteed to revert when called by normal users can be marked `payable` | 22 | 462 |
| [GAS-36](#GAS-36) | `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too) | 12 | 60 |
| [GAS-37](#GAS-37) | Using `private` rather than `public` for constants, saves gas | 14 | - |
| [GAS-38](#GAS-38) | Use shift Right/Left instead of division/multiplication if possible | 13 | - |
| [GAS-39](#GAS-39) | Use `!= 0` instead of `> 0` for unsigned integer comparison | 19 | 76 |
| [GAS-40](#GAS-40) | Using assembly to check for zero can save gas | 56 | 336 |

## Medium Issues

<a name="M-1"></a> 
### [M-1] The remaining ETH may be locked in the contract after call
After calling an external contract and forwards some ETH value, the contract balance should be checked. If there is excess eth left over due to a failed call, or more eth being delivered than needed, or any other reason, this eth must be refunded to the user or handled appropriately, otherwise the eth may be frozen in the contract forever.

There are <b>2</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

344:     (bool success, bytes memory result) = _to.call{ value: _value }(_data);

```
[#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L344) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

98:       (bool success, ) = to.call{ value: amount, gas: gas }("");

```
[#L98](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L98) 

---

<a name="M-2"></a> 
### [M-2] Return values of `approve()` not checked
Not all IERC20 implementations `revert()` when there's a failure in `approve()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually approving anything

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

134:     IERC20WithBurn(_token).approve(_spender, _amount);

```
[#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L134) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

150:       IERC20WithBurn(_token).approve(_target, _amount);

169:     IERC20WithBurn(params._tokenA).approve(

173:     IERC20WithBurn(params._tokenB).approve(

```
[#L150](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L150) [#L169](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L169) [#L173](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L173) 

```solidity
File: contracts/core/RdpxV2Core.sol

339:     IERC20WithBurn(weth).approve(

343:     IERC20WithBurn(weth).approve(addresses.dopexAMMRouter, type(uint256).max);

344:     IERC20WithBurn(weth).approve(addresses.dpxEthCurvePool, type(uint256).max);

345:     IERC20WithBurn(weth).approve(

411:     IERC20WithBurn(_token).approve(_spender, _amount);

```
[#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L339) [#L343](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L343) [#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L344) [#L345](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L345) [#L411](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L411) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

245:       ? collateralToken.approve(

249:       : collateralToken.approve(addresses.perpetualAtlanticVaultLP, 0);

```
[#L245](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L245) [#L249](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L249) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

106:     collateral.approve(_perpetualAtlanticVault, type(uint256).max);

107:     ERC20(rdpx).approve(_perpetualAtlanticVault, type(uint256).max);

```
[#L106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L106) [#L107](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L107) 

</details>

---

<a name="M-3"></a> 
### [M-3] Return values of `transfer()`/`transferFrom()` not checked
Not all ERC20 implementations `revert()` when there's a failure in `transfer()` or `transferFrom()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually transfer anything.

There are <b>6</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

158:     IERC20WithBurn(params._tokenA).transferFrom(

163:     IERC20WithBurn(params._tokenB).transferFrom(

283:     IERC20WithBurn(_tokenA).transferFrom(

```
[#L158](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L158) [#L163](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L163) [#L283](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L283) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

128:     collateral.transferFrom(msg.sender, address(this), assets);

170:     collateral.transfer(receiver, assets);

```
[#L128](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L128) [#L170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L170) 

```solidity
File: contracts/reLP/ReLPContract.sol

243:     IERC20WithBurn(addresses.pair).transferFrom(

```
[#L243](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L243) 

---

<a name="M-4"></a> 
### [M-4] Unsafe use of ERC20 `transfer()`/`transferFrom()`/`approve()`
Some tokens do not implement the ERC20 standard properly. For example Tether (USDT)'s `transfer()` and `transferFrom()` functions do not return booleans as the ERC20 specification requires, and instead have no return value. When these sorts of tokens are cast to IERC20/ERC20, their function signatures do not match and therefore the calls made will revert.It is recommended to use the [`SafeERC20`](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/f347b410cf6aeeaaf5197e1fece139c793c03b2b/contracts/token/ERC20/utils/SafeERC20.sol#L19)'s `safeTransfer()` and `safeTransferFrom()` from OpenZeppelin instead.

There are <b>4</b> instances:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

106:     collateral.approve(_perpetualAtlanticVault, type(uint256).max);

107:     ERC20(rdpx).approve(_perpetualAtlanticVault, type(uint256).max);

128:     collateral.transferFrom(msg.sender, address(this), assets);

170:     collateral.transfer(receiver, assets);

```
[#L106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L106) [#L107](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L107) [#L128](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L128) [#L170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L170) 

---

<a name="M-5"></a> 
### [M-5] Centralization Risk for trusted owners
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
[#L5](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L5) [#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L22) [#L82](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L82) [#L111](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L111) [#L130](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L130) [#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L144) [#L195](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L195) [#L263](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L263) [#L308](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L308) 

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
[#L5](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L5) [#L28](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L28) [#L119](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L119) [#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L144) [#L157](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L157) [#L217](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L217) [#L281](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L281) [#L316](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L316) [#L327](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L327) [#L343](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L343) 

```solidity
File: contracts/core/RdpxV2Bond.sol

7: import { AccessControl } from "@openzeppelin/contracts/access/AccessControl.sol";

15:   AccessControl,

29:   function pause() public onlyRole(DEFAULT_ADMIN_ROLE) {

33:   function unpause() public onlyRole(DEFAULT_ADMIN_ROLE) {

39:   ) public onlyRole(MINTER_ROLE) returns (uint256 tokenId) {

```
[#L7](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L7) [#L15](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L15) [#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L33) [#L39](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L39) 

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
[#L5](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L5) [#L35](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L35) [#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L144) [#L152](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L152) [#L163](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L163) [#L182](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L182) [#L195](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L195) [#L206](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L206) [#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L218) [#L230](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L230) [#L243](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L243) [#L272](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L272) [#L315](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L315) [#L361](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L361) [#L378](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L378) [#L390](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L390) [#L407](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L407) [#L421](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L421) [#L432](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L432) [#L443](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L443) [#L457](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L457) [#L767](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L767) [#L791](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L791) [#L1054](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1054) [#L1085](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1085) 

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
[#L12](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L12) [#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L70) [#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L76) [#L95](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L95) [#L118](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L118) [#L142](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L142) [#L151](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L151) 

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
[#L7](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L7) [#L16](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L16) [#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L33) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L37) [#L43](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L43) [#L50](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L50) 

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
[#L13](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L13) [#L35](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L35) [#L136](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L136) [#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L144) [#L155](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L155) [#L166](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L166) [#L189](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L189) [#L221](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L221) [#L239](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L239) [#L243](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L243) [#L261](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L261) [#L320](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L320) [#L372](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L372) 

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
[#L5](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L5) [#L25](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L25) [#L92](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L92) [#L125](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L125) [#L173](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L173) [#L188](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L188) [#L202](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L202) 

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
[#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L134) [#L200](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L200) [#L204](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L204) [#L268](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L268) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L328) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

148:       TransferHelper.safeApprove(_token, _target, _amount);

150:       IERC20WithBurn(_token).approve(_target, _amount);

169:     IERC20WithBurn(params._tokenA).approve(

173:     IERC20WithBurn(params._tokenB).approve(

302:     TransferHelper.safeApprove(_tokenA, address(univ3_router), _amountAtoB);

```
[#L148](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L148) [#L150](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L150) [#L169](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L169) [#L173](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L173) [#L302](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L302) 

```solidity
File: contracts/core/RdpxV2Core.sol

339:     IERC20WithBurn(weth).approve(

343:     IERC20WithBurn(weth).approve(addresses.dopexAMMRouter, type(uint256).max);

344:     IERC20WithBurn(weth).approve(addresses.dpxEthCurvePool, type(uint256).max);

345:     IERC20WithBurn(weth).approve(

411:     IERC20WithBurn(_token).approve(_spender, _amount);

```
[#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L339) [#L343](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L343) [#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L344) [#L345](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L345) [#L411](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L411) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

207:     collateralToken.safeApprove(

245:       ? collateralToken.approve(

249:       : collateralToken.approve(addresses.perpetualAtlanticVaultLP, 0);

```
[#L207](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L207) [#L245](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L245) [#L249](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L249) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

106:     collateral.approve(_perpetualAtlanticVault, type(uint256).max);

107:     ERC20(rdpx).approve(_perpetualAtlanticVault, type(uint256).max);

```
[#L106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L106) [#L107](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L107) 

```solidity
File: contracts/reLP/ReLPContract.sol

150:     IERC20WithBurn(addresses.pair).safeApprove(

155:     IERC20WithBurn(addresses.tokenA).safeApprove(

160:     IERC20WithBurn(addresses.tokenB).safeApprove(

```
[#L150](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L150) [#L155](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L155) [#L160](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L160) 

</details>

---

<a name="L-2"></a> 
### [L-2] Array is `push()`ed but not `pop()`ed
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

There is <b>1</b> instance:
```solidity
File: contracts/core/RdpxV2Core.sol

961:     delegates.push(delegatePosition);

```
[#L961](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L961) 

---

<a name="L-3"></a> 
### [L-3] Check division by zero is prevented

<details>
<summary>
There are <b>52</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

373:     return (lpTokenBalance * getLpPrice()) / 1e8;

```
[#L373](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L373) 

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
[#L535](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L535) [#L539](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L539) [#L546](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L546) [#L547](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L547) [#L548](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L548) [#L549](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L549) [#L570](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L570) [#L574](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L574) [#L579](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L579) [#L605](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L605) [#L608](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L608) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L612) [#L658](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L658) [#L665](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L665) [#L669](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L669) [#L673](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L673) [#L1165](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1165) [#L1170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1170) [#L1172](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1172) [#L1176](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1176) [#L1176](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1176) [#L1181](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1181) [#L1185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1185) [#L1190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1190) 

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
[#L270](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L270) [#L276](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L276) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L335) [#L475](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L475) [#L481](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L481) [#L487](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L487) [#L512](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L512) [#L516](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L516) [#L521](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L521) [#L550](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L550) [#L559](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L559) [#L604](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L604) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L612) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

281:       ((_rdpxCollateral * rdpxPriceInAlphaToken) / 1e8);

```
[#L281](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L281) 

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
[#L230](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L230) [#L232](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L232) [#L235](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L235) [#L239](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L239) [#L251](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L251) [#L252](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L252) [#L254](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L254) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) [#L279](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L279) [#L290](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L290) 

</details>

---

<a name="L-4"></a> 
### [L-4] Constructor / initialization function lacks parameter validation
Constructors and initialization functions play a critical role in contracts by setting important initial states when the contract is first deployed before the system starts. The parameters passed to the constructor and initialization functions directly affect the behavior of the contract / protocol. If incorrect parameters are provided, the system may fail to run, behave abnormally, be unstable, or lack security. Therefore, it's crucial to carefully check each parameter in the constructor and initialization functions. If an exception is found, the transaction should be rolled back.

There are <b>5</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit `_rdpx` not validated
/// @audit `_rdpxV2Core` not validated
76:   constructor(address _rdpx, address _rdpxV2Core) {

```
[#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L76) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit `_weth` not validated
124:   constructor(address _weth) {

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L124) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

/// @audit `_name` not validated
/// @audit `_symbol` not validated
56:   constructor(
        string memory _name,
        string memory _symbol
      ) ERC721(_name, _symbol) {

```
[#L56](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L56) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit `_name` not validated
/// @audit `_symbol` not validated
/// @audit `_gensis` not validated
113:   constructor(
         string memory _name,
         string memory _symbol,
         address _collateralToken,
         uint256 _gensis
       ) ERC721(_name, _symbol) {
         _validate(_collateralToken != address(0), 1);

```
[#L113](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L113) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit `_rdpxRdpxV2Core` not validated
/// @audit `_collateral` not validated
/// @audit `_collateralSymbol` not validated
81:   constructor(
        address _perpetualAtlanticVault,
        address _rdpxRdpxV2Core,
        address _collateral,
        address _rdpx,
        string memory _collateralSymbol
      )
        ERC20(
          "PerpetualAtlanticVault LP Token",
          _collateralSymbol,
          ERC20(_collateral).decimals()
        )
      {

```
[#L81](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L81) 

---

<a name="L-5"></a> 
### [L-5] Enum values should be used instead of constant array indexes
Create a commented enum value to use instead of constant array indexes, this makes the code far easier to understand.

There are <b>6</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

332:     path[0] = token1;

333:     path[1] = token2;

```
[#L332](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L332) [#L333](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L333) 

```solidity
File: contracts/core/RdpxV2Core.sol

1094:       path[0] = reserveAsset[reservesIndex["RDPX"]].tokenAddress;

1095:       path[1] = weth;

```
[#L1094](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1094) [#L1095](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1095) 

```solidity
File: contracts/reLP/ReLPContract.sol

269:     path[0] = addresses.tokenB;

270:     path[1] = addresses.tokenA;

```
[#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L269) [#L270](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L270) 

---

<a name="L-6"></a> 
### [L-6] External call recipient can consume all remaining gas
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

There is <b>1</b> instance:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

344:     (bool success, bytes memory result) = _to.call{ value: _value }(_data);

```
[#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L344) 

---

<a name="L-7"></a> 
### [L-7] Governance functions should be controlled by time locks
Governance functions (such as upgrading contracts, setting critical parameters) should be controlled using time locks to introduce a delay between a proposal and its execution. This gives users time to exit before a potentially dangerous or malicious operation is applied.

There are <b>2</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

206:   function setIsreLP(bool _isReLPActive) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L206](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L206) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

243:   function setLpAllowance(bool increase) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L243](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L243) 

---

<a name="L-8"></a> 
### [L-8] Loss of precision in divisions
Division by large numbers may result in the result being zero, due to solidity not supporting fractions. Consider requiring a minimum amount for the numerator to ensure that it is always larger than the denominator.

<details>
<summary>
There are <b>52</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

373:     return (lpTokenBalance * getLpPrice()) / 1e8;

```
[#L373](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L373) 

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
[#L535](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L535) [#L539](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L539) [#L546](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L546) [#L547](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L547) [#L548](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L548) [#L549](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L549) [#L570](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L570) [#L574](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L574) [#L579](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L579) [#L605](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L605) [#L608](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L608) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L612) [#L658](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L658) [#L665](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L665) [#L669](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L669) [#L673](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L673) [#L1165](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1165) [#L1170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1170) [#L1172](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1172) [#L1176](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1176) [#L1176](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1176) [#L1181](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1181) [#L1185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1185) [#L1190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1190) 

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
[#L270](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L270) [#L276](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L276) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L335) [#L475](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L475) [#L481](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L481) [#L487](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L487) [#L512](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L512) [#L516](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L516) [#L521](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L521) [#L550](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L550) [#L559](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L559) [#L604](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L604) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L612) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

281:       ((_rdpxCollateral * rdpxPriceInAlphaToken) / 1e8);

```
[#L281](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L281) 

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
[#L230](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L230) [#L232](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L232) [#L235](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L235) [#L239](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L239) [#L251](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L251) [#L252](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L252) [#L254](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L254) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) [#L279](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L279) [#L290](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L290) 

</details>

---

<a name="L-9"></a> 
### [L-9] Missing contract existence checks before low-level calls
Low-level calls return success if there is no code present at the specified address. In addition to the zero-address checks, add a check to verify that `<address>.code.length > 0`

There are <b>2</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

344:     (bool success, bytes memory result) = _to.call{ value: _value }(_data);

```
[#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L344) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

98:       (bool success, ) = to.call{ value: amount, gas: gas }("");

```
[#L98](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L98) 

---

<a name="L-10"></a> 
### [L-10] Missing zero address check in constructor
Constructors often take address parameters to initialize important components of a contract, such as owner or linked contracts. However, without a checking, there's a risk that an address parameter could be mistakenly set to the zero address (0x0). This could be due to an error or oversight during contract deployment. A zero address in a crucial role can cause serious issues, as it cannot perform actions like a normal address, and any funds sent to it will be irretrievable. It's therefore crucial to include a zero address check in constructors to prevent such potential problems. If a zero address is detected, the constructor should revert the transaction.

There are <b>3</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit Missing zero check for `_rdpx`
/// @audit Missing zero check for `_rdpxV2Core`
76:   constructor(address _rdpx, address _rdpxV2Core) {

```
[#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L76) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit Missing zero check for `_weth`
124:   constructor(address _weth) {

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L124) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit Missing zero check for `_rdpxRdpxV2Core`
/// @audit Missing zero check for `_collateral`
81:   constructor(
        address _perpetualAtlanticVault,
        address _rdpxRdpxV2Core,
        address _collateral,
        address _rdpx,
        string memory _collateralSymbol
      )
        ERC20(
          "PerpetualAtlanticVault LP Token",
          _collateralSymbol,
          ERC20(_collateral).decimals()
        )
      {

```
[#L81](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L81) 

---

<a name="L-11"></a> 
### [L-11] Consider some checks for `address(0)` when setting address state variables

There are <b>4</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

77:     rdpx = _rdpx;

78:     rdpxV2Core = _rdpxV2Core;

```
[#L77](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L77) [#L78](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L78) 

```solidity
File: contracts/core/RdpxV2Core.sol

126:     weth = _weth;

```
[#L126](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L126) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

99:     rdpxRdpxV2Core = _rdpxRdpxV2Core;

```
[#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L99) 

---

<a name="L-12"></a> 
### [L-12] prevent re-setting a state variable with the same value
Not only is wasteful in terms of gas, but this is especially problematic when an event is emitted and the old and new values set are the same, as listeners might not expect this kind of scenario.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

116:     slippageTolerance = _slippageTolerance;

```
[#L116](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L116) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

77:     rdpx = _rdpx;

78:     rdpxV2Core = _rdpxV2Core;

```
[#L77](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L77) [#L78](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L78) 

```solidity
File: contracts/core/RdpxV2Core.sol

126:     weth = _weth;

184:     rdpxBurnPercentage = _rdpxBurnPercentage;

197:     rdpxFeePercentage = _rdpxFeePercentage;

207:     isReLPActive = _isReLPActive;

219:     putOptionsRequired = _putOptionsRequired;

232:     bondMaturity = _bondMaturity;

445:     bondDiscountFactor = _bondDiscountFactor;

459:     slippageTolerance = _slippageTolerance;

```
[#L126](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L126) [#L184](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L184) [#L197](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L197) [#L207](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L207) [#L219](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L219) [#L232](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L232) [#L445](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L445) [#L459](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L459) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

121:     collateralToken = IERC20WithBurn(_collateralToken);

240:     fundingDuration = _fundingDuration;

```
[#L121](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L121) [#L240](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L240) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

98:     perpetualAtlanticVault = IPerpetualAtlanticVault(_perpetualAtlanticVault);

99:     rdpxRdpxV2Core = _rdpxRdpxV2Core;

100:     collateralSymbol = _collateralSymbol;

101:     rdpx = _rdpx;

102:     collateral = ERC20(_collateral);

```
[#L98](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L98) [#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L99) [#L100](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L100) [#L101](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L101) [#L102](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L102) 

```solidity
File: contracts/reLP/ReLPContract.sol

97:     reLPFactor = _reLPFactor;

178:     liquiditySlippageTolerance = _liquiditySlippageTolerance;

193:     slippageTolerance = _slippageTolerance;

```
[#L97](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L97) [#L178](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L178) [#L193](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L193) 

</details>

---

<a name="L-13"></a> 
### [L-13] `SafeTransferLib` does not ensure that the token contract exists

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

172:     IERC20WithBurn(rdpx).safeTransfer(receiver, rdpxAmount);

```
[#L172](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L172) 

---

<a name="L-14"></a> 
### [L-14] Some tokens may revert when large transfers are made
Tokens such as COMP or UNI will revert when an address' balance reaches `type(uint96).max`. Ensure that the calls below can be broken up into smaller batches if necessary.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

170:     collateral.transfer(receiver, assets);

```
[#L170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L170) 

---

<a name="L-15"></a> 
### [L-15] Some tokens may revert when zero value transfers are made
Despite the fact that [EIP-20 states](https://github.com/ethereum/EIPs/blob/7500ac4fc1bbdfaf684e7ef851f798f6b667b2fe/EIPS/eip-20.md?plain=1#L116) that zero-value transfers must be accepted, some tokens, such as LEND, will revert if this is attempted, which may cause transactions that involve other tokens (such as batch operations) to fully revert. Consider skipping the transfer if the amount is zero, which will also save gas.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

170:     collateral.transfer(receiver, assets);

```
[#L170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L170) 

---

<a name="L-16"></a> 
### [L-16] Timestamp may be manipulation
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
[#L231](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L231) [#L279](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L279) [#L342](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L342) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

250:           block.timestamp

```
[#L250](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L250) 

```solidity
File: contracts/core/RdpxV2Core.sol

502:       maturity: block.timestamp + bondMaturity,

503:       timestamp: block.timestamp

636:       _validate(expiry >= block.timestamp, 2);

1023:     _validate(block.timestamp > bonds[id].maturity, 7);

1103:           block.timestamp + 10

1194:     ).nextFundingPaymentTimestamp() - block.timestamp;

```
[#L502](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L502) [#L503](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L503) [#L636](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L636) [#L1023](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1023) [#L1103](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1103) [#L1194](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1194) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

283:     uint256 timeToExpiry = nextFundingPaymentTimestamp() - block.timestamp;

463:     while (block.timestamp >= nextFundingPaymentTimestamp()) {

508:     lastUpdateTime = block.timestamp;

512:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

516:       (currentFundingRate * (block.timestamp - startTime)) / 1e18

521:       ((currentFundingRate * (block.timestamp - startTime)) / 1e18),

```
[#L283](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L283) [#L463](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L463) [#L508](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L508) [#L512](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L512) [#L516](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L516) [#L521](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L521) 

```solidity
File: contracts/reLP/ReLPContract.sol

264:       block.timestamp + 10

283:         block.timestamp + 10

294:       block.timestamp + 10

```
[#L264](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L264) [#L283](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L283) [#L294](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L294) 

</details>

---

<a name="L-17"></a> 
### [L-17] Tokens may be minted to `address(0)`

There are <b>3</b> instances:
```solidity
File: contracts/core/RdpxV2Bond.sol

37:   function mint(
        address to
      ) public onlyRole(MINTER_ROLE) returns (uint256 tokenId) {
        tokenId = _tokenIdCounter.current();
        _tokenIdCounter.increment();
        _mint(to, tokenId);
      }

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L37) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

114:   function mint(
         address to,
         uint256 expiry,
         uint256 rdpxAmount
       ) external onlyRole(MINTER_ROLE) {
         _whenNotPaused();
         require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter");
         uint256 bondId = _mintToken(to);
         bonds[bondId] = Bond(to, expiry, rdpxAmount);
     
         emit BondMinted(to, bondId, expiry, rdpxAmount);
       }

```
[#L114](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L114) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {
        _mint(to, amount);
      }

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L37) 

---

<a name="L-18"></a> 
### [L-18] Unsafe solidity low-level call can cause gas grief attack
Using the low-level calls of a solidity address can leave the contract open to gas grief attacks. These attacks occur when the called contract returns a large amount of data. So when calling an external contract, it is necessary to check the length of the return data before reading/copying it (using `returndatasize()`).

There are <b>2</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

344:     (bool success, bytes memory result) = _to.call{ value: _value }(_data);

```
[#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L344) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

98:       (bool success, ) = to.call{ value: amount, gas: gas }("");

```
[#L98](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L98) 

---

<a name="L-19"></a> 
### [L-19] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

There are <b>6</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

129:     ReserveAsset memory zeroAsset = ReserveAsset({
           tokenAddress: address(0),

253:     ReserveAsset memory asset = ReserveAsset({

841:         memory returnValues = BondWithDelegateReturnValue(0, 0, 0, 0);

955:     Delegate memory delegatePosition = Delegate({

```
[#L129](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L129) [#L253](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L253) [#L841](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L841) [#L955](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L955) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

286:     premium = calculatePremium(strike, amount, timeToExpiry, 0);

```
[#L286](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L286) 

```solidity
File: contracts/reLP/ReLPContract.sol

214:     TokenAInfo memory tokenAInfo = TokenAInfo(0, 0, 0);

```
[#L214](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L214) 

---

<a name="L-20"></a> 
### [L-20]  `abi.encodePacked()` should not be used with dynamic types when passing the result to a hash function such as `keccak256()`
Use `abi.encode()` instead which will pad items to 32 bytes, which will [prevent hash collisions](https://docs.soliditylang.org/en/v0.8.13/abi-spec.html#non-standard-packed-mode) (e.g. `abi.encodePacked(0x123,0x456)` => `0x123456` => `abi.encodePacked(0x1,0x23456)`, but `abi.encode(0x123,0x456)` => `0x0...1230...456`). "Unless there is a compelling reason, `abi.encode` should be preferred". If there is only one argument to `abi.encodePacked()` it can often be cast to `bytes()` or `bytes32()` [instead](https://ethereum.stackexchange.com/questions/30912/how-to-compare-strings-in-solidity#answer-82739).
If all arguments are strings and or bytes, `bytes.concat()` should be used instead

There are <b>3</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

106:       keccak256(abi.encodePacked(address(this), _tickLower, _tickUpper))

```
[#L106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L106) 

```solidity
File: contracts/core/RdpxV2Core.sol

1141:       keccak256(abi.encodePacked(asset.tokenSymbol)) ==

1142:         keccak256(abi.encodePacked(_token)),

```
[#L1141](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1141) [#L1142](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1142) 

---

<a name="L-21"></a> 
### [L-21] `decimals()` is not a part of the ERC-20 standard
The `decimals()` function is not a part of the ERC-20 standard, and was added later as an optional extension. As such, some valid ERC20 tokens do not support this interface, so it is unsafe to blindly cast all tokens to this interface, and then call this function.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

91:       ERC20(_collateral).decimals()

```
[#L91](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L91) 

---

<a name="L-22"></a> 
### [L-22] Do not use deprecated library functions

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
[#L58](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L58) [#L200](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L200) [#L204](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L204) [#L268](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L268) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L328) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

80:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

148:       TransferHelper.safeApprove(_token, _target, _amount);

302:     TransferHelper.safeApprove(_tokenA, address(univ3_router), _amountAtoB);

```
[#L80](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L80) [#L148](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L148) [#L302](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L302) 

```solidity
File: contracts/core/RdpxV2Bond.sol

25:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

26:     _setupRole(MINTER_ROLE, msg.sender);

```
[#L25](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L25) [#L26](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L26) 

```solidity
File: contracts/core/RdpxV2Core.sol

125:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

```
[#L125](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L125) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

61:     _setupRole(MINTER_ROLE, msg.sender);

62:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

```
[#L61](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L61) [#L62](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L62) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

126:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

127:     _setupRole(MANAGER_ROLE, msg.sender);

207:     collateralToken.safeApprove(

```
[#L126](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L126) [#L127](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L127) [#L207](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L207) 

```solidity
File: contracts/reLP/ReLPContract.sol

80:     _setupRole(DEFAULT_ADMIN_ROLE, msg.sender);

81:     _setupRole(RDPXV2CORE_ROLE, msg.sender);

150:     IERC20WithBurn(addresses.pair).safeApprove(

155:     IERC20WithBurn(addresses.tokenA).safeApprove(

160:     IERC20WithBurn(addresses.tokenB).safeApprove(

```
[#L80](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L80) [#L81](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L81) [#L150](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L150) [#L155](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L155) [#L160](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L160) 

</details>

---

<a name="L-23"></a> 
### [L-23] Empty Function Body - Consider commenting why

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

235:   ) internal virtual {}

```
[#L235](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L235) 

---

<a name="L-24"></a> 
### [L-24] `safeApprove()` is deprecated
[Deprecated](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/bfff03c0d2a59bcd8e2ead1da9aed9edf0080d05/contracts/token/ERC20/utils/SafeERC20.sol#L38-L45) in favor of `safeIncreaseAllowance()` and `safeDecreaseAllowance()`. If only setting the initial allowance to the value that means infinite, `safeIncreaseAllowance()` can be used instead. The function may currently work, but if a bug is found in this version of OpenZeppelin, and the version that you're forced to upgrade to no longer has this function, you'll encounter unnecessary delays in porting and testing replacement contracts.

There are <b>4</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

268:     IERC20WithBurn(addresses.pair).safeApprove(addresses.ammRouter, lpAmount);

328:     IERC20WithBurn(token1).safeApprove(addresses.ammRouter, token1Amount);

```
[#L268](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L268) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L328) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

148:       TransferHelper.safeApprove(_token, _target, _amount);

302:     TransferHelper.safeApprove(_tokenA, address(univ3_router), _amountAtoB);

```
[#L148](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L148) [#L302](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L302) 

---


## Non Critical Issues

<a name="NC-1"></a> 
### [NC-1] Add inline comments for unnamed variables
`function foo(address x, address)` -> `function foo(address x, address /* y */)`

There are <b>2</b> instances:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

231:   function _beforeTokenTransfer(
         address from,
         address,
         uint256
       ) internal virtual {}

286:   function beforeWithdraw(uint256 assets, uint256 /*shares*/) internal {

```
[#L231](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L231) [#L286](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L286) 

---

<a name="NC-2"></a> 
### [NC-2] Contract declarations should have NatSpec `@author` annotations

There are <b>2</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

22: abstract contract OracleLike {

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L22) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

21: contract PerpetualAtlanticVaultLP is ERC20, IPerpetualAtlanticVaultLP {

```
[#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L21) 

---

<a name="NC-3"></a> 
### [NC-3] Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, for readability
Well-organized data structures make code reviews easier, which may lead to fewer bugs. Consider combining related mappings into mappings to structs, so it's clear what data is related

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

69:   mapping(uint256 => mapping(uint256 => uint256))

```
[#L69](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L69) 

---

<a name="NC-4"></a> 
### [NC-4] Consider adding a block/deny-list
Doing so will significantly increase centralization, but will help to prevent hackers from using stolen tokens.

There are <b>10</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

22: contract UniV2LiquidityAMO is AccessControl {

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L22) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

22: abstract contract OracleLike {

28: contract UniV3LiquidityAMO is AccessControl, ERC721Holder {

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L22) [#L28](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L28) 

```solidity
File: contracts/core/RdpxV2Bond.sol

11: contract RdpxV2Bond is
      ERC721,
      ERC721Enumerable,
      Pausable,
      AccessControl,
      ERC721Burnable
    {

```
[#L11](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L11) 

```solidity
File: contracts/core/RdpxV2Core.sol

33: contract RdpxV2Core is
      IRdpxV2Core,
      AccessControl,
      ContractWhitelist,
      ERC721Holder,
      Pausable
    {

```
[#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L33) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

18: contract RdpxDecayingBonds is
      ERC721,
      ERC721Enumerable,
      ERC721Burnable,
      Pausable,
      AccessControl
    {

```
[#L18](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L18) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

12: contract DpxEthToken is
      ERC20,
      ERC20Burnable,
      Pausable,
      AccessControl,
      IDpxEthToken
    {

```
[#L12](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L12) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

28: contract PerpetualAtlanticVault is
      IPerpetualAtlanticVault,
      ReentrancyGuard,
      Pausable,
      ERC721,
      ERC721Enumerable,
      ERC721Burnable,
      AccessControl,
      ContractWhitelist
    {

```
[#L28](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L28) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

21: contract PerpetualAtlanticVaultLP is ERC20, IPerpetualAtlanticVaultLP {

```
[#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L21) 

```solidity
File: contracts/reLP/ReLPContract.sol

25: contract ReLPContract is AccessControl {

```
[#L25](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L25) 

---

<a name="NC-5"></a> 
### [NC-5] Consider adding formal verification proofs
Formal verification is the act of proving or disproving the correctness of intended algorithms underlying a system with respect to a certain formal specification/property/invariant, using formal methods of mathematics.

Some tools that are currently available to perform these tests on smart contracts are [SMTChecker](https://docs.soliditylang.org/en/latest/smtchecker.html) and [Certora Prover](https://www.certora.com/).

There is <b>1</b> instance:
```solidity

Global finding

```


---

<a name="NC-6"></a> 
### [NC-6] Consider bounding input array length
The functions below take in an unbounded array, and make function calls for entries in the array. While the function will revert if it eventually runs out of gas, it may be a nicer user experience to require() that the length of the array is below some reasonable maximum, so that the user doesn't have to use up a full transaction's gas only to see that the transaction reverts.

There are <b>7</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

/// @audit Consider length check for `tokens`
147:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L147](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L147) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit Consider length check for `tokens`
167:     for (uint256 i = 0; i < tokens.length; i++) {

/// @audit Consider length check for `optionIds`
775:     for (uint256 i = 0; i < optionIds.length; i++) {

```
[#L167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L167) [#L775](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L775) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

/// @audit Consider length check for `tokens`
103:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L103](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L103) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit Consider length check for `tokens`
225:     for (uint256 i = 0; i < tokens.length; i++) {

/// @audit Consider length check for `optionIds`
328:     for (uint256 i = 0; i < optionIds.length; i++) {

/// @audit Consider length check for `strikes`
413:     for (uint256 i = 0; i < strikes.length; i++) {

```
[#L225](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L225) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L328) [#L413](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L413) 

---

<a name="NC-7"></a> 
### [NC-7] Constants should be put on the left side of comparisons
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
[#L84](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L84) [#L85](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L85) [#L86](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L86) [#L87](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L87) [#L88](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L88) [#L89](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L89) [#L90](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L90) [#L131](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L131) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L132) 

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
[#L244](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L244) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L274) [#L316](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L316) [#L317](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L317) [#L318](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L318) [#L319](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L319) [#L320](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L320) [#L321](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L321) [#L322](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L322) [#L323](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L323) [#L324](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L324) [#L325](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L325) [#L362](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L362) [#L363](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L363) [#L379](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L379) [#L408](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L408) [#L409](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L409) [#L630](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L630) [#L1091](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1091) [#L1162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1162) 

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
[#L119](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L119) [#L190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L190) [#L191](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L191) [#L192](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L192) [#L193](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L193) [#L194](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L194) [#L195](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L195) [#L196](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L196) [#L467](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L467) [#L505](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L505) [#L578](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L578) [#L595](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L595) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

95:       _perpetualAtlanticVault != address(0) || _rdpx != address(0),

95:       _perpetualAtlanticVault != address(0) || _rdpx != address(0),

123:     require((shares = previewDeposit(assets)) != 0, "ZERO_SHARES");

162:     require(assets != 0, "ZERO_ASSETS");

223:       (supply == 0)

283:       supply == 0 ? assets : assets.mulDivDown(supply, totalVaultCollateral);

```
[#L95](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L95) [#L95](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L95) [#L123](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L123) [#L162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L162) [#L223](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L223) [#L283](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L283) 

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
[#L127](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L127) [#L128](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L128) [#L129](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L129) [#L130](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L130) [#L131](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L131) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L132) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L133) [#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L134) [#L135](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L135) 

</details>

---

<a name="NC-8"></a> 
### [NC-8] Contract uses both `require()`/`revert()` as well as custom errors
Consider using just one method in a single file.

There is <b>1</b> instance:
```solidity
File: contracts/core/RdpxV2Core.sol

33: contract RdpxV2Core is

```
[#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L33) 

---

<a name="NC-9"></a> 
### [NC-9] Contracts should have full test coverage
While 100% code coverage does not guarantee that there are no bugs, it often will catch easy-to-find bugs, and will ensure that there are fewer regressions when the code invariably has to be modified. Furthermore, in order to get full coverage, code authors will often have to re-organize their code so that it is more modular, so that each component can be tested separately, which reduces interdependencies between modules and layers, and makes for code that is easier to reason about and audit.

There is <b>1</b> instance:
```solidity

Global finding

```


---

<a name="NC-10"></a> 
### [NC-10] Convert simple `if` statements to ternary expressions
Converting some if statements to ternaries (such as `z = (a < b) ? x : y`) can make the code more concise and easier to read.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

597:       if (lastUpdateTime > nextFundingPaymentTimestamp() - fundingDuration) {
             startTime = lastUpdateTime;
           } else {
             startTime = nextFundingPaymentTimestamp() - fundingDuration;

```
[#L597](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L597) 

---

<a name="NC-11"></a> 
### [NC-11] Events that mark critical parameter changes should contain both the old and the new value
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
[#L152](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L152) [#L177](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L177) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

268:     emit log(positions_array.length);

269:     emit log(positions_mapping[pos.token_id].token_id);

321:     emit RecoveredERC20(tokenAddress, tokenAmount);

335:     emit RecoveredERC721(tokenAddress, token_id);

363:     emit LogAssetsTransfered(tokenABalance, tokenBBalance, tokenA, tokenB);

```
[#L268](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L268) [#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L269) [#L321](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L321) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L335) [#L363](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L363) 

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
[#L172](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L172) [#L185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L185) [#L198](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L198) [#L208](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L208) [#L220](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L220) [#L233](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L233) [#L263](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L263) [#L289](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L289) [#L349](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L349) [#L370](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L370) [#L447](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L447) [#L461](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L461) [#L782](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L782) [#L807](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L807) [#L932](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L932) [#L966](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L966) [#L989](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L989) [#L1007](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1007) [#L1041](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1041) [#L1069](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1069) [#L1123](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1123) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

124:     emit BondMinted(to, bondId, expiry, rdpxAmount);

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L124) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

211:     emit AddressesSet(addresses);

230:     emit EmergencyWithdraw(msg.sender, tokens);

311:     emit Purchase(strike, amount, premium, to, msg.sender);

368:     emit Settle(ethAmount, rdpxAmount, optionIds);

494:       emit FundingPaymentPointerUpdated(latestFundingPaymentPointer);

```
[#L211](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L211) [#L230](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L230) [#L311](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L311) [#L368](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L368) [#L494](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L494) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

134:     emit Deposit(msg.sender, receiver, assets, shares);

174:     emit Withdraw(msg.sender, receiver, owner, assets, shares);

```
[#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L134) [#L174](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L174) 

```solidity
File: contracts/reLP/ReLPContract.sol

99:     emit LogSetReLpFactor(_reLPFactor);

```
[#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L99) 

</details>

---

<a name="NC-12"></a> 
### [NC-12] Custom errors should be used rather than `revert()`/`require()`
Custom errors are available from solidity version 0.8.4. Custom errors are more easily processed in try-catch blocks, and are easier to re-use and maintain.

There are <b>8</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

131:     require(_token != address(0), "reLPContract: token cannot be 0");

132:     require(_spender != address(0), "reLPContract: spender cannot be 0");

133:     require(_amount > 0, "reLPContract: amount must be greater than 0");

```
[#L131](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L131) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L132) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L133) 

```solidity
File: contracts/core/RdpxV2Core.sol

244:     require(_asset != address(0), "RdpxV2Core: asset cannot be 0 address");

```
[#L244](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L244) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

99:       require(success, "RdpxReserve: transfer failed");

120:     require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter");

```
[#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L99) [#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L120) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

123:     require((shares = previewDeposit(assets)) != 0, "ZERO_SHARES");

162:     require(assets != 0, "ZERO_ASSETS");

```
[#L123](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L123) [#L162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L162) 

---

<a name="NC-13"></a> 
### [NC-13] `else` block not required
One level of nesting can be removed by not having an `else` block when the `if`-block always jumps at the end. For example:
```solidity
if (condition) {
	body1...
	return x;
} else {
	body2...
}
```
can be changed to:
```solidity
if (condition) {
	body1...
	return x;
}
body2...
```

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

578:     if (remainder == 0) {
           return _strike;
         } else {
           return _strike - remainder + roundingPrecision;

```
[#L578](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L578) 

---

<a name="NC-14"></a> 
### [NC-14] Empty bytes check is missing
Passing empty bytes to a function can cause unexpected behavior, such as certain operations failing, producing incorrect results, or wasting gas. It is recommended to check that all byte parameters are not empty.

There is <b>1</b> instance:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit Missing empty check for `_data`
339:   function execute(
         address _to,
         uint256 _value,
         bytes calldata _data
       ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (bool, bytes memory) {

```
[#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L339) 

---

<a name="NC-15"></a> 
### [NC-15] Enable IR-based code generation
The IR-based code generator was introduced with an aim to not only allow code generation to be more transparent and auditable but also to enable more powerful optimization passes that span across functions. You can enable it on the command line using `--via-ir` or with the option `{"viaIR": true}`. This will take longer to compile, but you can just simple test it before deploying and if you got a better benchmark then you can add --via-ir to your deploy command More on: https://docs.soliditylang.org/en/v0.8.17/ir-breaking-changes.html

There is <b>1</b> instance:
```solidity

Global finding

```


---

<a name="NC-16"></a> 
### [NC-16] Names of structs, events, enums and errors should use CapWords style
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html)

There is <b>1</b> instance:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

379:   event log(uint);

```
[#L379](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L379) 

---

<a name="NC-17"></a> 
### [NC-17] Events are emitted without the sender information
When an action is triggered based on a user's action, not being able to filter based on who triggered the action makes event processing a lot more cumbersome. Including the `msg.sender` the events of these types of action will make events much more useful to end users, especially when `msg.sender` is not `tx.origin`.

<details>
<summary>
There are <b>29</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

268:     emit log(positions_array.length);

269:     emit log(positions_mapping[pos.token_id].token_id);

321:     emit RecoveredERC20(tokenAddress, tokenAmount);

335:     emit RecoveredERC721(tokenAddress, token_id);

363:     emit LogAssetsTransfered(tokenABalance, tokenBBalance, tokenA, tokenB);

```
[#L268](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L268) [#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L269) [#L321](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L321) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L335) [#L363](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L363) 

```solidity
File: contracts/core/RdpxV2Core.sol

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

1041:     emit LogRedeem(to, receiptTokenAmount);

1069:     emit LogUpperDepeg(_amount, wethReceived);

1123:     emit LogLowerDepeg(_rdpxAmount, _wethAmount, dpxEthReceived);

```
[#L185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L185) [#L198](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L198) [#L208](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L208) [#L220](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L220) [#L233](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L233) [#L263](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L263) [#L289](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L289) [#L349](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L349) [#L370](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L370) [#L447](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L447) [#L461](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L461) [#L782](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L782) [#L807](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L807) [#L875](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L875) [#L932](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L932) [#L966](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L966) [#L989](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L989) [#L1041](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1041) [#L1069](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1069) [#L1123](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1123) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

124:     emit BondMinted(to, bondId, expiry, rdpxAmount);

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L124) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

211:     emit AddressesSet(addresses);

368:     emit Settle(ethAmount, rdpxAmount, optionIds);

```
[#L211](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L211) [#L368](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L368) 

```solidity
File: contracts/reLP/ReLPContract.sol

99:     emit LogSetReLpFactor(_reLPFactor);

```
[#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L99) 

</details>

---

<a name="NC-18"></a> 
### [NC-18] Import declarations should import specific identifiers, rather than the whole file
Using import declarations of the form `import {<identifier_name>} from "some/file.sol"` avoids polluting the symbol namespace making flattened files smaller, and speeds up compilation (but does not save any gas).

There are <b>6</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

12: import "../uniswap_V3/IUniswapV3Factory.sol";

13: import "../uniswap_V3/libraries/TickMath.sol";

14: import "../uniswap_V3/libraries/LiquidityAmounts.sol";

15: import "../uniswap_V3/periphery/interfaces/INonfungiblePositionManager.sol";

16: import "../uniswap_V3/IUniswapV3Pool.sol";

17: import "../uniswap_V3/ISwapRouter.sol";

```
[#L12](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L12) [#L13](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L13) [#L14](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L14) [#L15](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L15) [#L16](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L16) [#L17](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L17) 

---

<a name="NC-19"></a> 
### [NC-19] Invalid NatSpec comment style
NatSpec must begin with `///` or use `/* ... */` syntax

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

81:   // @dev Funding rate for the epoch

```
[#L81](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L81) 

---

<a name="NC-20"></a> 
### [NC-20] Large or complicated code bases should implement invariant tests
This includes: large code bases, or code with lots of inline-assembly, complicated math, or complicated interactions between multiple contracts. Invariant fuzzers such as Echidna require the test writer to come up with invariants which should not be violated under any circumstances, and the fuzzer tests various inputs and function calls to ensure that the invariants always hold. Even code with 100% code coverage can still have bugs due to the order of the operations a user performs, and invariant fuzzers may help significantly.

There is <b>1</b> instance:
```solidity

Global finding

```


---

<a name="NC-21"></a> 
### [NC-21] Long functions should be refactored into multiple, smaller, functions

<details>
<summary>
There are <b>11</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

/// @audit 61 lines
189:   function addLiquidity(
         uint256 tokenAAmount,
         uint256 tokenBAmount,
         uint256 tokenAAmountMin,
         uint256 tokenBAmountMin
       )
         external
         onlyRole(DEFAULT_ADMIN_ROLE)
         returns (uint256 tokenAUsed, uint256 tokenBUsed, uint256 lpReceived)
       {

/// @audit 51 lines
304:   function swap(
         uint256 token1Amount,
         uint256 token2AmountOutMin,
         bool swapTokenAForTokenB
       ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 token2Amount) {

```
[#L189](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L189) [#L304](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L304) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit 56 lines
155:   function addLiquidity(
         AddLiquidityParams memory params
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit 57 lines
213:   function removeLiquidity(
         uint256 positionIndex,
         uint256 minAmount0,
         uint256 minAmount1
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L155](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L155) [#L213](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L213) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit 61 lines
624:   function _transfer(
         uint256 _rdpxAmount,
         uint256 _wethAmount,
         uint256 _bondAmount,
         uint256 _bondId
       ) internal {

/// @audit 66 lines
819:   function bondWithDelegate(
         address _to,
         uint256[] memory _amounts,
         uint256[] memory _delegateIds,
         uint256 rdpxBondId
       ) public returns (uint256 receiptTokenAmount, uint256[] memory) {

/// @audit 66 lines
894:   function bond(
         uint256 _amount,
         uint256 rdpxBondId,
         address _to
       ) public returns (uint256 receiptTokenAmount) {

```
[#L624](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L624) [#L819](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L819) [#L894](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L894) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit 57 lines
255:   function purchase(
         uint256 amount,
         address to
       )
         external
         nonReentrant
         onlyRole(RDPXV2CORE_ROLE)
         returns (uint256 premium, uint256 tokenId)
       {
         _whenNotPaused();

/// @audit 54 lines
315:   function settle(
         uint256[] memory optionIds
       )
         external
         nonReentrant
         onlyRole(RDPXV2CORE_ROLE)
         returns (uint256 ethAmount, uint256 rdpxAmount)
       {
         _whenNotPaused();

/// @audit 54 lines
405:   function calculateFunding(
         uint256[] memory strikes
       ) external nonReentrant returns (uint256 fundingAmount) {
         _whenNotPaused();

```
[#L255](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L255) [#L315](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L315) [#L405](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L405) 

```solidity
File: contracts/reLP/ReLPContract.sol

/// @audit 105 lines
202:   function reLP(uint256 _amount) external onlyRole(RDPXV2CORE_ROLE) {

```
[#L202](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L202) 

</details>

---

<a name="NC-22"></a> 
### [NC-22] Magic numbers should be replaced with constants
Magic numbers are hard-coded values in code that can make it difficult for developers and maintainers to understand the code, and can also cause confusion or errors. To improve the readability and maintainability of code, it is recommended to replace magic numbers with constants that have good readability.

<details>
<summary>
There are <b>41</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

373:     return (lpTokenBalance * getLpPrice()) / 1e8;

```
[#L373](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L373) 

```solidity
File: contracts/core/RdpxV2Core.sol

546:       ? (((_amount * getDpxEthPrice()) / 1e8) -

547:         (((_amount * getDpxEthPrice()) * slippageTolerance) / 1e16))

548:       : (((_amount * getEthPrice()) / 1e8) -

549:         (((_amount * getEthPrice()) * slippageTolerance) / 1e16));

605:     uint256 rdpxRequiredInWeth = (_rdpxRequired * getRdpxPrice()) / 1e8;

612:     amount1 = (amount1 * (100e8 - _delegateFee)) / 1e10;

658:         (_rdpxAmount * rdpxBurnPercentage) / 1e10

665:           (_rdpxAmount * rdpxFeePercentage) / 1e10

669:       uint256 rdpxAmountInWeth = (_rdpxAmount * getRdpxPrice()) / 1e8;

673:       uint256 extraRdpxToWithdraw = (discountReceivedInWeth * 1e8) /

947:     _validate(_fee < 100e8, 8);

949:     _validate(_amount > 1e16, 4);

951:     _validate(_fee >= 1e8, 8);

1057:     _validate(getDpxEthPrice() > 1e8, 10);

1087:     _validate(getDpxEthPrice() < 1e8, 13);

1165:         1e2) / (Math.sqrt(1e18)); // 1e8 precision

1167:       _validate(bondDiscount < 100e8, 14);

1173:         (DEFAULT_PRECISION * rdpxPrice * 1e2);

1177:         (DEFAULT_PRECISION * 1e2);

1182:         (DEFAULT_PRECISION * rdpxPrice * 1e2);

1186:         (DEFAULT_PRECISION * 1e2);

```
[#L546](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L546) [#L547](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L547) [#L548](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L548) [#L549](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L549) [#L605](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L605) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L612) [#L658](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L658) [#L665](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L665) [#L669](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L669) [#L673](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L673) [#L947](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L947) [#L949](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L949) [#L951](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L951) [#L1057](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1057) [#L1087](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1087) [#L1165](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1165) [#L1167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1167) [#L1173](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1173) [#L1177](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1177) [#L1182](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1182) [#L1186](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1186) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

104:   uint256 public roundingPrecision = 1e6;

276:     uint256 requiredCollateral = (amount * strike) / 1e8;

335:       ethAmount += (amount * strike) / 1e8;

476:             1e18

482:               1e18

488:             1e18),

550:     ) * _amount) / 1e8);

559:     return strike > price ? ((strike - price) * amount) / 1e8 : 0;

604:         (amount * 1e18) /

612:         ((amount * 1e18) / (endTime - startTime));

```
[#L104](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L104) [#L276](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L276) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L335) [#L476](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L476) [#L482](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L482) [#L488](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L488) [#L550](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L550) [#L559](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L559) [#L604](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L604) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L612) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

281:       ((_rdpxCollateral * rdpxPriceInAlphaToken) / 1e8);

```
[#L281](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L281) 

```solidity
File: contracts/reLP/ReLPContract.sol

230:       1e2) / (Math.sqrt(1e18)); // 1e6 precision

232:     uint256 tokenAToRemove = ((((_amount * 4) * 1e18) /

235:       baseReLpRatio) / (1e18 * DEFAULT_PRECISION * 1e2);

251:       ((tokenAToRemove * liquiditySlippageTolerance) / 1e8);

253:       1e8) -

255:       1e16;

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

```
[#L230](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L230) [#L232](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L232) [#L235](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L235) [#L251](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L251) [#L253](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L253) [#L255](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L255) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) 

</details>

---

<a name="NC-23"></a> 
### [NC-23] Missing zero address check in functions with address parameters
Adding a zero address check for each address type parameter can prevent errors.

<details>
<summary>
There are <b>34</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit Missing zero check for `_rdpx`
/// @audit Missing zero check for `_rdpxV2Core`
76:   constructor(address _rdpx, address _rdpxV2Core) {

/// @audit Missing zero check for `_collateral_address`
94:   function liquidityInPool(
        address _collateral_address,
        int24 _tickLower,
        int24 _tickUpper,
        uint24 _fee
      ) public view returns (uint128) {

/// @audit Missing zero check for `_target`
/// @audit Missing zero check for `_token`
139:   function approveTarget(
         address _target,
         address _token,
         uint256 _amount,
         bool use_safe_approve
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing zero check for `_tokenA`
/// @audit Missing zero check for `_tokenB`
274:   function swap(
         address _tokenA,
         address _tokenB,
         uint24 _fee_tier,
         uint256 _amountAtoB,
         uint256 _amountOutMinimum,
         uint160 _sqrtPriceLimitX96
       ) public onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256) {

/// @audit Missing zero check for `tokenAddress`
313:   function recoverERC20(
         address tokenAddress,
         uint256 tokenAmount
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing zero check for `tokenAddress`
324:   function recoverERC721(
         address tokenAddress,
         uint256 token_id
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing zero check for `_to`
339:   function execute(
         address _to,
         uint256 _value,
         bytes calldata _data
       ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (bool, bytes memory) {

/// @audit Missing zero check for `tokenA`
/// @audit Missing zero check for `tokenB`
353:   function _sendTokensToRdpxV2Core(address tokenA, address tokenB) internal {

```
[#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L76) [#L94](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L94) [#L139](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L139) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L274) [#L313](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L313) [#L324](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L324) [#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L339) [#L353](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L353) 

```solidity
File: contracts/core/RdpxV2Bond.sol

/// @audit Missing zero check for `to`
37:   function mint(
        address to
      ) public onlyRole(MINTER_ROLE) returns (uint256 tokenId) {

/// @audit Missing zero check for `from`
/// @audit Missing zero check for `to`
45:   function _beforeTokenTransfer(
        address from,
        address to,
        uint256 tokenId,
        uint256 batchSize
      ) internal override(ERC721, ERC721Enumerable) {

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L37) [#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L45) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit Missing zero check for `_weth`
124:   constructor(address _weth) {

/// @audit Missing zero check for `_addr`
419:   function addToContractWhitelist(
         address _addr
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing zero check for `_addr`
430:   function removeFromContractWhitelist(
         address _addr
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing zero check for `_to`
495:   function _issueBond(
         address _to,
         uint256 _amount
       ) internal returns (uint256 bondId) {

/// @audit Missing zero check for `_to`
566:   function _stake(
         address _to,
         uint256 _amount
       ) internal returns (uint256 receiptTokenAmount) {

/// @audit Missing zero check for `_to`
819:   function bondWithDelegate(
         address _to,
         uint256[] memory _amounts,
         uint256[] memory _delegateIds,
         uint256 rdpxBondId
       ) public returns (uint256 receiptTokenAmount, uint256[] memory) {

/// @audit Missing zero check for `_to`
894:   function bond(
         uint256 _amount,
         uint256 rdpxBondId,
         address _to
       ) public returns (uint256 receiptTokenAmount) {

/// @audit Missing zero check for `to`
1016:   function redeem(
          uint256 id,
          address to
        ) external returns (uint256 receiptTokenAmount) {

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L124) [#L419](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L419) [#L430](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L430) [#L495](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L495) [#L566](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L566) [#L819](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L819) [#L894](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L894) [#L1016](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1016) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

/// @audit Missing zero check for `to`
89:   function emergencyWithdraw(
        address[] calldata tokens,
        bool transferNative,
        address payable to,
        uint256 amount,
        uint256 gas
      ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing zero check for `to`
114:   function mint(
         address to,
         uint256 expiry,
         uint256 rdpxAmount
       ) external onlyRole(MINTER_ROLE) {

/// @audit Missing zero check for `to`
129:   function _mintToken(address to) private returns (uint256 tokenId) {

/// @audit Missing zero check for `_address`
151:   function getBondsOwned(
         address _address
       ) external view returns (uint256[] memory) {

/// @audit Missing zero check for `from`
/// @audit Missing zero check for `to`
162:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256 tokenId,
         uint256 batchSize
       ) internal override(ERC721, ERC721Enumerable) {

```
[#L89](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L89) [#L114](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L114) [#L129](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L129) [#L151](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L151) [#L162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L162) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

/// @audit Missing zero check for `to`
37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {

/// @audit Missing zero check for `account`
47:   function burnFrom(
        address account,
        uint256 amount
      ) public override onlyRole(BURNER_ROLE) {

/// @audit Missing zero check for `from`
/// @audit Missing zero check for `to`
55:   function _beforeTokenTransfer(
        address from,
        address to,
        uint256 amount
      ) internal override {

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L37) [#L47](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L47) [#L55](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L55) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit Missing zero check for `_contract`
153:   function addToContractWhitelist(
         address _contract
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {
         _addToContractWhitelist(_contract);

/// @audit Missing zero check for `_contract`
164:   function removeFromContractWhitelist(
         address _contract
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {
         _removeFromContractWhitelist(_contract);

/// @audit Missing zero check for `to`
255:   function purchase(
         uint256 amount,
         address to
       )
         external
         nonReentrant
         onlyRole(RDPXV2CORE_ROLE)
         returns (uint256 premium, uint256 tokenId)
       {
         _whenNotPaused();

/// @audit Missing zero check for `from`
/// @audit Missing zero check for `to`
635:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256 tokenId,
         uint256 batchSize
       ) internal override(ERC721, ERC721Enumerable) {
         _whenNotPaused();

```
[#L153](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L153) [#L164](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L164) [#L255](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L255) [#L635](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L635) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit Missing zero check for `_perpetualAtlanticVault`
/// @audit Missing zero check for `_rdpxRdpxV2Core`
/// @audit Missing zero check for `_collateral`
/// @audit Missing zero check for `_rdpx`
81:   constructor(
        address _perpetualAtlanticVault,
        address _rdpxRdpxV2Core,
        address _collateral,
        address _rdpx,
        string memory _collateralSymbol
      )
        ERC20(
          "PerpetualAtlanticVault LP Token",
          _collateralSymbol,
          ERC20(_collateral).decimals()
        )
      {

/// @audit Missing zero check for `receiver`
118:   function deposit(
         uint256 assets,
         address receiver
       ) public virtual returns (uint256 shares) {

/// @audit Missing zero check for `receiver`
/// @audit Missing zero check for `owner`
145:   function redeem(
         uint256 shares,
         address receiver,
         address owner
       ) public returns (uint256 assets, uint256 rdpxAmount) {

/// @audit Missing zero check for `from`
/// @audit Missing zero check for ``
231:   function _beforeTokenTransfer(
         address from,
         address,
         uint256
       ) internal virtual {}

```
[#L81](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L81) [#L118](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L118) [#L145](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L145) [#L231](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L231) 

</details>

---

<a name="NC-24"></a> 
### [NC-24] Consider moving `msg.sender` checks to `modifier`s
If some functions are only allowed to be called by some specific users, consider using a modifier instead of checking with a require statement, especially if this check is done in multiple functions.

There is <b>1</b> instance:
```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

120:     require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter");

```
[#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L120) 

---

<a name="NC-25"></a> 
### [NC-25] Named mappings are recommended
[Named mappings](https://docs.soliditylang.org/en/v0.8.18/types.html#mapping-types) (with syntax `mapping(KeyType KeyName? => ValueType ValueName?)`) are recommended.It can make the mapping variables clearer, more readable and easier to maintain.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

66:   mapping(uint256 => Position) public positions_mapping;

```
[#L66](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L66) 

```solidity
File: contracts/core/RdpxV2Core.sol

73:   mapping(string => uint256) public reservesIndex;

76:   mapping(uint256 => Bond) public bonds;

79:   mapping(uint256 => bool) public optionsOwned;

82:   mapping(uint256 => bool) public fundingPaidFor;

```
[#L73](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L73) [#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L76) [#L79](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L79) [#L82](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L82) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

37:   mapping(uint256 => Bond) public bonds;

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L37) 

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
[#L63](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L63) [#L66](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L66) [#L69](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L69) [#L73](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L73) [#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L76) [#L79](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L79) [#L82](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L82) 

</details>

---

<a name="NC-26"></a> 
### [NC-26] NatSpec documentation for contract is missing
e.g. `@dev` or `@notice`, and it must appear above the contract definition braces in order to be identified by the compiler as NatSpec.

There are <b>2</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

22: abstract contract OracleLike {

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L22) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

21: contract PerpetualAtlanticVaultLP is ERC20, IPerpetualAtlanticVaultLP {

```
[#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L21) 

---

<a name="NC-27"></a> 
### [NC-27] Event declarations should have NatSpec descriptions

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

387:   event LogAddLiquidity(

398:   event LogRemoveLiquidity(

407:   event LogSwap(

415:   event LogAssetsTransfered(

421:   event LogEmergencyWithdraw(address sender, address[] tokens);

```
[#L387](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L387) [#L398](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L398) [#L407](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L407) [#L415](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L415) [#L421](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L421) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

368:   event RecoveredERC20(address token, uint256 amount);

369:   event RecoveredERC721(address token, uint256 id);

370:   event LogAssetsTransfered(

379:   event log(uint);

```
[#L368](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L368) [#L369](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L369) [#L370](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L370) [#L379](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L379) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

46:   event BondMinted(

53:   event EmergencyWithdraw(address sender);

```
[#L46](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L46) [#L53](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L53) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

28:   event Deposit(

35:   event Withdraw(

```
[#L28](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L28) [#L35](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L35) 

```solidity
File: contracts/reLP/ReLPContract.sol

311:   event LogSetReLpFactor(uint256 _reLPFactor);

```
[#L311](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L311) 

</details>

---

<a name="NC-28"></a> 
### [NC-28] NatSpec documentation for function is missing
It is recommended that Solidity contracts are fully annotated using NatSpec for all public interfaces (everything in the ABI). It is clearly stated in the Solidity official documentation. In complex projects such as DeFi, the interpretation of all functions and their arguments and returns is important for code readability and auditability.

<details>
<summary>
There are <b>39</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

57:   constructor() {

```
[#L57](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L57) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

23:   function read() external view virtual returns (uint);

25:   function uniswapPool() external view virtual returns (address);

76:   constructor(address _rdpx, address _rdpxV2Core) {

94:   function liquidityInPool(
        address _collateral_address,
        int24 _tickLower,
        int24 _tickUpper,
        uint24 _fee
      ) public view returns (uint128) {

112:   function numPositions() public view returns (uint256) {

119:   function collectFees() external onlyRole(DEFAULT_ADMIN_ROLE) {

139:   function approveTarget(
         address _target,
         address _token,
         uint256 _amount,
         bool use_safe_approve
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

155:   function addLiquidity(
         AddLiquidityParams memory params
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

213:   function removeLiquidity(
         uint256 positionIndex,
         uint256 minAmount0,
         uint256 minAmount1
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

274:   function swap(
         address _tokenA,
         address _tokenB,
         uint24 _fee_tier,
         uint256 _amountAtoB,
         uint256 _amountOutMinimum,
         uint160 _sqrtPriceLimitX96
       ) public onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256) {

313:   function recoverERC20(
         address tokenAddress,
         uint256 tokenAmount
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

324:   function recoverERC721(
         address tokenAddress,
         uint256 token_id
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

339:   function execute(
         address _to,
         uint256 _value,
         bytes calldata _data
       ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (bool, bytes memory) {

```
[#L23](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L23) [#L25](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L25) [#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L76) [#L94](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L94) [#L112](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L112) [#L119](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L119) [#L139](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L139) [#L155](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L155) [#L213](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L213) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L274) [#L313](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L313) [#L324](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L324) [#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L339) 

```solidity
File: contracts/core/RdpxV2Bond.sol

24:   constructor() ERC721("rDPX V2 Bond", "rDPXV2Bond") {

29:   function pause() public onlyRole(DEFAULT_ADMIN_ROLE) {

33:   function unpause() public onlyRole(DEFAULT_ADMIN_ROLE) {

37:   function mint(
        address to
      ) public onlyRole(MINTER_ROLE) returns (uint256 tokenId) {

45:   function _beforeTokenTransfer(
        address from,
        address to,
        uint256 tokenId,
        uint256 batchSize
      ) internal override(ERC721, ERC721Enumerable) {

57:   function supportsInterface(
        bytes4 interfaceId
      )
        public
        view
        override(ERC721, ERC721Enumerable, AccessControl)
        returns (bool)
      {

```
[#L24](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L24) [#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L33) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L37) [#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L45) [#L57](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L57) 

```solidity
File: contracts/core/RdpxV2Core.sol

124:   constructor(address _weth) {

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L124) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

56:   constructor(
        string memory _name,
        string memory _symbol
      ) ERC721(_name, _symbol) {

162:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256 tokenId,
         uint256 batchSize
       ) internal override(ERC721, ERC721Enumerable) {

174:   function supportsInterface(
         bytes4 interfaceId
       )
         public
         view
         override(ERC721, ERC721Enumerable, AccessControl)
         returns (bool)
       {

```
[#L56](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L56) [#L162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L162) [#L174](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L174) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

23:   constructor() ERC20("Dopex Synthetic ETH", "dpxETH") {

29:   function pause() public onlyRole(PAUSER_ROLE) {

33:   function unpause() public onlyRole(PAUSER_ROLE) {

37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {

41:   function burn(
        uint256 _amount
      ) public override(ERC20Burnable, IDpxEthToken) onlyRole(BURNER_ROLE) {

47:   function burnFrom(
        address account,
        uint256 amount
      ) public override onlyRole(BURNER_ROLE) {

55:   function _beforeTokenTransfer(
        address from,
        address to,
        uint256 amount
      ) internal override {

```
[#L23](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L23) [#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L33) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L37) [#L41](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L41) [#L47](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L47) [#L55](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L55) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

243:   function setLpAllowance(bool increase) external onlyRole(DEFAULT_ADMIN_ROLE) {
         increase

594:   function _updateFundingRate(uint256 amount) private {
         if (fundingRates[latestFundingPaymentPointer] == 0) {

635:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256 tokenId,
         uint256 batchSize
       ) internal override(ERC721, ERC721Enumerable) {
         _whenNotPaused();

645:   function supportsInterface(
         bytes4 interfaceId
       )
         public
         view
         override(ERC721, ERC721Enumerable, AccessControl)
         returns (bool)
       {
         return super.supportsInterface(interfaceId);

```
[#L243](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L243) [#L594](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L594) [#L635](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L635) [#L645](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L645) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

218:   function _convertToAssets(
         uint256 shares
       ) internal view virtual returns (uint256 assets, uint256 rdpxAmount) {

231:   function _beforeTokenTransfer(
         address from,
         address,
         uint256
       ) internal virtual {}

286:   function beforeWithdraw(uint256 assets, uint256 /*shares*/) internal {

```
[#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L218) [#L231](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L231) [#L286](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L286) 

```solidity
File: contracts/reLP/ReLPContract.sol

79:   constructor() {

```
[#L79](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L79) 

</details>

---

<a name="NC-29"></a> 
### [NC-29] Modifier declarations should have NatSpec descriptions

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

295:   modifier onlyPerpVault() {

```
[#L295](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L295) 

---

<a name="NC-30"></a> 
### [NC-30] Missing NatSpec `@param`
Some functions have an incomplete NatSpec: add a `@param` notation to describe the function parameters to improve the code documentation.

<details>
<summary>
There are <b>89</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

/// @audit Missing @param for _tokenA
/// @audit Missing @param for _tokenB
74:   function setAddresses(
        address _tokenA,
        address _tokenB,
        address _pair,
        address _rdpxV2Core,
        address _rdpxOracle,
        address _ammFactory,
        address _ammRouter
      ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _slippageTolerance
109:   function setSlippageTolerance(
         uint256 _slippageTolerance
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _token
/// @audit Missing @param for _spender
/// @audit Missing @param for _amount
126:   function approveContractToSpend(
         address _token,
         address _spender,
         uint256 _amount
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for tokens
142:   function emergencyWithdraw(
         address[] calldata tokens
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L74](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L74) [#L109](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L109) [#L126](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L126) [#L142](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L142) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit Missing @param for _rdpx
/// @audit Missing @param for _rdpxV2Core
76:   constructor(address _rdpx, address _rdpxV2Core) {

/// @audit Missing @param for _collateral_address
/// @audit Missing @param for _tickLower
/// @audit Missing @param for _tickUpper
/// @audit Missing @param for _fee
94:   function liquidityInPool(
        address _collateral_address,
        int24 _tickLower,
        int24 _tickUpper,
        uint24 _fee
      ) public view returns (uint128) {

/// @audit Missing @param for _target
/// @audit Missing @param for _token
/// @audit Missing @param for _amount
/// @audit Missing @param for use_safe_approve
139:   function approveTarget(
         address _target,
         address _token,
         uint256 _amount,
         bool use_safe_approve
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for params
155:   function addLiquidity(
         AddLiquidityParams memory params
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for positionIndex
/// @audit Missing @param for minAmount0
/// @audit Missing @param for minAmount1
213:   function removeLiquidity(
         uint256 positionIndex,
         uint256 minAmount0,
         uint256 minAmount1
       ) public onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _tokenA
/// @audit Missing @param for _tokenB
/// @audit Missing @param for _fee_tier
/// @audit Missing @param for _amountAtoB
/// @audit Missing @param for _amountOutMinimum
/// @audit Missing @param for _sqrtPriceLimitX96
274:   function swap(
         address _tokenA,
         address _tokenB,
         uint24 _fee_tier,
         uint256 _amountAtoB,
         uint256 _amountOutMinimum,
         uint160 _sqrtPriceLimitX96
       ) public onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256) {

/// @audit Missing @param for tokenAddress
/// @audit Missing @param for tokenAmount
313:   function recoverERC20(
         address tokenAddress,
         uint256 tokenAmount
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for tokenAddress
/// @audit Missing @param for token_id
324:   function recoverERC721(
         address tokenAddress,
         uint256 token_id
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _to
/// @audit Missing @param for _value
/// @audit Missing @param for _data
339:   function execute(
         address _to,
         uint256 _value,
         bytes calldata _data
       ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (bool, bytes memory) {

/// @audit Missing @param for tokenA
/// @audit Missing @param for tokenB
353:   function _sendTokensToRdpxV2Core(address tokenA, address tokenB) internal {

```
[#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L76) [#L94](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L94) [#L139](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L139) [#L155](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L155) [#L213](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L213) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L274) [#L313](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L313) [#L324](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L324) [#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L339) [#L353](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L353) 

```solidity
File: contracts/core/RdpxV2Bond.sol

/// @audit Missing @param for to
37:   function mint(
        address to
      ) public onlyRole(MINTER_ROLE) returns (uint256 tokenId) {

/// @audit Missing @param for from
/// @audit Missing @param for to
/// @audit Missing @param for tokenId
/// @audit Missing @param for batchSize
45:   function _beforeTokenTransfer(
        address from,
        address to,
        uint256 tokenId,
        uint256 batchSize
      ) internal override(ERC721, ERC721Enumerable) {

/// @audit Missing @param for interfaceId
57:   function supportsInterface(
        bytes4 interfaceId
      )
        public
        view
        override(ERC721, ERC721Enumerable, AccessControl)
        returns (bool)
      {

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L37) [#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L45) [#L57](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L57) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit Missing @param for _weth
124:   constructor(address _weth) {

/// @audit Missing @param for tokens
161:   function emergencyWithdraw(
         address[] calldata tokens
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _rdpxBurnPercentage
180:   function setRdpxBurnPercentage(
         uint256 _rdpxBurnPercentage
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _rdpxFeePercentage
193:   function setRdpxFeePercentage(
         uint256 _rdpxFeePercentage
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _isReLPActive
206:   function setIsreLP(bool _isReLPActive) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _putOptionsRequired
216:   function setPutOptionsRequired(
         bool _putOptionsRequired
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _bondMaturity
228:   function setBondMaturity(
         uint256 _bondMaturity
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _asset
/// @audit Missing @param for _assetSymbol
240:   function addAssetTotokenReserves(
         address _asset,
         string memory _assetSymbol
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _assetSymbol
270:   function removeAssetFromtokenReserves(
         string memory _assetSymbol
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _dopexAMMRouter
/// @audit Missing @param for _dpxEthCurvePool
/// @audit Missing @param for _rdpxDecayingBonds
/// @audit Missing @param for _perpetualAtlanticVault
/// @audit Missing @param for _perpetualAtlanticVaultLP
/// @audit Missing @param for _rdpxReserve
/// @audit Missing @param for _rdpxV2ReceiptToken
/// @audit Missing @param for _feeDistributor
/// @audit Missing @param for _reLPContract
/// @audit Missing @param for _receiptTokenBonds
304:   function setAddresses(
         address _dopexAMMRouter,
         address _dpxEthCurvePool,
         address _rdpxDecayingBonds,
         address _perpetualAtlanticVault,
         address _perpetualAtlanticVaultLP,
         address _rdpxReserve,
         address _rdpxV2ReceiptToken,
         address _feeDistributor,
         address _reLPContract,
         address _receiptTokenBonds
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _rdpxPriceOracle
/// @audit Missing @param for _dpxEthPriceOracle
358:   function setPricingOracleAddresses(
         address _rdpxPriceOracle,
         address _dpxEthPriceOracle
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _addr
378:   function addAMOAddress(address _addr) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _index
388:   function removeAMOAddress(
         uint256 _index
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _token
/// @audit Missing @param for _spender
/// @audit Missing @param for _amount
403:   function approveContractToSpend(
         address _token,
         address _spender,
         uint256 _amount
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _addr
419:   function addToContractWhitelist(
         address _addr
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _addr
430:   function removeFromContractWhitelist(
         address _addr
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _bondDiscountFactor
441:   function setBondDiscount(
         uint256 _bondDiscountFactor
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _slippageTolerance
455:   function setSlippageTolerance(
         uint256 _slippageTolerance
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _to
/// @audit Missing @param for _amount
495:   function _issueBond(
         address _to,
         uint256 _amount
       ) internal returns (uint256 bondId) {

/// @audit Missing @param for _to
/// @audit Missing @param for _amount
566:   function _stake(
         address _to,
         uint256 _amount
       ) internal returns (uint256 receiptTokenAmount) {

/// @audit Missing @param for _wethRequired
/// @audit Missing @param for _rdpxRequired
/// @audit Missing @param for _amount
/// @audit Missing @param for _delegateFee
598:   function _calculateAmounts(
         uint256 _wethRequired,
         uint256 _rdpxRequired,
         uint256 _amount,
         uint256 _delegateFee
       ) internal view returns (uint256 amount1, uint256 amount2) {

/// @audit Missing @param for _rdpxAmount
/// @audit Missing @param for _wethAmount
/// @audit Missing @param for _bondAmount
/// @audit Missing @param for _bondId
624:   function _transfer(
         uint256 _rdpxAmount,
         uint256 _wethAmount,
         uint256 _bondAmount,
         uint256 _bondId
       ) internal {

/// @audit Missing @param for _amount
/// @audit Missing @param for rdpxBondId
/// @audit Missing @param for delegateId
699:   function _bondWithDelegate(
         uint256 _amount,
         uint256 rdpxBondId,
         uint256 delegateId
       ) internal returns (BondWithDelegateReturnValue memory returnValues) {

/// @audit Missing @param for _clause
/// @audit Missing @param for _errorCode
751:   function _validate(bool _clause, uint256 _errorCode) internal pure {

/// @audit Missing @param for optionIds
764:   function settle(
         uint256[] memory optionIds
       )
         external
         onlyRole(DEFAULT_ADMIN_ROLE)
         returns (uint256 amountOfWeth, uint256 rdpxAmount)
       {

/// @audit Missing @param for _to
/// @audit Missing @param for _amounts
/// @audit Missing @param for _delegateIds
/// @audit Missing @param for rdpxBondId
819:   function bondWithDelegate(
         address _to,
         uint256[] memory _amounts,
         uint256[] memory _delegateIds,
         uint256 rdpxBondId
       ) public returns (uint256 receiptTokenAmount, uint256[] memory) {

/// @audit Missing @param for _amount
/// @audit Missing @param for rdpxBondId
/// @audit Missing @param for _to
894:   function bond(
         uint256 _amount,
         uint256 rdpxBondId,
         address _to
       ) public returns (uint256 receiptTokenAmount) {

/// @audit Missing @param for _amount
/// @audit Missing @param for _fee
941:   function addToDelegate(
         uint256 _amount,
         uint256 _fee
       ) external returns (uint256) {

/// @audit Missing @param for delegateId
975:   function withdraw(
         uint256 delegateId
       ) external returns (uint256 amountWithdrawn) {

/// @audit Missing @param for id
/// @audit Missing @param for to
1016:   function redeem(
          uint256 id,
          address to
        ) external returns (uint256 receiptTokenAmount) {

/// @audit Missing @param for _amount
1051:   function upperDepeg(
          uint256 _amount,
          uint256 minOut
        ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 wethReceived) {

/// @audit Missing @param for _rdpxAmount
/// @audit Missing @param for _wethAmount
/// @audit Missing @param for minOut
1080:   function lowerDepeg(
          uint256 _rdpxAmount,
          uint256 _wethAmount,
          uint256 minamountOfWeth,
          uint256 minOut
        ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 dpxEthReceived) {

/// @audit Missing @param for _amount
1156:   function calculateBondCost(
          uint256 _amount,
          uint256 _rdpxBondId
        ) public view returns (uint256 rdpxRequired, uint256 wethRequired) {

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L124) [#L161](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L161) [#L180](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L180) [#L193](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L193) [#L206](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L206) [#L216](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L216) [#L228](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L228) [#L240](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L240) [#L270](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L270) [#L304](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L304) [#L358](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L358) [#L378](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L378) [#L388](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L388) [#L403](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L403) [#L419](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L419) [#L430](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L430) [#L441](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L441) [#L455](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L455) [#L495](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L495) [#L566](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L566) [#L598](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L598) [#L624](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L624) [#L699](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L699) [#L751](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L751) [#L764](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L764) [#L819](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L819) [#L894](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L894) [#L941](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L941) [#L975](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L975) [#L1016](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1016) [#L1051](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1051) [#L1080](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1080) [#L1156](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1156) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

/// @audit Missing @param for _name
/// @audit Missing @param for _symbol
56:   constructor(
        string memory _name,
        string memory _symbol
      ) ERC721(_name, _symbol) {

/// @audit Missing @param for tokens
/// @audit Missing @param for transferNative
/// @audit Missing @param for to
/// @audit Missing @param for amount
/// @audit Missing @param for gas
89:   function emergencyWithdraw(
        address[] calldata tokens,
        bool transferNative,
        address payable to,
        uint256 amount,
        uint256 gas
      ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for from
/// @audit Missing @param for to
/// @audit Missing @param for tokenId
/// @audit Missing @param for batchSize
162:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256 tokenId,
         uint256 batchSize
       ) internal override(ERC721, ERC721Enumerable) {

/// @audit Missing @param for interfaceId
174:   function supportsInterface(
         bytes4 interfaceId
       )
         public
         view
         override(ERC721, ERC721Enumerable, AccessControl)
         returns (bool)
       {

```
[#L56](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L56) [#L89](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L89) [#L162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L162) [#L174](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L174) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

/// @audit Missing @param for to
/// @audit Missing @param for amount
37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {

/// @audit Missing @param for _amount
41:   function burn(
        uint256 _amount
      ) public override(ERC20Burnable, IDpxEthToken) onlyRole(BURNER_ROLE) {

/// @audit Missing @param for account
/// @audit Missing @param for amount
47:   function burnFrom(
        address account,
        uint256 amount
      ) public override onlyRole(BURNER_ROLE) {

/// @audit Missing @param for from
/// @audit Missing @param for to
/// @audit Missing @param for amount
55:   function _beforeTokenTransfer(
        address from,
        address to,
        uint256 amount
      ) internal override {

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L37) [#L41](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L41) [#L47](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L47) [#L55](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L55) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit Missing @param for _contract
153:   function addToContractWhitelist(
         address _contract
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {
         _addToContractWhitelist(_contract);

/// @audit Missing @param for _contract
164:   function removeFromContractWhitelist(
         address _contract
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {
         _removeFromContractWhitelist(_contract);

/// @audit Missing @param for _optionPricing
/// @audit Missing @param for _assetPriceOracle
/// @audit Missing @param for _volatilityOracle
/// @audit Missing @param for _feeDistributor
/// @audit Missing @param for _rdpx
/// @audit Missing @param for _perpetualAtlanticVaultLP
/// @audit Missing @param for _rdpxV2Core
181:   function setAddresses(
         address _optionPricing,
         address _assetPriceOracle,
         address _volatilityOracle,
         address _feeDistributor,
         address _rdpx,
         address _perpetualAtlanticVaultLP,
         address _rdpxV2Core
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {
         _validate(_optionPricing != address(0), 1);

/// @audit Missing @param for tokens
219:   function emergencyWithdraw(
         address[] calldata tokens
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {
         _whenPaused();

/// @audit Missing @param for _fundingDuration
237:   function updateFundingDuration(
         uint256 _fundingDuration
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {
         fundingDuration = _fundingDuration;

/// @audit Missing @param for increase
243:   function setLpAllowance(bool increase) external onlyRole(DEFAULT_ADMIN_ROLE) {
         increase

/// @audit Missing @param for amount
/// @audit Missing @param for to
255:   function purchase(
         uint256 amount,
         address to
       )
         external
         nonReentrant
         onlyRole(RDPXV2CORE_ROLE)
         returns (uint256 premium, uint256 tokenId)
       {
         _whenNotPaused();

/// @audit Missing @param for optionIds
315:   function settle(
         uint256[] memory optionIds
       )
         external
         nonReentrant
         onlyRole(RDPXV2CORE_ROLE)
         returns (uint256 ethAmount, uint256 rdpxAmount)
       {
         _whenNotPaused();

/// @audit Missing @param for strikes
405:   function calculateFunding(
         uint256[] memory strikes
       ) external nonReentrant returns (uint256 fundingAmount) {
         _whenNotPaused();

/// @audit Missing @param for _strike
534:   function getVolatility(uint256 _strike) public view returns (uint256) {
         return IVolatilityOracle(addresses.volatilityOracle).getVolatility(_strike);

/// @audit Missing @param for _strike
/// @audit Missing @param for _amount
/// @audit Missing @param for timeToExpiry
/// @audit Missing @param for _price
539:   function calculatePremium(
         uint256 _strike,
         uint256 _amount,
         uint256 timeToExpiry,
         uint256 _price
       ) public view returns (uint256 premium) {
         premium = ((IOptionPricing(addresses.optionPricing).getOptionPrice(

/// @audit Missing @param for price
/// @audit Missing @param for strike
/// @audit Missing @param for amount
554:   function calculatePnl(
         uint256 price,
         uint256 strike,
         uint256 amount
       ) public pure returns (uint256) {
         return strike > price ? ((strike - price) * amount) / 1e8 : 0;

/// @audit Missing @param for amount
594:   function _updateFundingRate(uint256 amount) private {
         if (fundingRates[latestFundingPaymentPointer] == 0) {

/// @audit Missing @param for _clause
/// @audit Missing @param for _errorCode
621:   function _validate(bool _clause, uint256 _errorCode) private pure {
         if (!_clause) revert PerpetualAtlanticVaultError(_errorCode);

/// @audit Missing @param for from
/// @audit Missing @param for to
/// @audit Missing @param for tokenId
/// @audit Missing @param for batchSize
635:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256 tokenId,
         uint256 batchSize
       ) internal override(ERC721, ERC721Enumerable) {
         _whenNotPaused();

/// @audit Missing @param for interfaceId
645:   function supportsInterface(
         bytes4 interfaceId
       )
         public
         view
         override(ERC721, ERC721Enumerable, AccessControl)
         returns (bool)
       {
         return super.supportsInterface(interfaceId);

```
[#L153](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L153) [#L164](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L164) [#L181](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L181) [#L219](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L219) [#L237](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L237) [#L243](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L243) [#L255](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L255) [#L315](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L315) [#L405](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L405) [#L534](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L534) [#L539](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L539) [#L554](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L554) [#L594](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L594) [#L621](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L621) [#L635](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L635) [#L645](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L645) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit Missing @param for amount
180:   function lockCollateral(uint256 amount) public onlyPerpVault {

/// @audit Missing @param for amount
185:   function unlockLiquidity(uint256 amount) public onlyPerpVault {

/// @audit Missing @param for proceeds
190:   function addProceeds(uint256 proceeds) public onlyPerpVault {

/// @audit Missing @param for loss
199:   function subtractLoss(uint256 loss) public onlyPerpVault {

/// @audit Missing @param for amount
208:   function addRdpx(uint256 amount) public onlyPerpVault {

/// @audit Missing @param for shares
218:   function _convertToAssets(
         uint256 shares
       ) internal view virtual returns (uint256 assets, uint256 rdpxAmount) {

/// @audit Missing @param for from
231:   function _beforeTokenTransfer(
         address from,
         address,
         uint256
       ) internal virtual {}

/// @audit Missing @param for shares
262:   function redeemPreview(
         uint256 shares
       ) public view returns (uint256, uint256) {

/// @audit Missing @param for assets
269:   function previewDeposit(uint256 assets) public view returns (uint256) {

/// @audit Missing @param for assets
274:   function convertToShares(
         uint256 assets
       ) public view returns (uint256 shares) {

/// @audit Missing @param for assets
286:   function beforeWithdraw(uint256 assets, uint256 /*shares*/) internal {

```
[#L180](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L180) [#L185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L185) [#L190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L190) [#L199](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L199) [#L208](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L208) [#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L218) [#L231](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L231) [#L262](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L262) [#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L269) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L274) [#L286](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L286) 

```solidity
File: contracts/reLP/ReLPContract.sol

/// @audit Missing @param for _reLPFactor
90:   function setreLpFactor(
        uint256 _reLPFactor
      ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _tokenB
115:   function setAddresses(
         address _tokenA,
         address _tokenB,
         address _pair,
         address _rdpxV2Core,
         address _tokenAReserve,
         address _amo,
         address _rdpxOracle,
         address _ammFactory,
         address _ammRouter
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _liquiditySlippageTolerance
171:   function setLiquiditySlippageTolerance(
         uint256 _liquiditySlippageTolerance
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Missing @param for _slippageTolerance
186:   function setSlippageTolerance(
         uint256 _slippageTolerance
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L90](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L90) [#L115](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L115) [#L171](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L171) [#L186](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L186) 

</details>

---

<a name="NC-31"></a> 
### [NC-31] Public variable declarations should have NatSpec descriptions

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

35:   IUniswapV3Factory public univ3_factory;

36:   INonfungiblePositionManager public univ3_positions;

37:   ISwapRouter public univ3_router;

63:   Position[] public positions_array;

66:   mapping(uint256 => Position) public positions_mapping;

69:   address public rdpx;

72:   address public rdpxV2Core;

```
[#L35](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L35) [#L36](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L36) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L37) [#L63](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L63) [#L66](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L66) [#L69](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L69) [#L72](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L72) 

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L22) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

37:   mapping(uint256 => Bond) public bonds;

```
[#L31](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L31) [#L34](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L34) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L37) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L19](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L19) [#L20](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L20) [#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

82:   mapping(uint256 => uint256) public fundingRates;

```
[#L82](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L82) 

</details>

---

<a name="NC-32"></a> 
### [NC-32] NatSpec `@return` is missing
It is recommended that Solidity contracts are fully annotated using NatSpec

<details>
<summary>
There are <b>34</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

189:   function addLiquidity(
         uint256 tokenAAmount,
         uint256 tokenBAmount,
         uint256 tokenAAmountMin,
         uint256 tokenBAmountMin
       )
         external
         onlyRole(DEFAULT_ADMIN_ROLE)
         returns (uint256 tokenAUsed, uint256 tokenBUsed, uint256 lpReceived)
       {

258:   function removeLiquidity(
         uint256 lpAmount,
         uint256 tokenAAmountMin,
         uint256 tokenBAmountMin
       )
         external
         onlyRole(DEFAULT_ADMIN_ROLE)
         returns (uint256 tokenAReceived, uint256 tokenBReceived)
       {

304:   function swap(
         uint256 token1Amount,
         uint256 token2AmountOutMin,
         bool swapTokenAForTokenB
       ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 token2Amount) {

```
[#L189](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L189) [#L258](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L258) [#L304](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L304) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

23:   function read() external view virtual returns (uint);

25:   function uniswapPool() external view virtual returns (address);

94:   function liquidityInPool(
        address _collateral_address,
        int24 _tickLower,
        int24 _tickUpper,
        uint24 _fee
      ) public view returns (uint128) {

112:   function numPositions() public view returns (uint256) {

274:   function swap(
         address _tokenA,
         address _tokenB,
         uint24 _fee_tier,
         uint256 _amountAtoB,
         uint256 _amountOutMinimum,
         uint160 _sqrtPriceLimitX96
       ) public onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256) {

339:   function execute(
         address _to,
         uint256 _value,
         bytes calldata _data
       ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (bool, bytes memory) {

```
[#L23](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L23) [#L25](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L25) [#L94](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L94) [#L112](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L112) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L274) [#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L339) 

```solidity
File: contracts/core/RdpxV2Bond.sol

37:   function mint(
        address to
      ) public onlyRole(MINTER_ROLE) returns (uint256 tokenId) {

57:   function supportsInterface(
        bytes4 interfaceId
      )
        public
        view
        override(ERC721, ERC721Enumerable, AccessControl)
        returns (bool)
      {

```
[#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L37) [#L57](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L57) 

```solidity
File: contracts/core/RdpxV2Core.sol

1051:   function upperDepeg(
          uint256 _amount,
          uint256 minOut
        ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 wethReceived) {

1080:   function lowerDepeg(
          uint256 _rdpxAmount,
          uint256 _wethAmount,
          uint256 minamountOfWeth,
          uint256 minOut
        ) external onlyRole(DEFAULT_ADMIN_ROLE) returns (uint256 dpxEthReceived) {

```
[#L1051](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1051) [#L1080](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1080) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

129:   function _mintToken(address to) private returns (uint256 tokenId) {

151:   function getBondsOwned(
         address _address
       ) external view returns (uint256[] memory) {

174:   function supportsInterface(
         bytes4 interfaceId
       )
         public
         view
         override(ERC721, ERC721Enumerable, AccessControl)
         returns (bool)
       {

```
[#L129](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L129) [#L151](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L151) [#L174](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L174) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

255:   function purchase(
         uint256 amount,
         address to
       )
         external
         nonReentrant
         onlyRole(RDPXV2CORE_ROLE)
         returns (uint256 premium, uint256 tokenId)
       {
         _whenNotPaused();

315:   function settle(
         uint256[] memory optionIds
       )
         external
         nonReentrant
         onlyRole(RDPXV2CORE_ROLE)
         returns (uint256 ethAmount, uint256 rdpxAmount)
       {
         _whenNotPaused();

372:   function payFunding() external onlyRole(RDPXV2CORE_ROLE) returns (uint256) {
         _whenNotPaused();

529:   function getUnderlyingPrice() public view returns (uint256) {
         return IRdpxEthOracle(addresses.assetPriceOracle).getRdpxPriceInEth();

534:   function getVolatility(uint256 _strike) public view returns (uint256) {
         return IVolatilityOracle(addresses.volatilityOracle).getVolatility(_strike);

539:   function calculatePremium(
         uint256 _strike,
         uint256 _amount,
         uint256 timeToExpiry,
         uint256 _price
       ) public view returns (uint256 premium) {
         premium = ((IOptionPricing(addresses.optionPricing).getOptionPrice(

554:   function calculatePnl(
         uint256 price,
         uint256 strike,
         uint256 amount
       ) public pure returns (uint256) {
         return strike > price ? ((strike - price) * amount) / 1e8 : 0;

563:   function nextFundingPaymentTimestamp()
         public
         view
         returns (uint256 timestamp)
       {
         return genesis + (latestFundingPaymentPointer * fundingDuration);

588:   function _mintOptionToken() private returns (uint256 tokenId) {
         tokenId = _tokenIdCounter.current();

645:   function supportsInterface(
         bytes4 interfaceId
       )
         public
         view
         override(ERC721, ERC721Enumerable, AccessControl)
         returns (bool)
       {
         return super.supportsInterface(interfaceId);

```
[#L255](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L255) [#L315](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L315) [#L372](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L372) [#L529](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L529) [#L534](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L534) [#L539](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L539) [#L554](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L554) [#L563](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L563) [#L588](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L588) [#L645](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L645) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

218:   function _convertToAssets(
         uint256 shares
       ) internal view virtual returns (uint256 assets, uint256 rdpxAmount) {

240:   function activeCollateral() public view returns (uint256) {

245:   function totalCollateral() public view returns (uint256) {

250:   function rdpxCollateral() public view returns (uint256) {

255:   function totalAvailableCollateral() public view returns (uint256) {

262:   function redeemPreview(
         uint256 shares
       ) public view returns (uint256, uint256) {

269:   function previewDeposit(uint256 assets) public view returns (uint256) {

274:   function convertToShares(
         uint256 assets
       ) public view returns (uint256 shares) {

```
[#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L218) [#L240](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L240) [#L245](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L245) [#L250](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L250) [#L255](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L255) [#L262](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L262) [#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L269) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L274) 

</details>

---

<a name="NC-33"></a> 
### [NC-33] There is no need to initialize variables with 0
Since the variables are automatically set to 0 when created, it is redundant to initialize it with 0 again.

There are <b>10</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L147](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L147) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```
[#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L120) 

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

```
[#L167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L167) [#L775](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L775) [#L836](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L836) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L103](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L103) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

89:   uint256 public latestFundingPaymentPointer = 0;

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```
[#L89](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L89) [#L225](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L225) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L328) [#L413](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L413) 

---

<a name="NC-34"></a> 
### [NC-34] Put all system-wide constants in one file
Putting all the system-wide constants in a single file improves code readability, makes it easier to understand the basic configuration and limitations of the system, and makes maintenance easier.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

48:   uint256 public constant DEFAULT_PRECISION = 1e8;

```
[#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L48) 

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L22) 

```solidity
File: contracts/core/RdpxV2Core.sol

85:   uint256 public constant DEFAULT_PRECISION = 1e8;

88:   uint256 public constant RDPX_RATIO_PERCENTAGE = 25 * DEFAULT_PRECISION;

91:   uint256 public constant ETH_RATIO_PERCENTAGE = 75 * DEFAULT_PRECISION;

```
[#L85](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L85) [#L88](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L88) [#L91](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L91) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L31](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L31) [#L34](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L34) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L19](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L19) [#L20](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L20) [#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L45) [#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L48) 

```solidity
File: contracts/reLP/ReLPContract.sol

67:   uint256 public constant DEFAULT_PRECISION = 1e8;

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L67](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L67) [#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L70) 

</details>

---

<a name="NC-35"></a> 
### [NC-35] Contract declarations should have NatSpec `@title` annotations
Some contract definitions have an incomplete NatSpec: add a `@title` notation to describe the contract to improve the code documentation.

There is <b>1</b> instance:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

22: abstract contract OracleLike {

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L22) 

---

<a name="NC-36"></a> 
### [NC-36] Unused named return
Declaring named returns, but not using them, is confusing to the reader. Consider either completely removing them (by declaring just the type without a name), or remove the return statement and do a variable assignment. This would improve the readability of the code, and it may also help reduce regressions during future code refactors.

There are <b>8</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit `` not used
819:   function bondWithDelegate(
         address _to,
         uint256[] memory _amounts,
         uint256[] memory _delegateIds,
         uint256 rdpxBondId
       ) public returns (uint256 receiptTokenAmount, uint256[] memory) {

/// @audit `dpxEthPrice` not used
1216:   function getDpxEthPrice() public view returns (uint256 dpxEthPrice) {

/// @audit `ethPrice` not used
1227:   function getEthPrice() public view returns (uint256 ethPrice) {

/// @audit `delegate` not used
1260:   function getDelegatePosition(
          uint256 _delegateId
        )
          public
          view
          returns (
            address delegate,
            uint256 amount,
            uint256 fee,
            uint256 activeCollateral
          )
        {

```
[#L819](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L819) [#L1216](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1216) [#L1227](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1227) [#L1260](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1260) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit `timestamp` not used
563:   function nextFundingPaymentTimestamp()
         public
         view
         returns (uint256 timestamp)
       {
         return genesis + (latestFundingPaymentPointer * fundingDuration);

/// @audit `strike` not used
576:   function roundUp(uint256 _strike) public view returns (uint256 strike) {
         uint256 remainder = _strike % roundingPrecision;

```
[#L563](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L563) [#L576](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L576) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit `assets` not used
/// @audit `rdpxAmount` not used
218:   function _convertToAssets(
         uint256 shares
       ) internal view virtual returns (uint256 assets, uint256 rdpxAmount) {

/// @audit `shares` not used
274:   function convertToShares(
         uint256 assets
       ) public view returns (uint256 shares) {

```
[#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L218) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L274) 

---

<a name="NC-37"></a> 
### [NC-37] Unused contract variables
The following state variables are defined but not used. It is recommended to check the code for logical omissions that cause them not to be used. If it's determined that they are not needed anywhere, it's best to remove them from the codebase to improve code clarity and minimize confusion.

There is <b>1</b> instance:
```solidity
File: contracts/dpxETH/DpxEthToken.sol

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

---

<a name="NC-38"></a> 
### [NC-38] Consider using `delete` rather than assigning zero to clear values
The `delete` keyword more closely matches the semantics of what is being done, and draws more attention to the changing of state, which may lead to a more thorough audit of its associated logic.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

343:       optionPositions[optionIds[i]].strike = 0;

```
[#L343](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L343) 

---

<a name="NC-39"></a> 
### [NC-39] Expressions for constant values should use `immutable` rather than `constant`
While it doesn't save any gas because the compiler knows that developers often make this mistake, it's still best to use the right tool for the task at hand. There is a difference between `constant` variables and `immutable` variables, and they should each be used in their appropriate contexts. `constants` should be used for literal values written into the code, and `immutable` variables should be used for expressions, or values calculated in, or passed into the constructor.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

48:   uint256 public constant DEFAULT_PRECISION = 1e8;

```
[#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L48) 

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L22) 

```solidity
File: contracts/core/RdpxV2Core.sol

85:   uint256 public constant DEFAULT_PRECISION = 1e8;

88:   uint256 public constant RDPX_RATIO_PERCENTAGE = 25 * DEFAULT_PRECISION;

91:   uint256 public constant ETH_RATIO_PERCENTAGE = 75 * DEFAULT_PRECISION;

```
[#L85](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L85) [#L88](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L88) [#L91](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L91) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L31](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L31) [#L34](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L34) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L19](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L19) [#L20](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L20) [#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L45) [#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L48) 

```solidity
File: contracts/reLP/ReLPContract.sol

67:   uint256 public constant DEFAULT_PRECISION = 1e8;

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L67](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L67) [#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L70) 

</details>

---

<a name="NC-40"></a> 
### [NC-40] Use the latest solidity version for deployment
Upgrading to a newer Solidity release can optimize gas usage, take advantage of new features and improve overall contract efficiency. Where possible, based on compatibility requirements, it is recommended to use newer/latest solidity version to take advantage of the latest optimizations and features.

There are <b>9</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L2) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L2) 

```solidity
File: contracts/core/RdpxV2Bond.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L2) 

```solidity
File: contracts/core/RdpxV2Core.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L2) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L2) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L2) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L2) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L2) 

```solidity
File: contracts/reLP/ReLPContract.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L2) 

---

<a name="NC-41"></a> 
### [NC-41] Use of `override` is unnecessary
Starting with Solidity version [0.8.8](https://docs.soliditylang.org/en/v0.8.20/contracts.html#function-overriding), using the `override` keyword when the function solely overrides an interface function, and the function doesn't exist in multiple base contracts, is unnecessary.

There are <b>2</b> instances:
```solidity
File: contracts/dpxETH/DpxEthToken.sol

50:   ) public override onlyRole(BURNER_ROLE) {

59:   ) internal override {

```
[#L50](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L50) [#L59](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L59) 

---

<a name="NC-42"></a> 
### [NC-42] Visibility of state variables is not explicitly defined
To avoid misunderstandings and unexpected state accesses, it is recommended to explicitly define the visibility of each state variable.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

69:   mapping(uint256 => mapping(uint256 => uint256))

```
[#L69](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L69) 

---

<a name="NC-43"></a> 
### [NC-43] Whitespace in Expressions
See the [Whitespace in Expressions](https://docs.soliditylang.org/en/latest/style-guide.html#whitespace-in-expressions) section of the Solidity Style Guide.

There are <b>3</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

105:     (uint128 liquidity, , , , ) = get_pool.positions(

193:     (uint256 tokenId, uint128 amountLiquidity, , ) = univ3_positions.mint(

```
[#L105](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L105) [#L193](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L193) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

98:       (bool success, ) = to.call{ value: amount, gas: gas }("");

```
[#L98](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L98) 

---

<a name="NC-44"></a> 
### [NC-44] Missing checks for `address(0)` when assigning values to address state variables

There are <b>4</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

77:     rdpx = _rdpx;

78:     rdpxV2Core = _rdpxV2Core;

```
[#L77](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L77) [#L78](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L78) 

```solidity
File: contracts/core/RdpxV2Core.sol

126:     weth = _weth;

```
[#L126](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L126) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

99:     rdpxRdpxV2Core = _rdpxRdpxV2Core;

```
[#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L99) 

---

<a name="NC-45"></a> 
### [NC-45] Common functions should be refactored to a common base contract
The functions below have the same implementation as is seen in other files. The functions should be refactored into functions of a common base contract.

There are <b>8</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

/// @audit Seen in contracts/reLP/ReLPContract.sol
109:   function setSlippageTolerance(
         uint256 _slippageTolerance
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L109](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L109) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit Seen in contracts/decaying-bonds/RdpxDecayingBonds.sol
144:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Seen in contracts/decaying-bonds/RdpxDecayingBonds.sol
152:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L144) [#L152](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L152) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

/// @audit Seen in contracts/core/RdpxV2Core.sol
70:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

/// @audit Seen in contracts/core/RdpxV2Core.sol
76:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L70) [#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L76) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit Seen in contracts/core/RdpxV2Core.sol
136:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {
         _pause();

/// @audit Seen in contracts/core/RdpxV2Core.sol
144:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {
         _unpause();

```
[#L136](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L136) [#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L144) 

```solidity
File: contracts/reLP/ReLPContract.sol

/// @audit Seen in contracts/amo/UniV2LiquidityAmo.sol
186:   function setSlippageTolerance(
         uint256 _slippageTolerance
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L186](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L186) 

---

<a name="NC-46"></a> 
### [NC-46] Names of `private`/`internal` functions should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

286:   function beforeWithdraw(uint256 assets, uint256 /*shares*/) internal {

```
[#L286](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L286) 

---

<a name="NC-47"></a> 
### [NC-47] Return values of `approve()` not checked
Not all IERC20 implementations `revert()` when there's a failure in `approve()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually approving anything

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

134:     IERC20WithBurn(_token).approve(_spender, _amount);

```
[#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L134) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

150:       IERC20WithBurn(_token).approve(_target, _amount);

169:     IERC20WithBurn(params._tokenA).approve(

173:     IERC20WithBurn(params._tokenB).approve(

```
[#L150](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L150) [#L169](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L169) [#L173](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L173) 

```solidity
File: contracts/core/RdpxV2Core.sol

339:     IERC20WithBurn(weth).approve(

343:     IERC20WithBurn(weth).approve(addresses.dopexAMMRouter, type(uint256).max);

344:     IERC20WithBurn(weth).approve(addresses.dpxEthCurvePool, type(uint256).max);

345:     IERC20WithBurn(weth).approve(

411:     IERC20WithBurn(_token).approve(_spender, _amount);

```
[#L339](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L339) [#L343](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L343) [#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L344) [#L345](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L345) [#L411](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L411) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

245:       ? collateralToken.approve(

249:       : collateralToken.approve(addresses.perpetualAtlanticVaultLP, 0);

```
[#L245](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L245) [#L249](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L249) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

106:     collateral.approve(_perpetualAtlanticVault, type(uint256).max);

107:     ERC20(rdpx).approve(_perpetualAtlanticVault, type(uint256).max);

```
[#L106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L106) [#L107](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L107) 

</details>

---

<a name="NC-48"></a> 
### [NC-48] Variables should be named in mixedCase style
As the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html#naming-styles) suggests: arguments, local variables and mutable state variables should be named in mixedCase style.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

48:   uint256 public constant DEFAULT_PRECISION = 1e8;

```
[#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L48) 

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L22) 

```solidity
File: contracts/core/RdpxV2Core.sol

85:   uint256 public constant DEFAULT_PRECISION = 1e8;

88:   uint256 public constant RDPX_RATIO_PERCENTAGE = 25 * DEFAULT_PRECISION;

91:   uint256 public constant ETH_RATIO_PERCENTAGE = 75 * DEFAULT_PRECISION;

```
[#L85](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L85) [#L88](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L88) [#L91](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L91) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L31](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L31) [#L34](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L34) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L19](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L19) [#L20](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L20) [#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L45) [#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L48) 

```solidity
File: contracts/reLP/ReLPContract.sol

67:   uint256 public constant DEFAULT_PRECISION = 1e8;

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L67](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L67) [#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L70) 

</details>

---

<a name="NC-49"></a> 
### [NC-49] Event is missing `indexed` fields
Index event fields make the field more quickly accessible to off-chain tools that parse events. However, note that each index field costs extra gas during emission, so it's not necessarily best to index the maximum allowed per event (three fields). Each event should use three indexed fields if there are three or more fields, and gas usage is not particularly of concern for the events in question. If there are fewer than three fields, all of the fields should be indexed.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

387:   event LogAddLiquidity(

398:   event LogRemoveLiquidity(

407:   event LogSwap(

415:   event LogAssetsTransfered(

421:   event LogEmergencyWithdraw(address sender, address[] tokens);

```
[#L387](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L387) [#L398](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L398) [#L407](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L407) [#L415](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L415) [#L421](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L421) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

368:   event RecoveredERC20(address token, uint256 amount);

369:   event RecoveredERC721(address token, uint256 id);

370:   event LogAssetsTransfered(

379:   event log(uint);

```
[#L368](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L368) [#L369](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L369) [#L370](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L370) [#L379](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L379) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

46:   event BondMinted(

53:   event EmergencyWithdraw(address sender);

```
[#L46](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L46) [#L53](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L53) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

28:   event Deposit(

```
[#L28](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L28) 

```solidity
File: contracts/reLP/ReLPContract.sol

311:   event LogSetReLpFactor(uint256 _reLPFactor);

```
[#L311](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L311) 

</details>

---

<a name="NC-50"></a> 
### [NC-50] Functions not used internally could be marked `external`

<details>
<summary>
There are <b>32</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

94:   function liquidityInPool(

112:   function numPositions() public view returns (uint256) {

139:   function approveTarget(

155:   function addLiquidity(

213:   function removeLiquidity(

274:   function swap(

```
[#L94](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L94) [#L112](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L112) [#L139](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L139) [#L155](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L155) [#L213](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L213) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L274) 

```solidity
File: contracts/core/RdpxV2Bond.sol

29:   function pause() public onlyRole(DEFAULT_ADMIN_ROLE) {

33:   function unpause() public onlyRole(DEFAULT_ADMIN_ROLE) {

37:   function mint(

57:   function supportsInterface(

```
[#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L33) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L37) [#L57](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L57) 

```solidity
File: contracts/core/RdpxV2Core.sol

819:   function bondWithDelegate(

894:   function bond(

1135:   function getReserveTokenInfo(

1206:   function getLpPrice() public view returns (uint256) {

1260:   function getDelegatePosition(

```
[#L819](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L819) [#L894](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L894) [#L1135](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1135) [#L1206](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1206) [#L1260](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1260) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

139:   function decreaseAmount(

174:   function supportsInterface(

```
[#L139](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L139) [#L174](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L174) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

29:   function pause() public onlyRole(PAUSER_ROLE) {

33:   function unpause() public onlyRole(PAUSER_ROLE) {

37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {

41:   function burn(

47:   function burnFrom(

```
[#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L33) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L37) [#L41](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L41) [#L47](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L47) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

554:   function calculatePnl(

645:   function supportsInterface(

```
[#L554](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L554) [#L645](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L645) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

145:   function redeem(

180:   function lockCollateral(uint256 amount) public onlyPerpVault {

185:   function unlockLiquidity(uint256 amount) public onlyPerpVault {

190:   function addProceeds(uint256 proceeds) public onlyPerpVault {

199:   function subtractLoss(uint256 loss) public onlyPerpVault {

208:   function addRdpx(uint256 amount) public onlyPerpVault {

240:   function activeCollateral() public view returns (uint256) {

250:   function rdpxCollateral() public view returns (uint256) {

```
[#L145](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L145) [#L180](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L180) [#L185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L185) [#L190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L190) [#L199](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L199) [#L208](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L208) [#L240](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L240) [#L250](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L250) 

</details>

---


## Gas Optimizations

<a name="GAS-1"></a> 
### [GAS-1] Multiple `address`/ID mappings can be combined into a single `mapping` of an `address`/ID to a `struct`, where appropriate
Saves a storage slot for the mapping. Depending on the circumstances and sizes of types, can avoid a Gsset (20000 gas) per mapping combined. Reads and subsequent writes can also be cheaper when a function requires both values and they both fit in the same storage slot. Finally, if both fields are accessed in the same function, can save ~42 gas per access due to not having to [recalculate the key's keccak256 hash](https://gist.github.com/IllIllI000/ec23a57daa30a8f8ca8b9681c8ccefb0) (Gkeccak256 - 30 gas) and that calculation's associated stack operations.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

69:   mapping(uint256 => mapping(uint256 => uint256))

```
[#L69](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L69) 

---

<a name="GAS-2"></a> 
### [GAS-2] Consider activating via-ir for deploying
By using `--via-ir` or `{"viaIR": true}`, the compiler is able to use more advanced [multi-function optimizations](https://docs.soliditylang.org/en/v0.8.17/ir-breaking-changes.html#solidity-ir-based-codegen-changes), for extra gas savings.

There is <b>1</b> instance:
```solidity

Global finding

```


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
[#L373](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L373) 

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
[#L535](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L535) [#L539](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L539) [#L546](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L546) [#L547](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L547) [#L548](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L548) [#L549](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L549) [#L570](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L570) [#L574](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L574) [#L579](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L579) [#L605](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L605) [#L608](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L608) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L612) [#L658](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L658) [#L665](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L665) [#L669](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L669) [#L673](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L673) [#L1165](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1165) [#L1170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1170) [#L1172](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1172) [#L1176](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1176) [#L1176](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1176) [#L1181](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1181) [#L1185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1185) [#L1190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1190) 

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
[#L270](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L270) [#L276](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L276) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L335) [#L475](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L475) [#L481](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L481) [#L487](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L487) [#L512](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L512) [#L516](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L516) [#L521](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L521) [#L550](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L550) [#L559](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L559) [#L604](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L604) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L612) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

281:       ((_rdpxCollateral * rdpxPriceInAlphaToken) / 1e8);

```
[#L281](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L281) 

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
[#L230](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L230) [#L232](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L232) [#L235](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L235) [#L239](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L239) [#L251](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L251) [#L252](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L252) [#L254](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L254) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) [#L279](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L279) [#L290](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L290) 

</details>

---

<a name="GAS-4"></a> 
### [GAS-4] Don't transfer with zero amount to save gas
In Solidity, unnecessary operations can waste gas. For example, a transfer function without a zero amount check uses gas even if called with a zero amount, since the contract state remains unchanged. Implementing a zero amount check avoids these unnecessary function calls, saving gas and improving efficiency.

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

170:     collateral.transfer(receiver, assets);

```
[#L170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L170) 

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
[#L235](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L235) [#L283](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L283) 

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
[#L486](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L486) [#L570](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L570) [#L650](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L650) [#L681](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L681) [#L711](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L711) [#L717](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L717) [#L720](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L720) [#L779](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L779) [#L780](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L780) [#L803](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L803) [#L851](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L851) [#L852](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L852) [#L916](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L916) [#L964](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L964) [#L1067](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1067) [#L1106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1106) [#L1110](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1110) [#L1196](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1196) 

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
[#L302](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L302) [#L303](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L303) [#L304](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L304) [#L309](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L309) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L335) [#L336](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L336) [#L337](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L337) [#L338](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L338) [#L437](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L437) [#L440](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L440) [#L445](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L445) [#L449](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L449) [#L493](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L493) 

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
[#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L132) [#L164](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L164) [#L181](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L181) [#L186](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L186) [#L195](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L195) [#L204](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L204) [#L213](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L213) [#L291](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L291) 

</details>

---

<a name="GAS-6"></a> 
### [GAS-6] `internal` functions only called once can be inlined to save gas
If an `internal` function is only used once, there is no need to modularize it, unless the function calling it would otherwise be too long and complex. Not inlining costs 20 to 40 gas because of two extra JUMP instructions and additional stack operations needed for function calls.

There are <b>5</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit `_issueBond` is used only once
495:   function _issueBond(

/// @audit `_calculateAmounts` is used only once
598:   function _calculateAmounts(

/// @audit `_bondWithDelegate` is used only once
699:   function _bondWithDelegate(

```
[#L495](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L495) [#L598](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L598) [#L699](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L699) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit `_convertToAssets` is used only once
218:   function _convertToAssets(

/// @audit `beforeWithdraw` is used only once
286:   function beforeWithdraw(uint256 assets, uint256 /*shares*/) internal {

```
[#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L218) [#L286](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L286) 

---

<a name="GAS-7"></a> 
### [GAS-7] `keccak256()` hash of literals should only be computed once
The result of the hash should be stored in an immutable variable, and the variable should be used instead. If the hash is being used as a part of a function selector, the cast to `bytes4` should also only be done once.

There are <b>9</b> instances:
```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L22) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L31](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L31) [#L34](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L34) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L19](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L19) [#L20](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L20) [#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L45) [#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L48) 

```solidity
File: contracts/reLP/ReLPContract.sol

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L70) 

---

<a name="GAS-8"></a> 
### [GAS-8] Low level `call` can be optimized with assembly
When using low-level calls, the `returnData` is copied to memory even if the variable is not utilized. The proper way to handle this is through a low level assembly call.

There are <b>2</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

344:     (bool success, bytes memory result) = _to.call{ value: _value }(_data);

```
[#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L344) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

98:       (bool success, ) = to.call{ value: amount, gas: gas }("");

```
[#L98](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L98) 

---

<a name="GAS-9"></a> 
### [GAS-9] Multiple accesses of the same mapping/array key/index should be cached
The instances below point to the second+ access of a value inside a mapping/array, within a function. Caching a mapping's value in a local `storage` or `calldata` variable when the value is accessed [multiple times](https://gist.github.com/IllIllI000/ec23a57daa30a8f8ca8b9681c8ccefb0), saves ~42 gas per access due to not having to recalculate the key's keccak256 hash (Gkeccak256 - 30 gas) and that calculation's associated stack operations. Caching an array's struct avoids recalculating the array offsets into memory/calldata

<details>
<summary>
There are <b>17</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit `positions_array[positionIndex]` is also accessed on line 218
259:     positions_array[positionIndex] = positions_array[

/// @audit `positions_mapping[pos.token_id]` is also accessed on line 263
269:     emit log(positions_mapping[pos.token_id].token_id);

```
[#L259](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L259) [#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L269) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit `reservesIndex[_assetSymbol]` is also accessed on line 273
277:     reservesIndex[_assetSymbol] = 0;

/// @audit `fundingPaidFor[pointer]` is also accessed on line 798
805:     fundingPaidFor[pointer] = true;

/// @audit `reserveAsset[i]` is also accessed on line 997
1001:       if (weth == reserveAsset[i].tokenAddress) {

/// @audit `reserveAsset[i]` is also accessed on line 997
1004:       reserveAsset[i].tokenBalance = balance;

/// @audit `bonds[id]` is also accessed on line 1021
1023:     _validate(block.timestamp > bonds[id].maturity, 7);

/// @audit `bonds[id]` is also accessed on line 1021
1035:     receiptTokenAmount = bonds[id].amount;

/// @audit ` = ` is also accessed on line 1093
1094:       path[0] = reserveAsset[reservesIndex["RDPX"]].tokenAddress;

/// @audit `reserveAsset[reservesIndex["RDPX"]` is also accessed on line 1094
1106:       reserveAsset[reservesIndex["RDPX"]].tokenBalance -= _rdpxAmount;

/// @audit `reservesIndex["RDPX"]` is also accessed on line 1094
1106:       reserveAsset[reservesIndex["RDPX"]].tokenBalance -= _rdpxAmount;

```
[#L277](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L277) [#L805](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L805) [#L1001](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1001) [#L1004](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1004) [#L1023](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1023) [#L1035](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1035) [#L1094](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1094) [#L1106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1106) [#L1106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1106) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit `optionPositions[optionIds[i]` is also accessed on line 329
330:       uint256 amount = optionPositions[optionIds[i]].amount;

/// @audit `optionPositions[optionIds[i]` is also accessed on line 329
343:       optionPositions[optionIds[i]].strike = 0;

/// @audit `totalFundingForEpoch[latestFundingPaymentPointer]` is also accessed on line 385
387:     _updateFundingRate(totalFundingForEpoch[latestFundingPaymentPointer]);

/// @audit `totalFundingForEpoch[latestFundingPaymentPointer]` is also accessed on line 385
391:       totalFundingForEpoch[latestFundingPaymentPointer],

/// @audit `totalFundingForEpoch[latestFundingPaymentPointer]` is also accessed on line 385
395:     return (totalFundingForEpoch[latestFundingPaymentPointer]);

/// @audit `fundingPaymentsAccountedForPerStrike[latestFundingPaymentPointer]` is also accessed on line 422
443:       fundingPaymentsAccountedForPerStrike[latestFundingPaymentPointer][

```
[#L330](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L330) [#L343](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L343) [#L387](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L387) [#L391](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L391) [#L395](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L395) [#L443](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L443) 

</details>

---

<a name="GAS-10"></a> 
### [GAS-10] Newer versions of solidity are more gas efficient
The solidity language continues to pursue more efficient gas optimization schemes. Adopting a newer version of solidity can be more gas efficient.

There are <b>9</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L2) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L2) 

```solidity
File: contracts/core/RdpxV2Bond.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L2) 

```solidity
File: contracts/core/RdpxV2Core.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L2) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L2) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L2) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L2) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L2) 

```solidity
File: contracts/reLP/ReLPContract.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L2) 

---

<a name="GAS-11"></a> 
### [GAS-11] Operator `>=`/`<=` costs less gas than operator `>`/`<`
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
[#L113](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L113) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L133) [#L147](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L147) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```
[#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L120) 

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
[#L167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L167) [#L183](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L183) [#L196](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L196) [#L231](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L231) [#L246](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L246) [#L391](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L391) [#L410](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L410) [#L444](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L444) [#L458](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L458) [#L556](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L556) [#L775](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L775) [#L836](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L836) [#L901](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L901) [#L947](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L947) [#L949](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L949) [#L979](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L979) [#L984](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L984) [#L996](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L996) [#L1021](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1021) [#L1023](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1023) [#L1167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1167) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

156:     for (uint256 i; i < ownerTokenCount; i++) {

```
[#L103](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L103) [#L156](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L156) 

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
[#L225](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L225) [#L265](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L265) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L328) [#L413](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L413) [#L464](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L464) [#L547](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L547) [#L559](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L559) [#L597](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L597) 

```solidity
File: contracts/reLP/ReLPContract.sol

94:       _reLPFactor > 0,

175:       _liquiditySlippageTolerance > 0,

190:       _slippageTolerance > 0,

```
[#L94](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L94) [#L175](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L175) [#L190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L190) 

</details>

---

<a name="GAS-12"></a> 
### [GAS-12] Redundant state variable getters
Getters for public state variables are automatically generated so there is no need to code them manually and waste gas.

There are <b>3</b> instances:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

240:   function activeCollateral() public view returns (uint256) {
         return _activeCollateral;

245:   function totalCollateral() public view returns (uint256) {
         return _totalCollateral;

250:   function rdpxCollateral() public view returns (uint256) {
         return _rdpxCollateral;

```
[#L240](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L240) [#L245](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L245) [#L250](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L250) 

---

<a name="GAS-13"></a> 
### [GAS-13] Remove or replace unused state variables
Saves a storage slot. If the variable is assigned a non-zero value, saves Gsset (20000 gas). If it's assigned a zero value, saves Gsreset (2900 gas). If the variable remains unassigned, there is no gas savings unless the variable is `public`, in which case the compiler-generated non-payable getter deployment cost is saved. If the state variable is overriding an interface's public function, mark the variable as `constant` or `immutable` so that it does not use a storage slot.

There is <b>1</b> instance:
```solidity
File: contracts/dpxETH/DpxEthToken.sol

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

---

<a name="GAS-14"></a> 
### [GAS-14] `require()`/`revert()` strings longer than 32 bytes cost extra gas
Each extra memory word of bytes past the original 32 [incurs an MSTORE](https://gist.github.com/hrkrshnn/ee8fabd532058307229d65dcd5836ddc#consider-having-short-revert-strings) which costs 3 gas

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

83:     require(
          _tokenA != address(0) &&
            _tokenB != address(0) &&
            _pair != address(0) &&
            _rdpxV2Core != address(0) &&
            _rdpxOracle != address(0) &&
            _ammFactory != address(0) &&
            _ammRouter != address(0),
          "reLPContract: address cannot be 0"

112:     require(
           _slippageTolerance > 0,
           "reLPContract: slippage tolerance must be greater than 0"

132:     require(_spender != address(0), "reLPContract: spender cannot be 0");

133:     require(_amount > 0, "reLPContract: amount must be greater than 0");

```
[#L83](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L83) [#L112](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L112) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L132) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L133) 

```solidity
File: contracts/core/RdpxV2Core.sol

244:     require(_asset != address(0), "RdpxV2Core: asset cannot be 0 address");

```
[#L244](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L244) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

191:     require(
           collateral.balanceOf(address(this)) >= _totalCollateral + proceeds,
           "Not enough collateral token was sent"

200:     require(
           collateral.balanceOf(address(this)) == _totalCollateral - loss,
           "Not enough collateral was sent out"

287:     require(
           assets <= totalAvailableCollateral(),
           "Not enough available assets to satisfy withdrawal"

```
[#L191](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L191) [#L200](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L200) [#L287](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L287) 

```solidity
File: contracts/reLP/ReLPContract.sol

93:     require(
          _reLPFactor > 0,
          "reLPContract: reLP factor must be greater than 0"

126:     require(
           _tokenA != address(0) &&
             _tokenB != address(0) &&
             _pair != address(0) &&
             _rdpxV2Core != address(0) &&
             _tokenAReserve != address(0) &&
             _amo != address(0) &&
             _rdpxOracle != address(0) &&
             _ammFactory != address(0) &&
             _ammRouter != address(0),
           "reLPContract: address cannot be 0"

174:     require(
           _liquiditySlippageTolerance > 0,
           "reLPContract: liquidity slippage tolerance must be greater than 0"

189:     require(
           _slippageTolerance > 0,
           "reLPContract: slippage tolerance must be greater than 0"

```
[#L93](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L93) [#L126](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L126) [#L174](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L174) [#L189](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L189) 

</details>

---

<a name="GAS-15"></a> 
### [GAS-15] The result of a function call should be cached rather than re-calling the function
The function calls in solidity are expensive. If the same result of the same function calls are to be used several times, the result should be cached to reduce the gas consumption of repeated calls.

There are <b>4</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit `getDpxEthPrice` is called 2 times
/// @audit `getEthPrice` is called 2 times
515:   function _curveSwap(
         uint256 _amount,
         bool _ethToDpxEth,
         bool validate,
         uint256 minAmount
       ) internal returns (uint256 amountOut) {

/// @audit `withdraw` is called 2 times
/// @audit `getRdpxPrice` is called 2 times
624:   function _transfer(
         uint256 _rdpxAmount,
         uint256 _wethAmount,
         uint256 _bondAmount,
         uint256 _bondId
       ) internal {

```
[#L515](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L515) [#L624](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L624) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit `nextFundingPaymentTimestamp` is called 7 times
462:   function updateFundingPaymentPointer() public {
         while (block.timestamp >= nextFundingPaymentTimestamp()) {

/// @audit `nextFundingPaymentTimestamp` is called 4 times
594:   function _updateFundingRate(uint256 amount) private {
         if (fundingRates[latestFundingPaymentPointer] == 0) {

```
[#L462](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L462) [#L594](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L594) 

---

<a name="GAS-16"></a> 
### [GAS-16] Unlimited gas consumption risk due to external call recipients
When calling an external function without specifying a gas limit , the called contract may consume all the remaining gas, causing the tx to be reverted. To mitigate this, it is recommended to explicitly set a gas limit when making low level external calls.

There is <b>1</b> instance:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

344:     (bool success, bytes memory result) = _to.call{ value: _value }(_data);

```
[#L344](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L344) 

---

<a name="GAS-17"></a> 
### [GAS-17] Unused named return variables without optimizer waste gas
Consider changing the variable to be an unnamed one, since the variable is never assigned, nor is it returned by name. If the optimizer is not turned on, leaving the code as it is will also waste gas for the stack variable.

There are <b>8</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit `` not used
819:   function bondWithDelegate(
         address _to,
         uint256[] memory _amounts,
         uint256[] memory _delegateIds,
         uint256 rdpxBondId
       ) public returns (uint256 receiptTokenAmount, uint256[] memory) {

/// @audit `dpxEthPrice` not used
1216:   function getDpxEthPrice() public view returns (uint256 dpxEthPrice) {

/// @audit `ethPrice` not used
1227:   function getEthPrice() public view returns (uint256 ethPrice) {

/// @audit `delegate` not used
1260:   function getDelegatePosition(
          uint256 _delegateId
        )
          public
          view
          returns (
            address delegate,
            uint256 amount,
            uint256 fee,
            uint256 activeCollateral
          )
        {

```
[#L819](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L819) [#L1216](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1216) [#L1227](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1227) [#L1260](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1260) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit `timestamp` not used
563:   function nextFundingPaymentTimestamp()
         public
         view
         returns (uint256 timestamp)
       {
         return genesis + (latestFundingPaymentPointer * fundingDuration);

/// @audit `strike` not used
576:   function roundUp(uint256 _strike) public view returns (uint256 strike) {
         uint256 remainder = _strike % roundingPrecision;

```
[#L563](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L563) [#L576](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L576) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit `assets` not used
/// @audit `rdpxAmount` not used
218:   function _convertToAssets(
         uint256 shares
       ) internal view virtual returns (uint256 assets, uint256 rdpxAmount) {

/// @audit `shares` not used
274:   function convertToShares(
         uint256 assets
       ) public view returns (uint256 shares) {

```
[#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L218) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L274) 

---

<a name="GAS-18"></a> 
### [GAS-18] Use assembly to compute hashes to save gas
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
[#L106](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L106) 

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L22) 

```solidity
File: contracts/core/RdpxV2Core.sol

1141:       keccak256(abi.encodePacked(asset.tokenSymbol)) ==

1142:         keccak256(abi.encodePacked(_token)),

```
[#L1141](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1141) [#L1142](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1142) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L31](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L31) [#L34](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L34) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L19](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L19) [#L20](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L20) [#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L45) [#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L48) 

```solidity
File: contracts/reLP/ReLPContract.sol

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L70) 

</details>

---

<a name="GAS-19"></a> 
### [GAS-19] Use assembly to emit events
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
[#L152](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L152) [#L177](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L177) [#L240](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L240) [#L288](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L288) [#L348](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L348) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

268:     emit log(positions_array.length);

269:     emit log(positions_mapping[pos.token_id].token_id);

321:     emit RecoveredERC20(tokenAddress, tokenAmount);

335:     emit RecoveredERC721(tokenAddress, token_id);

363:     emit LogAssetsTransfered(tokenABalance, tokenBBalance, tokenA, tokenB);

```
[#L268](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L268) [#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L269) [#L321](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L321) [#L335](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L335) [#L363](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L363) 

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
[#L172](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L172) [#L185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L185) [#L198](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L198) [#L208](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L208) [#L220](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L220) [#L233](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L233) [#L263](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L263) [#L289](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L289) [#L349](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L349) [#L370](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L370) [#L447](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L447) [#L461](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L461) [#L782](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L782) [#L807](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L807) [#L875](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L875) [#L932](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L932) [#L966](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L966) [#L989](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L989) [#L1007](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1007) [#L1041](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1041) [#L1069](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1069) [#L1123](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1123) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

124:     emit BondMinted(to, bondId, expiry, rdpxAmount);

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L124) 

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
[#L211](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L211) [#L230](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L230) [#L311](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L311) [#L368](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L368) [#L389](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L389) [#L451](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L451) [#L485](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L485) [#L494](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L494) [#L519](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L519) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

134:     emit Deposit(msg.sender, receiver, assets, shares);

174:     emit Withdraw(msg.sender, receiver, owner, assets, shares);

```
[#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L134) [#L174](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L174) 

```solidity
File: contracts/reLP/ReLPContract.sol

99:     emit LogSetReLpFactor(_reLPFactor);

```
[#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L99) 

</details>

---

<a name="GAS-20"></a> 
### [GAS-20] Using a double `if` statement instead of a logical AND (`&&`)
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
[#L84](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L84) [#L85](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L85) [#L86](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L86) [#L87](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L87) [#L88](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L88) [#L89](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L89) 

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
[#L127](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L127) [#L128](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L128) [#L129](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L129) [#L130](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L130) [#L131](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L131) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L132) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L133) [#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L134) 

</details>

---

<a name="GAS-21"></a> 
### [GAS-21] Use a more recent version of solidity
- Use a solidity version of at least 0.8.2 to get simple compiler automatic inlining.
- Use a solidity version of at least 0.8.3 to get better struct packing and cheaper multiple storage reads.
- Use a solidity version of at least 0.8.4 to get custom errors, which are cheaper at deployment than revert()/require() strings.
- Use a solidity version of at least 0.8.10 to have external calls skip contract existence checks if the external call has a return value.

There are <b>9</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L2) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L2) 

```solidity
File: contracts/core/RdpxV2Bond.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L2) 

```solidity
File: contracts/core/RdpxV2Core.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L2) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L2) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L2) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L2) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L2) 

```solidity
File: contracts/reLP/ReLPContract.sol

2: pragma solidity 0.8.19;

```
[#L2](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L2) 

---

<a name="GAS-22"></a> 
### [GAS-22] Use `storage` instead of `memory` for structs/arrays
When fetching data from a storage location, assigning the data to a `memory` variable causes all fields of the struct/array to be read from storage, which incurs a Gcoldsload (**2100 gas**) for *each* field of the struct/array. If the fields are read from the new memory variable, they incur an additional `MLOAD` rather than a cheap stack read. Instead of declaring the variable with the `memory` keyword, declaring the variable with the `storage` keyword and caching any fields that need to be re-read in stack variables, will be much cheaper, only incurring the Gcoldsload for the fields actually read. The only time it makes sense to read the whole struct/array into a `memory` variable, is if the full struct/array is being returned by the function, is being passed to a function that requires `memory`, or if the array/struct is being read from another `memory` array/struct.

There are <b>4</b> instances:
```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

121:       Position memory current_position = positions_array[i];

218:     Position memory pos = positions_array[positionIndex];

```
[#L121](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L121) [#L218](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L218) 

```solidity
File: contracts/core/RdpxV2Core.sol

1138:     ReserveAsset memory asset = reserveAsset[reservesIndex[_token]];

1272:     Delegate memory delegatePosition = delegates[_delegateId];

```
[#L1138](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1138) [#L1272](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1272) 

---

<a name="GAS-23"></a> 
### [GAS-23] Use `unchecked` block for safe subtractions
If it can be confirmed that the subtraction operation will not overflow, using an unchecked block can save gas. For example, `require(x <= y); z = y - x;` can be optimized to `require(x <= y); unchecked { z = y - x; }`

There are <b>4</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit Checked on line 635
645:         amount - _rdpxAmount

```
[#L645](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L645) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit Checked on line 559
559:     return strike > price ? ((strike - price) * amount) / 1e8 : 0;

/// @audit Checked on line 609
605:         (endTime - startTime);

/// @audit Checked on line 609
612:         ((amount * 1e18) / (endTime - startTime));

```
[#L559](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L559) [#L605](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L605) [#L612](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L612) 

---

<a name="GAS-24"></a> 
### [GAS-24] Using bitmap to store bool states can save gas
Using a bitmap instead of a bool array or a bool mapping to store boolean states can save gas fees. This is because the bitmap can store 256 boolean values in a single slot instead of 256 slots, which can save gas when writing bool values or when reading multiple bool values from the same slot.

There are <b>2</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

79:   mapping(uint256 => bool) public optionsOwned;

82:   mapping(uint256 => bool) public fundingPaidFor;

```
[#L79](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L79) [#L82](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L82) 

---

<a name="GAS-25"></a> 
### [GAS-25] `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants)
When updating a value in an array with arithmetic, using `array[index] += amount` is cheaper than `array[index] = array[index] + amount`.
This is because you avoid an additonal `mload` when the array is stored in memory, and an `sload` when the array is stored in storage.
This can be applied for any arithmetic operation including `+=`, `-=`,`/=`,`*=`,`^=`,`&=`, `%=`, `<<=`,`>>=`, and `>>>=`.
This optimization can be particularly significant if the pattern occurs during a loop.

*Saves 28 gas for a storage array, 38 for a memory array*

There is <b>1</b> instance:
```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

610:       fundingRates[latestFundingPaymentPointer] =

```
[#L610](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L610) 

---

<a name="GAS-26"></a> 
### [GAS-26] Using bools for storage incurs overhead
Use uint256(1) and uint256(2) for true/false to avoid a Gwarmaccess (100 gas), and to avoid Gsset (20000 gas) when changing from ‘false’ to ‘true’, after having been ‘true’ in the past. See [source](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/58f635312aa21f947cae5f8578638a85aa2519f5/contracts/security/ReentrancyGuard.sol#L23-L27).

There are <b>4</b> instances:
```solidity
File: contracts/core/RdpxV2Core.sol

79:   mapping(uint256 => bool) public optionsOwned;

82:   mapping(uint256 => bool) public fundingPaidFor;

115:   bool public isReLPActive;

118:   bool public putOptionsRequired;

```
[#L79](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L79) [#L82](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L82) [#L115](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L115) [#L118](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L118) 

---

<a name="GAS-27"></a> 
### [GAS-27] Cache array length outside of loop
If not cached, the solidity compiler will always read the length of the array during each iteration. That is, if it is a storage array, this is an extra sload operation (100 additional extra gas for each iteration except for the first) and if it is a memory array, this is an extra mload operation (3 additional gas for each iteration except for the first).

<details>
<summary>
There are <b>11</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L147](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L147) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```
[#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L120) 

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

246:     for (uint256 i = 1; i < reserveAsset.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

996:     for (uint256 i = 1; i < reserveAsset.length; i++) {

```
[#L167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L167) [#L246](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L246) [#L775](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L775) [#L836](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L836) [#L996](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L996) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L103](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L103) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```
[#L225](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L225) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L328) [#L413](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L413) 

</details>

---

<a name="GAS-28"></a> 
### [GAS-28] State variables should be cached in stack variables rather than re-reading them from storage
The instances below point to the second+ access of a state variable within a function. Caching of a state variable replaces each Gwarmaccess (100 gas) with a much cheaper stack read. Other less obvious fixes/optimizations include having local memory caches of state variable structs, or having local caches of state variable contracts/addresses.

<details>
<summary>
There are <b>16</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

/// @audit More than 1 read for `addresses`, line 315 and 314
315:       token2 = addresses.tokenB;

/// @audit More than 1 read for `addresses`, line 317 and 314
317:       token1 = addresses.tokenB;

/// @audit More than 1 read for `addresses`, line 318 and 314
318:       token2 = addresses.tokenA;

```
[#L315](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L315) [#L317](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L317) [#L318](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L318) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

/// @audit More than 1 read for `positions_array`, line 259 and 218
259:     positions_array[positionIndex] = positions_array[

```
[#L259](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L259) 

```solidity
File: contracts/core/RdpxV2Core.sol

/// @audit More than 1 read for `weth`, line 716 and 711
716:     _validate(delegate.amount - delegate.activeCollateral >= wethRequired, 5);

/// @audit More than 1 read for `weth`, line 717 and 711
717:     delegate.activeCollateral += wethRequired;

/// @audit More than 1 read for `weth`, line 720 and 711
720:     totalWethDelegated -= wethRequired;

```
[#L716](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L716) [#L717](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L717) [#L720](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L720) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

/// @audit More than 1 read for `collateralToken`, line 121 and 119
121:     collateralToken = IERC20WithBurn(_collateralToken);

/// @audit More than 1 read for `collateralToken`, line 122 and 119
122:     underlyingSymbol = collateralToken.symbol();

/// @audit More than 1 read for `optionPositions`, line 330 and 329
330:       uint256 amount = optionPositions[optionIds[i]].amount;

/// @audit More than 1 read for `latestFundingPaymentPointer`, line 436 and 416
436:       latestFundingPerStrike[strike] = latestFundingPaymentPointer;

```
[#L121](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L121) [#L122](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L122) [#L330](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L330) [#L436](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L436) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

/// @audit More than 1 read for `_totalCollateral`, line 195 and 192
195:     _totalCollateral += proceeds;

/// @audit More than 1 read for `_totalCollateral`, line 204 and 201
204:     _totalCollateral -= loss;

/// @audit More than 1 read for `_rdpxCollateral`, line 213 and 210
213:     _rdpxCollateral += amount;

```
[#L195](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L195) [#L204](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L204) [#L213](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L213) 

```solidity
File: contracts/reLP/ReLPContract.sol

/// @audit More than 1 read for `addresses`, line 269 and 224
269:     path[0] = addresses.tokenB;

/// @audit More than 1 read for `addresses`, line 270 and 224
270:     path[1] = addresses.tokenA;

```
[#L269](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L269) [#L270](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L270) 

</details>

---

<a name="GAS-29"></a> 
### [GAS-29] Use `calldata` instead of `memory` for function arguments that do not get mutated
Mark data types as `calldata` instead of `memory` where possible. This makes it so that the data is not automatically loaded into memory. If the data passed into the function does not need to be changed (like updating values in an array), it can be passed in as `calldata`. The one exception to this is if the argument must later be passed into another function that takes an argument that specifies `memory` storage.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

156:     AddLiquidityParams memory params

```
[#L156](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L156) 

```solidity
File: contracts/core/RdpxV2Core.sol

242:     string memory _assetSymbol

271:     string memory _assetSymbol

765:     uint256[] memory optionIds

821:     uint256[] memory _amounts,

822:     uint256[] memory _delegateIds,

1136:     string memory _token

```
[#L242](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L242) [#L271](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L271) [#L765](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L765) [#L821](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L821) [#L822](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L822) [#L1136](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1136) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

57:     string memory _name,

58:     string memory _symbol

```
[#L57](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L57) [#L58](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L58) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

114:     string memory _name,

115:     string memory _symbol,

316:     uint256[] memory optionIds

406:     uint256[] memory strikes

```
[#L114](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L114) [#L115](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L115) [#L316](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L316) [#L406](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L406) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

86:     string memory _collateralSymbol

```
[#L86](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L86) 

</details>

---

<a name="GAS-30"></a> 
### [GAS-30] Use Custom Errors
[Source](https://blog.soliditylang.org/2021/04/21/custom-errors/)
Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

There are <b>8</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

131:     require(_token != address(0), "reLPContract: token cannot be 0");

132:     require(_spender != address(0), "reLPContract: spender cannot be 0");

133:     require(_amount > 0, "reLPContract: amount must be greater than 0");

```
[#L131](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L131) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L132) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L133) 

```solidity
File: contracts/core/RdpxV2Core.sol

244:     require(_asset != address(0), "RdpxV2Core: asset cannot be 0 address");

```
[#L244](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L244) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

99:       require(success, "RdpxReserve: transfer failed");

120:     require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter");

```
[#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L99) [#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L120) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

123:     require((shares = previewDeposit(assets)) != 0, "ZERO_SHARES");

162:     require(assets != 0, "ZERO_ASSETS");

```
[#L123](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L123) [#L162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L162) 

---

<a name="GAS-31"></a> 
### [GAS-31] Don't use `SafeMath` once the solidity version is 0.8.0 or greater
Solidity 0.8.0 introduces internal overflow checks, so using SafeMath is redundant and adds overhead.

There are <b>3</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

6: import { SafeMath } from "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[#L6](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L6) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

7: import { SafeMath } from "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[#L7](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L7) 

```solidity
File: contracts/reLP/ReLPContract.sol

6: import { SafeMath } from "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[#L6](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L6) 

---

<a name="GAS-32"></a> 
### [GAS-32] Don't initialize variables with default value

There are <b>10</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L147](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L147) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```
[#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L120) 

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

```
[#L167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L167) [#L775](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L775) [#L836](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L836) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L103](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L103) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

89:   uint256 public latestFundingPaymentPointer = 0;

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```
[#L89](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L89) [#L225](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L225) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L328) [#L413](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L413) 

---

<a name="GAS-33"></a> 
### [GAS-33] Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead
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
[#L43](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L43) [#L99](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L99) [#L105](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L105) [#L126](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L126) [#L127](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L127) [#L193](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L193) [#L223](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L223) [#L224](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L224) [#L235](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L235) [#L280](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L280) 

```solidity
File: contracts/core/RdpxV2Core.sol

553:       _ethToDpxEth ? int128(int256(a)) : int128(int256(b)),

553:       _ethToDpxEth ? int128(int256(a)) : int128(int256(b)),

554:       _ethToDpxEth ? int128(int256(b)) : int128(int256(a)),

554:       _ethToDpxEth ? int128(int256(b)) : int128(int256(a)),

```
[#L553](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L553) [#L553](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L553) [#L554](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L554) [#L554](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L554) 

</details>

---

<a name="GAS-34"></a> 
### [GAS-34] Constructors can be marked as `payable` to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. A constructor can be safely marked as payable, because only the deployer would be able to pass funds, and the project itself would not pass any funds.

There are <b>6</b> instances:
```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

57:   constructor() {

```
[#L57](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L57) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

76:   constructor(address _rdpx, address _rdpxV2Core) {

```
[#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L76) 

```solidity
File: contracts/core/RdpxV2Bond.sol

24:   constructor() ERC721("rDPX V2 Bond", "rDPXV2Bond") {

```
[#L24](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L24) 

```solidity
File: contracts/core/RdpxV2Core.sol

124:   constructor(address _weth) {

```
[#L124](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L124) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

23:   constructor() ERC20("Dopex Synthetic ETH", "dpxETH") {

```
[#L23](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L23) 

```solidity
File: contracts/reLP/ReLPContract.sol

79:   constructor() {

```
[#L79](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L79) 

---

<a name="GAS-35"></a> 
### [GAS-35] Functions guaranteed to revert when called by normal users can be marked `payable`
If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function. Marking the function as `payable` will lower the gas cost for legitimate callers because the compiler will not include checks for whether a payment was provided.

<details>
<summary>
There are <b>22</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

119:   function collectFees() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L119](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L119) 

```solidity
File: contracts/core/RdpxV2Bond.sol

29:   function pause() public onlyRole(DEFAULT_ADMIN_ROLE) {

33:   function unpause() public onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L33) 

```solidity
File: contracts/core/RdpxV2Core.sol

144:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

152:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

206:   function setIsreLP(bool _isReLPActive) external onlyRole(DEFAULT_ADMIN_ROLE) {

378:   function addAMOAddress(address _addr) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L144) [#L152](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L152) [#L206](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L206) [#L378](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L378) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

70:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

76:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L70) [#L76](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L76) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

29:   function pause() public onlyRole(PAUSER_ROLE) {

33:   function unpause() public onlyRole(PAUSER_ROLE) {

37:   function mint(address to, uint256 amount) public onlyRole(MINTER_ROLE) {

```
[#L29](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L29) [#L33](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L33) [#L37](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L37) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

136:   function pause() external onlyRole(DEFAULT_ADMIN_ROLE) {

144:   function unpause() external onlyRole(DEFAULT_ADMIN_ROLE) {

243:   function setLpAllowance(bool increase) external onlyRole(DEFAULT_ADMIN_ROLE) {

372:   function payFunding() external onlyRole(RDPXV2CORE_ROLE) returns (uint256) {

```
[#L136](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L136) [#L144](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L144) [#L243](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L243) [#L372](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L372) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

180:   function lockCollateral(uint256 amount) public onlyPerpVault {

185:   function unlockLiquidity(uint256 amount) public onlyPerpVault {

190:   function addProceeds(uint256 proceeds) public onlyPerpVault {

199:   function subtractLoss(uint256 loss) public onlyPerpVault {

208:   function addRdpx(uint256 amount) public onlyPerpVault {

```
[#L180](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L180) [#L185](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L185) [#L190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L190) [#L199](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L199) [#L208](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L208) 

```solidity
File: contracts/reLP/ReLPContract.sol

202:   function reLP(uint256 _amount) external onlyRole(RDPXV2CORE_ROLE) {

```
[#L202](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L202) 

</details>

---

<a name="GAS-36"></a> 
### [GAS-36] `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too)
*Saves 5 gas per loop*

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

147:     for (uint256 i = 0; i < tokens.length; i++) {

```
[#L147](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L147) 

```solidity
File: contracts/amo/UniV3LiquidityAmo.sol

120:     for (uint i = 0; i < positions_array.length; i++) {

```
[#L120](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV3LiquidityAmo.sol#L120) 

```solidity
File: contracts/core/RdpxV2Core.sol

167:     for (uint256 i = 0; i < tokens.length; i++) {

246:     for (uint256 i = 1; i < reserveAsset.length; i++) {

775:     for (uint256 i = 0; i < optionIds.length; i++) {

836:     for (uint256 i = 0; i < _amounts.length; i++) {

996:     for (uint256 i = 1; i < reserveAsset.length; i++) {

```
[#L167](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L167) [#L246](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L246) [#L775](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L775) [#L836](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L836) [#L996](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L996) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

103:     for (uint256 i = 0; i < tokens.length; i++) {

156:     for (uint256 i; i < ownerTokenCount; i++) {

```
[#L103](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L103) [#L156](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L156) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

225:     for (uint256 i = 0; i < tokens.length; i++) {

328:     for (uint256 i = 0; i < optionIds.length; i++) {

413:     for (uint256 i = 0; i < strikes.length; i++) {

```
[#L225](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L225) [#L328](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L328) [#L413](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L413) 

</details>

---

<a name="GAS-37"></a> 
### [GAS-37] Using `private` rather than `public` for constants, saves gas
If needed, the values can be read from the verified contract source code, or if there are multiple values there can be a single getter function that [returns a tuple](https://github.com/code-423n4/2022-08-frax/blob/90f55a9ce4e25bceed3a74290b854341d8de6afa/src/contracts/FraxlendPair.sol#L156-L178) of the values of all currently-public constants. Saves **3406-3606 gas** in deployment gas due to the compiler not having to create non-payable getter functions for deployment calldata, not having to store the bytes of the value outside of where it's used, and not adding another entry to the method ID table

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/amo/UniV2LiquidityAmo.sol

48:   uint256 public constant DEFAULT_PRECISION = 1e8;

```
[#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L48) 

```solidity
File: contracts/core/RdpxV2Bond.sol

22:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

```
[#L22](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Bond.sol#L22) 

```solidity
File: contracts/core/RdpxV2Core.sol

85:   uint256 public constant DEFAULT_PRECISION = 1e8;

88:   uint256 public constant RDPX_RATIO_PERCENTAGE = 25 * DEFAULT_PRECISION;

91:   uint256 public constant ETH_RATIO_PERCENTAGE = 75 * DEFAULT_PRECISION;

```
[#L85](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L85) [#L88](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L88) [#L91](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L91) 

```solidity
File: contracts/decaying-bonds/RdpxDecayingBonds.sol

31:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

34:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L31](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L31) [#L34](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/decaying-bonds/RdpxDecayingBonds.sol#L34) 

```solidity
File: contracts/dpxETH/DpxEthToken.sol

19:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

20:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

21:   bytes32 public constant BURNER_ROLE = keccak256("BURNER_ROLE");

```
[#L19](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L19) [#L20](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L20) [#L21](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/dpxETH/DpxEthToken.sol#L21) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

45:   bytes32 public constant MANAGER_ROLE = keccak256("MANAGER_ROLE");

48:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L45](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L45) [#L48](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L48) 

```solidity
File: contracts/reLP/ReLPContract.sol

67:   uint256 public constant DEFAULT_PRECISION = 1e8;

70:   bytes32 public constant RDPXV2CORE_ROLE = keccak256("RDPXV2CORE_ROLE");

```
[#L67](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L67) [#L70](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L70) 

</details>

---

<a name="GAS-38"></a> 
### [GAS-38] Use shift Right/Left instead of division/multiplication if possible

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
[#L535](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L535) [#L539](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L539) [#L570](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L570) [#L574](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L574) [#L579](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L579) [#L1170](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1170) [#L1176](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1176) [#L1190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1190) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

270:     uint256 strike = roundUp(currentPrice - (currentPrice / 4)); // 25% below the current price

```
[#L270](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L270) 

```solidity
File: contracts/reLP/ReLPContract.sol

274:       (((amountB / 2) * tokenAInfo.tokenAPrice) / 1e8) -

275:       (((amountB / 2) * tokenAInfo.tokenAPrice * slippageTolerance) / 1e16);

279:         amountB / 2,

290:       amountB / 2,

```
[#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L274) [#L275](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L275) [#L279](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L279) [#L290](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L290) 

</details>

---

<a name="GAS-39"></a> 
### [GAS-39] Use `!= 0` instead of `> 0` for unsigned integer comparison
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
[#L113](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L113) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L133) 

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
[#L183](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L183) [#L196](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L196) [#L231](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L231) [#L410](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L410) [#L444](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L444) [#L458](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L458) [#L556](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L556) [#L838](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L838) [#L901](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L901) [#L984](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L984) [#L1021](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1021) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVault.sol

265:     _validate(amount > 0, 2);

414:       _validate(optionsPerStrike[strikes[i]] > 0, 4);

547:       _price > 0 ? _price : getUnderlyingPrice(),

```
[#L265](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L265) [#L414](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L414) [#L547](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L547) 

```solidity
File: contracts/reLP/ReLPContract.sol

94:       _reLPFactor > 0,

175:       _liquiditySlippageTolerance > 0,

190:       _slippageTolerance > 0,

```
[#L94](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L94) [#L175](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L175) [#L190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L190) 

</details>

---

<a name="GAS-40"></a> 
### [GAS-40] Using assembly to check for zero can save gas
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

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
[#L84](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L84) [#L85](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L85) [#L86](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L86) [#L87](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L87) [#L88](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L88) [#L89](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L89) [#L90](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L90) [#L131](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L131) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/amo/UniV2LiquidityAmo.sol#L132) 

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
[#L244](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L244) [#L274](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L274) [#L316](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L316) [#L317](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L317) [#L318](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L318) [#L319](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L319) [#L320](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L320) [#L321](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L321) [#L322](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L322) [#L323](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L323) [#L324](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L324) [#L325](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L325) [#L362](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L362) [#L363](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L363) [#L379](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L379) [#L408](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L408) [#L409](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L409) [#L630](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L630) [#L1091](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1091) [#L1162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/core/RdpxV2Core.sol#L1162) 

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
[#L119](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L119) [#L190](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L190) [#L191](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L191) [#L192](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L192) [#L193](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L193) [#L194](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L194) [#L195](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L195) [#L196](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L196) [#L467](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L467) [#L505](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L505) [#L578](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L578) [#L595](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVault.sol#L595) 

```solidity
File: contracts/perp-vault/PerpetualAtlanticVaultLP.sol

95:       _perpetualAtlanticVault != address(0) || _rdpx != address(0),

95:       _perpetualAtlanticVault != address(0) || _rdpx != address(0),

123:     require((shares = previewDeposit(assets)) != 0, "ZERO_SHARES");

162:     require(assets != 0, "ZERO_ASSETS");

223:       (supply == 0)

283:       supply == 0 ? assets : assets.mulDivDown(supply, totalVaultCollateral);

```
[#L95](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L95) [#L95](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L95) [#L123](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L123) [#L162](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L162) [#L223](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L223) [#L283](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/perp-vault/PerpetualAtlanticVaultLP.sol#L283) 

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
[#L127](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L127) [#L128](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L128) [#L129](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L129) [#L130](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L130) [#L131](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L131) [#L132](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L132) [#L133](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L133) [#L134](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L134) [#L135](https://github.com/code-423n4/2023-08-dopex/blob/0ea4387a4851cd6c8811dfb61da95a677f3f63ae/contracts/reLP/ReLPContract.sol#L135) 

</details>

---

