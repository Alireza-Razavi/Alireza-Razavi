# Report


## Medium Issues


Total <b>39</b> instances over <b>4</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | The remaining ETH may be locked in the contract after call | 2 |
| [M-2](#M-2) | Return values of `transfer()`/`transferFrom()` not checked | 4 |
| [M-3](#M-3) | Unsafe use of ERC20 `transfer()`/`transferFrom()` | 4 |
| [M-4](#M-4) | Centralization Risk for trusted owners | 29 |

## Low Issues


Total <b>105</b> instances over <b>22</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Array is `push()`ed but not `pop()`ed | 5 |
| [L-2](#L-2) | Check division by zero is prevented | 12 |
| [L-3](#L-3) | Consider implementing two-step procedure for updating protocol addresses | 4 |
| [L-4](#L-4) | Constructor / initialization function lacks parameter validation | 5 |
| [L-5](#L-5) | Enum values should be used instead of constant array indexes | 2 |
| [L-6](#L-6) | External call recipient can consume all remaining gas | 2 |
| [L-7](#L-7) | Governance functions should be controlled by time locks | 29 |
| [L-8](#L-8) | Loss of precision in divisions | 12 |
| [L-9](#L-9) | Missing contract existence checks before low-level calls | 2 |
| [L-10](#L-10) | Missing zero address check in constructor | 4 |
| [L-11](#L-11) | Missing checks for `address(0)` when setting address state variables | 1 |
| [L-12](#L-12) | Missing storage gap for upgradable contracts | 1 |
| [L-13](#L-13) | Owner can renounce Ownership | 2 |
| [L-14](#L-14) | prevent re-setting a state variable with the same value | 4 |
| [L-15](#L-15) | Some tokens may revert when large transfers are made | 3 |
| [L-16](#L-16) | Some tokens may revert when zero value transfers are made | 3 |
| [L-17](#L-17) | Timestamp may be manipulation | 4 |
| [L-18](#L-18) | Unsafe solidity low-level call can cause gas grief attack | 2 |
| [L-19](#L-19) | Use Ownable2Step instead of Ownable | 2 |
| [L-20](#L-20) | Using zero as a parameter | 4 |
| [L-21](#L-21) | Missing zero address check in initializer | 1 |
| [L-22](#L-22) | Initializers could be front-run | 1 |

## Non Critical Issues


Total <b>410</b> instances over <b>50</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | `assert()` should be replaced with `require()` or `revert()` | 1 |
| [NC-2](#NC-2) | Contract declarations should have NatSpec `@author` annotations | 3 |
| [NC-3](#NC-3) | Consider adding formal verification proofs | 1 |
| [NC-4](#NC-4) | Consider bounding input array length | 2 |
| [NC-5](#NC-5) | Constants should be put on the left side of comparisons | 16 |
| [NC-6](#NC-6) | Contract name does not follow the Solidity Style Guide | 2 |
| [NC-7](#NC-7) | Contract uses both `require()`/`revert()` as well as custom errors | 3 |
| [NC-8](#NC-8) | Contracts should have full test coverage | 1 |
| [NC-9](#NC-9) | Events that mark critical parameter changes should contain both the old and the new value | 16 |
| [NC-10](#NC-10) | Custom errors has no error details | 15 |
| [NC-11](#NC-11) | Custom errors should be used rather than `revert()`/`require()` | 21 |
| [NC-12](#NC-12) | `else` block not required | 3 |
| [NC-13](#NC-13) | Enable IR-based code generation | 1 |
| [NC-14](#NC-14) | Names of structs, events, enums and errors should use CapWords style | 1 |
| [NC-15](#NC-15) | Events are emitted without the sender information | 14 |
| [NC-16](#NC-16) | Import declarations should import specific identifiers, rather than the whole file | 32 |
| [NC-17](#NC-17) | Large or complicated code bases should implement invariant tests | 1 |
| [NC-18](#NC-18) | Large multiples of ten should use scientific notation | 1 |
| [NC-19](#NC-19) | Magic numbers should be replaced with constants | 14 |
| [NC-20](#NC-20) | Missing zero address check in functions with address parameters | 23 |
| [NC-21](#NC-21) | Consider moving `msg.sender` checks to `modifier`s | 3 |
| [NC-22](#NC-22) | Named mappings are recommended | 9 |
| [NC-23](#NC-23) | NatSpec documentation for contract is missing | 3 |
| [NC-24](#NC-24) | NatSpec documentation for function is missing | 11 |
| [NC-25](#NC-25) | Modifier declarations should have NatSpec descriptions | 1 |
| [NC-26](#NC-26) | Missing NatSpec `@param` | 28 |
| [NC-27](#NC-27) | Public variable declarations should have NatSpec descriptions | 19 |
| [NC-28](#NC-28) | NatSpec `@return` is missing | 15 |
| [NC-29](#NC-29) | There is no need to initialize variables with 0 | 8 |
| [NC-30](#NC-30) | Put all system-wide constants in one file | 13 |
| [NC-31](#NC-31) | SPDX identifier should be the in the first line of a solidity file | 6 |
| [NC-32](#NC-32) | State variables should include comments | 11 |
| [NC-33](#NC-33) | Contract declarations should have NatSpec `@title` annotations | 3 |
| [NC-34](#NC-34) | Unused errors | 2 |
| [NC-35](#NC-35) | Unused named return | 3 |
| [NC-36](#NC-36) | Unused contract variables | 1 |
| [NC-37](#NC-37) | Consider using `delete` rather than assigning zero to clear values | 8 |
| [NC-38](#NC-38) | Expressions for constant values should use `immutable` rather than `constant` | 13 |
| [NC-39](#NC-39) | Use the latest solidity version for deployment | 6 |
| [NC-40](#NC-40) | Use of `override` is unnecessary | 6 |
| [NC-41](#NC-41) | Use scientific notation (e.g. `1e18`) rather than exponentiation (e.g. `10**18`) | 1 |
| [NC-42](#NC-42) | Missing checks for `address(0)` when assigning values to address state variables | 1 |
| [NC-43](#NC-43) | Common functions should be refactored to a common base contract | 8 |
| [NC-44](#NC-44) | Names of `private`/`internal` functions should be prefixed with an underscore | 2 |
| [NC-45](#NC-45) | Names of `private`/`internal` state variables should be prefixed with an underscore | 5 |
| [NC-46](#NC-46) |  `require()` / `revert()` statements should have descriptive reason strings | 1 |
| [NC-47](#NC-47) | Return values of `approve()` not checked | 6 |
| [NC-48](#NC-48) | Variables should be named in mixedCase style | 19 |
| [NC-49](#NC-49) | Event is missing `indexed` fields | 13 |
| [NC-50](#NC-50) | Functions not used internally could be marked external | 14 |

## Gas Optimizations


Total <b>263</b> instances over <b>40</b> issues:

|ID|Issue|Instances|Gas|
|-|:-|:-:|:-:|
| [GAS-1](#GAS-1) | Consider activating via-ir for deploying | 1 | - |
| [GAS-2](#GAS-2) | Divisions can be `unchecked` to save gas | 12 | 240 |
| [GAS-3](#GAS-3) | Don't transfer with zero amount to save gas | 3 | - |
| [GAS-4](#GAS-4) | Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables | 4 | 452 |
| [GAS-5](#GAS-5) | Increments can be `unchecked` to save gas | 8 | 480 |
| [GAS-6](#GAS-6) | Initializers can be marked as payable to save deployment gas | 1 | 21 |
| [GAS-7](#GAS-7) | `internal` functions only called once can be inlined to save gas | 9 | 270 |
| [GAS-8](#GAS-8) | `keccak256()` hash of literals should only be computed once | 7 | 294 |
| [GAS-9](#GAS-9) | Low level `call` can be optimized with assembly | 2 | 496 |
| [GAS-10](#GAS-10) | Multiple accesses of the same mapping/array key/index should be cached | 19 | 798 |
| [GAS-11](#GAS-11) | Newer versions of solidity are more gas efficient | 6 | - |
| [GAS-12](#GAS-12) | Operator `>=`/`<=` costs less gas than operator `>`/`<` | 18 | 54 |
| [GAS-13](#GAS-13) | Reduce gas usage by moving to Solidity 0.8.19 or later | 6 | 6000 |
| [GAS-14](#GAS-14) | Redundant state variable getters | 1 | - |
| [GAS-15](#GAS-15) | Remove or replace unused state variables | 1 | - |
| [GAS-16](#GAS-16) | `require()`/`revert()` strings longer than 32 bytes cost extra gas | 3 | 9 |
| [GAS-17](#GAS-17) | The result of a function call should be cached rather than re-calling the function | 13 | 1300 |
| [GAS-18](#GAS-18) | Unlimited gas consumption risk due to external call recipients | 2 | - |
| [GAS-19](#GAS-19) | Unused named return variables without optimizer waste gas | 3 | 27 |
| [GAS-20](#GAS-20) | Use assembly to compute hashes to save gas | 10 | 800 |
| [GAS-21](#GAS-21) | Use assembly to emit events | 20 | 760 |
| [GAS-22](#GAS-22) | Using a double `if` statement instead of a logical AND (`&&`) | 2 | 60 |
| [GAS-23](#GAS-23) | Use a more recent version of solidity | 6 | - |
| [GAS-24](#GAS-24) | Use `storage` instead of `memory` for structs/arrays | 8 | 33600 |
| [GAS-25](#GAS-25) | Use `unchecked` block for safe subtractions | 4 | 340 |
| [GAS-26](#GAS-26) | Using bitmap to store bool states can save gas | 2 | - |
| [GAS-27](#GAS-27) | `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants) | 2 | - |
| [GAS-28](#GAS-28) | Using bools for storage incurs overhead | 2 | - |
| [GAS-29](#GAS-29) | Cache array length outside of loop | 5 | - |
| [GAS-30](#GAS-30) | State variables should be cached in stack variables rather than re-reading them from storage | 4 | 388 |
| [GAS-31](#GAS-31) | Use `calldata` instead of `memory` for function arguments that do not get mutated | 1 | - |
| [GAS-32](#GAS-32) | Use Custom Errors | 21 | 1050 |
| [GAS-33](#GAS-33) | Don't initialize variables with default value | 8 | - |
| [GAS-34](#GAS-34) | Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead | 1 | 55 |
| [GAS-35](#GAS-35) | Constructors can be marked as `payable` to save deployment gas | 2 | 42 |
| [GAS-36](#GAS-36) | Functions guaranteed to revert when called by normal users can be marked `payable` | 14 | 294 |
| [GAS-37](#GAS-37) | `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too) | 1 | 5 |
| [GAS-38](#GAS-38) | Using `private` rather than `public` for constants, saves gas | 12 | - |
| [GAS-39](#GAS-39) | Use `!= 0` instead of `> 0` for unsigned integer comparison | 3 | 12 |
| [GAS-40](#GAS-40) | Using assembly to check for zero can save gas | 16 | 96 |

## Medium Issues

<a name="M-1"></a> 
### [M-1] The remaining ETH may be locked in the contract after call
After calling an external contract and forwards some ETH value, the contract balance should be checked. If there is excess eth left over due to a failed call, or more eth being delivered than needed, or any other reason, this eth must be refunded to the user or handled appropriately, otherwise the eth may be frozen in the contract forever.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

180:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L180](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L180) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L131](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L131) 

</details>

---

<a name="M-2"></a> 
### [M-2] Return values of `transfer()`/`transferFrom()` not checked
Not all ERC20 implementations `revert()` when there's a failure in `transfer()` or `transferFrom()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually transfer anything.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

324:     IRWALike(_token).transfer(owner(), balance);

```
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

437:     usdy.transferFrom(msg.sender, address(this), _USDYAmount);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L437](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L437) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="M-3"></a> 
### [M-3] Unsafe use of ERC20 `transfer()`/`transferFrom()`
Some tokens do not implement the ERC20 standard properly. For example Tether (USDT)'s `transfer()` and `transferFrom()` functions do not return booleans as the ERC20 specification requires, and instead have no return value. When these sorts of tokens are cast to IERC20/ERC20, their function signatures do not match and therefore the calls made will revert.It is recommended to use the [`SafeERC20`](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/f347b410cf6aeeaaf5197e1fece139c793c03b2b/contracts/token/ERC20/utils/SafeERC20.sol#L19)'s `safeTransfer()` and `safeTransferFrom()` from OpenZeppelin instead.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

324:     IRWALike(_token).transfer(owner(), balance);

```
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

437:     usdy.transferFrom(msg.sender, address(this), _USDYAmount);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L437](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L437) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="M-4"></a> 
### [M-4] Centralization Risk for trusted owners
Contracts have owners with privileged rights to perform admin tasks and need to be trusted to not perform malicious updates or drain funds.

<details>
<summary>
There are <b>29</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

30:   Ownable,

210:   function addApprover(address approver) external onlyOwner {

220:   function removeApprover(address approver) external onlyOwner {

237:   ) external onlyOwner {

259:   ) external onlyOwner {

286:   function setMintLimit(uint256 mintLimit) external onlyOwner {

295:   function setMintLimitDuration(uint256 mintDuration) external onlyOwner {

304:   function pause() external onlyOwner {

313:   function unpause() external onlyOwner {

322:   function rescueTokens(address _token) external onlyOwner {

```
[#L30](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L30) [#L210](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L210) [#L220](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L220) [#L237](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L237) [#L259](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L259) [#L286](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L286) [#L295](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L295) [#L304](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L304) [#L313](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L313) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L322) 

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

139:   ) external onlyOwner {

151:   function pause() external onlyOwner {

160:   function unpause() external onlyOwner {

177:   ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) [#L139](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L139) [#L151](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L151) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L160) [#L177](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L177) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

140:   ) external onlyRole(SETTER_ROLE) {

178:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L8](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L8) [#L140](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L140) [#L178](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L178) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L227) [#L234](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L234) 

```solidity
File: contracts/usdy/rUSDY.sol

662:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

675:   ) external onlyRole(BURNER_ROLE) {

685:   function pause() external onlyRole(PAUSER_ROLE) {

689:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

700:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

711:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

722:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```
[#L662](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L662) [#L675](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L675) [#L685](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L685) [#L689](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L689) [#L700](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L700) [#L711](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L711) [#L722](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L722) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

81:   ) external onlyGuardian returns (address, address, address) {

128:   ) external payable override onlyGuardian returns (bytes[] memory results) {

```
[#L81](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L81) [#L128](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L128) 

</details>

---


## Low Issues

<a name="L-1"></a> 
### [L-1] Array is `push()`ed but not `pop()`ed
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

166:     t.approvers.push(msg.sender);

266:         chainToThresholds[srcChain].push(

273:         chainToThresholds[srcChain].push(

```
[#L166](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L166) [#L266](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L266) [#L273](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L273) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

31:     ranges.push(Range(firstRangeStart, firstRangeEnd, dailyIR, trueStart));

147:     ranges.push(

```
[#L31](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L31) [#L147](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L147) 

</details>

---

<a name="L-2"></a> 
### [L-2] Check division by zero is prevented

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

30:     uint256 trueStart = (startPrice * ONE) / dailyIR;

103:       uint256 trueStart = (rangeStartPrice * ONE) / dailyIR;

205:       uint256 trueStart = (newPrevRangeClosePrice * ONE) / newDailyIR;

252:     uint256 elapsedDays = (currentTime - currentRange.start) / DAY;

387:     z = _mul(x, y) / ONE;

391:     require(y == 0 || (z = x * y) / y == x);

```
[#L30](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L30) [#L103](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L103) [#L205](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L205) [#L252](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L252) [#L387](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L387) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L391) 

```solidity
File: contracts/usdy/rUSDY.sol

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

391:     return (_rUSDYAmount * 1e18 * BPS_DENOMINATOR) / oracle.getPrice();

398:     return (_shares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L217](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L217) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L391) [#L398](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L398) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="L-3"></a> 
### [L-3] Consider implementing two-step procedure for updating protocol addresses
A copy-paste error or a typo may end up bricking protocol functionality, or sending tokens to an address with no known private key. Consider implementing a two-step procedure for updating protocol addresses, where the recipient is set as pending, and must "accept" the assignment by making an affirmative call. A straight forward way of doing this would be to have the target contracts implement [EIP-165](https://eips.ethereum.org/EIPS/eip-165), and to have the "set" functions ensure that the recipient is of the right interface type.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

662:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

698:   function setBlocklist(

709:   function setAllowlist(

720:   function setSanctionsList(

```
[#L662](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L662) [#L698](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L698) [#L709](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L709) [#L720](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L720) 

</details>

---

<a name="L-4"></a> 
### [L-4] Constructor / initialization function lacks parameter validation
Constructors and initialization functions play a critical role in contracts by setting important initial states when the contract is first deployed before the system starts. The parameters passed to the constructor and initialization functions directly affect the behavior of the contract / protocol. If incorrect parameters are provided, the system may fail to run, behave abnormally, be unstable, or lack security. Therefore, it's crucial to carefully check each parameter in the constructor and initialization functions. If an exception is found, the transaction should be rolled back.

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `_token` not validated
/// `_axelarGateway` not validated
/// `_allowlist` not validated
/// `_ondoApprover` not validated
/// `_owner` not validated
/// `_mintLimit` not validated
/// `_mintDuration` not validated
55:   constructor(
        address _token,
        address _axelarGateway,
        address _allowlist,
        address _ondoApprover,
        address _owner,
        uint256 _mintLimit,
        uint256 _mintDuration
      )
        AxelarExecutable(_axelarGateway)
        MintTimeBasedRateLimiter(_mintDuration, _mintLimit)
      {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L55) 

```solidity
File: contracts/bridge/SourceBridge.sol

/// `_token` not validated
/// `_axelarGateway` not validated
/// `_gasService` not validated
/// `owner` not validated
55:   constructor(
        address _token,
        address _axelarGateway,
        address _gasService,
        address owner
      ) {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L55) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `admin` not validated
/// `setter` not validated
/// `pauser` not validated
/// `dailyIR` not validated
/// `startPrice` not validated
16:   constructor(
        address admin,
        address setter,
        address pauser,
        uint256 firstRangeStart,
        uint256 firstRangeEnd,
        uint256 dailyIR,
        uint256 startPrice
      ) {

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L16) 

```solidity
File: contracts/usdy/rUSDY.sol

/// `blocklist` not validated
/// `allowlist` not validated
/// `sanctionsList` not validated
/// `_usdy` not validated
/// `guardian` not validated
/// `_oracle` not validated
109:   function initialize(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) public virtual initializer {

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L109) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// `_guardian` not validated
51:   constructor(address _guardian) {

```
[#L51](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L51) 

</details>

---

<a name="L-5"></a> 
### [L-5] Enum values should be used instead of constant array indexes
Create a commented enum value to use instead of constant array indexes, this makes the code far easier to understand.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

345:           ALLOWLIST.getValidTermIndexes()[0],

```
[#L345](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L345) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

102:     if (startTime == ranges[0].start) {

```
[#L102](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L102) 

</details>

---

<a name="L-6"></a> 
### [L-6] External call recipient can consume all remaining gas
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

180:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L180](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L180) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L131](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L131) 

</details>

---

<a name="L-7"></a> 
### [L-7] Governance functions should be controlled by time locks
Governance functions (such as upgrading contracts, setting critical parameters) should be controlled using time locks to introduce a delay between a proposal and its execution. This gives users time to exit before a potentially dangerous or malicious operation is applied.

<details>
<summary>
There are <b>29</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

30:   Ownable,

210:   function addApprover(address approver) external onlyOwner {

220:   function removeApprover(address approver) external onlyOwner {

237:   ) external onlyOwner {

259:   ) external onlyOwner {

286:   function setMintLimit(uint256 mintLimit) external onlyOwner {

295:   function setMintLimitDuration(uint256 mintDuration) external onlyOwner {

304:   function pause() external onlyOwner {

313:   function unpause() external onlyOwner {

322:   function rescueTokens(address _token) external onlyOwner {

```
[#L30](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L30) [#L210](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L210) [#L220](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L220) [#L237](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L237) [#L259](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L259) [#L286](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L286) [#L295](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L295) [#L304](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L304) [#L313](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L313) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L322) 

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

139:   ) external onlyOwner {

151:   function pause() external onlyOwner {

160:   function unpause() external onlyOwner {

177:   ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) [#L139](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L139) [#L151](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L151) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L160) [#L177](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L177) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

140:   ) external onlyRole(SETTER_ROLE) {

178:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L8](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L8) [#L140](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L140) [#L178](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L178) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L227) [#L234](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L234) 

```solidity
File: contracts/usdy/rUSDY.sol

662:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

675:   ) external onlyRole(BURNER_ROLE) {

685:   function pause() external onlyRole(PAUSER_ROLE) {

689:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

700:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

711:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

722:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```
[#L662](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L662) [#L675](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L675) [#L685](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L685) [#L689](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L689) [#L700](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L700) [#L711](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L711) [#L722](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L722) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

81:   ) external onlyGuardian returns (address, address, address) {

128:   ) external payable override onlyGuardian returns (bytes[] memory results) {

```
[#L81](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L81) [#L128](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L128) 

</details>

---

<a name="L-8"></a> 
### [L-8] Loss of precision in divisions
Division by large numbers may result in the result being zero, due to solidity not supporting fractions. Consider requiring a minimum amount for the numerator to ensure that it is always larger than the denominator.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

30:     uint256 trueStart = (startPrice * ONE) / dailyIR;

103:       uint256 trueStart = (rangeStartPrice * ONE) / dailyIR;

205:       uint256 trueStart = (newPrevRangeClosePrice * ONE) / newDailyIR;

252:     uint256 elapsedDays = (currentTime - currentRange.start) / DAY;

387:     z = _mul(x, y) / ONE;

391:     require(y == 0 || (z = x * y) / y == x);

```
[#L30](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L30) [#L103](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L103) [#L205](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L205) [#L252](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L252) [#L387](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L387) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L391) 

```solidity
File: contracts/usdy/rUSDY.sol

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

391:     return (_rUSDYAmount * 1e18 * BPS_DENOMINATOR) / oracle.getPrice();

398:     return (_shares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L217](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L217) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L391) [#L398](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L398) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="L-9"></a> 
### [L-9] Missing contract existence checks before low-level calls
Low-level calls return success if there is no code present at the specified address. In addition to the zero-address checks, add a check to verify that `<address>.code.length > 0`

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

180:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L180](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L180) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L131](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L131) 

</details>

---

<a name="L-10"></a> 
### [L-10] Missing zero address check in constructor
Constructors often take address parameters to initialize important components of a contract, such as owner or linked contracts. However, without a checking, there's a risk that an address parameter could be mistakenly set to the zero address (0x0). This could be due to an error or oversight during contract deployment. A zero address in a crucial role can cause serious issues, as it cannot perform actions like a normal address, and any funds sent to it will be irretrievable. It's therefore crucial to include a zero address check in constructors to prevent such potential problems. If a zero address is detected, the constructor should revert the transaction.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// Missing zero check for `_token`
/// Missing zero check for `_axelarGateway`
/// Missing zero check for `_allowlist`
/// Missing zero check for `_ondoApprover`
/// Missing zero check for `_owner`
55:   constructor(
        address _token,
        address _axelarGateway,
        address _allowlist,
        address _ondoApprover,
        address _owner,
        uint256 _mintLimit,
        uint256 _mintDuration
      )
        AxelarExecutable(_axelarGateway)
        MintTimeBasedRateLimiter(_mintDuration, _mintLimit)
      {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L55) 

```solidity
File: contracts/bridge/SourceBridge.sol

/// Missing zero check for `_token`
/// Missing zero check for `_axelarGateway`
/// Missing zero check for `_gasService`
/// Missing zero check for `owner`
55:   constructor(
        address _token,
        address _axelarGateway,
        address _gasService,
        address owner
      ) {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L55) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Missing zero check for `admin`
/// Missing zero check for `setter`
/// Missing zero check for `pauser`
16:   constructor(
        address admin,
        address setter,
        address pauser,
        uint256 firstRangeStart,
        uint256 firstRangeEnd,
        uint256 dailyIR,
        uint256 startPrice
      ) {

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing zero check for `_guardian`
51:   constructor(address _guardian) {

```
[#L51](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L51) 

</details>

---

<a name="L-11"></a> 
### [L-11] Missing checks for `address(0)` when setting address state variables

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

52:     guardian = _guardian;

```
[#L52](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L52) 

</details>

---

<a name="L-12"></a> 
### [L-12] Missing storage gap for upgradable contracts
Each upgradable contract should include a state variable (usually named `__gap`) to provide reserved space in storage. This allows the team to freely add new state variables in the future upgrades without compromising the storage compatibility with existing deployments.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

57: contract rUSDY is
      Initializable,
      ContextUpgradeable,

```
[#L57](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L57) 

</details>

---

<a name="L-13"></a> 
### [L-13] Owner can renounce Ownership
Each of the following contracts implements or inherits the `renounceOwnership()` function. This can represent a certain risk if the ownership is renounced for any other reason than by design. Renouncing ownership will leave the contract without an owner, thereby removing any functionality that is only available to the owner.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

27: contract DestinationBridge is
      AxelarExecutable,
      MintTimeBasedRateLimiter,
      Ownable,

```
[#L27](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L27) 

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) 

</details>

---

<a name="L-14"></a> 
### [L-14] prevent re-setting a state variable with the same value
Not only is wasteful in terms of gas, but this is especially problematic when an event is emitted and the old and new values set are the same, as listeners might not expect this kind of scenario.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

139:     usdy = IUSDY(_usdy);

140:     oracle = IRWADynamicOracle(_oracle);

663:     oracle = IRWADynamicOracle(_oracle);

```
[#L139](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L139) [#L140](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L140) [#L663](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L663) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

52:     guardian = _guardian;

```
[#L52](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L52) 

</details>

---

<a name="L-15"></a> 
### [L-15] Some tokens may revert when large transfers are made
Tokens such as COMP or UNI will revert when an address' balance reaches `type(uint96).max`. Ensure that the calls below can be broken up into smaller batches if necessary.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

324:     IRWALike(_token).transfer(owner(), balance);

```
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="L-16"></a> 
### [L-16] Some tokens may revert when zero value transfers are made
Despite the fact that [EIP-20 states](https://github.com/ethereum/EIPs/blob/7500ac4fc1bbdfaf684e7ef851f798f6b667b2fe/EIPS/eip-20.md?plain=1#L116) that zero-value transfers must be accepted, some tokens, such as LEND, will revert if this is attempted, which may cause transactions that involve other tokens (such as batch operations) to fully revert. Consider skipping the transfer if the amount is zero, which will also save gas.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

324:     IRWALike(_token).transfer(owner(), balance);

```
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="L-17"></a> 
### [L-17] Timestamp may be manipulation
The `block.timestamp` can be manipulated by miners to perform MEV profiting or other time-based attacks.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

50:     timestamp = block.timestamp;

65:       if (range.start <= block.timestamp) {

66:         if (range.end <= block.timestamp) {

69:           return derivePrice(range, block.timestamp);

```
[#L50](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L50) [#L65](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L65) [#L66](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L66) [#L69](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L69) 

</details>

---

<a name="L-18"></a> 
### [L-18] Unsafe solidity low-level call can cause gas grief attack
Using the low-level calls of a solidity address can leave the contract open to gas grief attacks. These attacks occur when the called contract returns a large amount of data. So when calling an external contract, it is necessary to check the length of the return data before reading/copying it (using `returndatasize()`).

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

180:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L180](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L180) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L131](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L131) 

</details>

---

<a name="L-19"></a> 
### [L-19] Use Ownable2Step instead of Ownable
`Ownable2Step` and `Ownable2StepUpgradeable` prevent the contract ownership from mistakenly being transferred to an address that cannot handle it (e.g. due to a typo in the address), by requiring that the recipient of the owner permissions actively accept via a contract call of its own.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

27: contract DestinationBridge is
      AxelarExecutable,
      MintTimeBasedRateLimiter,
      Ownable,

```
[#L27](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L27) 

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) 

</details>

---

<a name="L-20"></a> 
### [L-20] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

438:     emit Transfer(address(0), msg.sender, getRUSDYByShares(_USDYAmount));

439:     emit TransferShares(address(0), msg.sender, _USDYAmount);

549:     _beforeTokenTransfer(address(0), _recipient, _sharesAmount);

581:     _beforeTokenTransfer(_account, address(0), _sharesAmount);

```
[#L438](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L438) [#L439](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L439) [#L549](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L549) [#L581](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L581) 

</details>

---

<a name="L-21"></a> 
### [L-21] Missing zero address check in initializer

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
109:   function initialize(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) public virtual initializer {

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L109) 

</details>

---

<a name="L-22"></a> 
### [L-22] Initializers could be front-run
Initializers could be front-run, allowing an attacker to either set their own values, take ownership of the contract, and in the best case forcing a re-deployment

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

109:   function initialize(

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L109) 

</details>

---


## Non Critical Issues

<a name="NC-1"></a> 
### [NC-1] `assert()` should be replaced with `require()` or `revert()`
In versions of Solidity prior to 0.8.0, when encountering an assert all the remaining gas will be consumed. Even after solidity 0.8.0, the assert function is still not recommended, as described in the [documentation](https://docs.soliditylang.org/en/v0.8.20/control-structures.html#panic-via-assert-and-error-via-require):
> Assert should only be used to test for internal errors, and to check invariants. Properly functioning code should never create a Panic, not even on invalid external input. If this happens, then there is a bug in your contract which you should fix.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

100:     assert(rUSDYProxyAdmin.owner() == guardian);

```
[#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L100) 

</details>

---

<a name="NC-2"></a> 
### [NC-2] Contract declarations should have NatSpec `@author` annotations

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

18: interface IRWADynamicOracle {

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L18) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```
[#L8](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L8) 

</details>

---

<a name="NC-3"></a> 
### [NC-3] Consider adding formal verification proofs
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

<a name="NC-4"></a> 
### [NC-4] Consider bounding input array length
The functions below take in an unbounded array, and make function calls for entries in the array. While the function will revert if it eventually runs out of gas, it may be a nicer user experience to require() that the length of the array is below some reasonable maximum, so that the user doesn't have to use up a full transaction's gas only to see that the transaction reverts.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

/// Consider length check for `exCallData`
179:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L179) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Consider length check for `exCallData`
130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="NC-5"></a> 
### [NC-5] Constants should be put on the left side of comparisons
Putting constants on the left side of comparison statements is a best practice known as [Yoda conditions](https://en.wikipedia.org/wiki/Yoda_conditions). Although solidity's static typing system prevents accidental assignments within conditionals, adopting this practice can improve code readability and consistency, especially when working across multiple languages.

<details>
<summary>
There are <b>16</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

144:     if (txnToThresholdSet[txnHash].numberOfApprovalsNeeded == 0) {

265:       if (i == 0) {

```
[#L144](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L144) [#L265](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L265) 

```solidity
File: contracts/bridge/SourceBridge.sol

83:     if (bytes(destContract).length == 0) {

87:     if (msg.value == 0) {

```
[#L83](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L83) [#L87](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L87) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

184:     if (indexToModify == 0) {

204:     if (indexToModify == 0) {

270:     if (remainder >= 0.5e10) {

391:     require(y == 0 || (z = x * y) / y == x);

```
[#L184](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L184) [#L204](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L204) [#L270](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L270) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L391) 

```solidity
File: contracts/usdy/rUSDY.sol

490:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

491:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

519:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

520:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

547:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

579:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

642:     if (from != address(0)) {

649:     if (to != address(0)) {

```
[#L490](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L490) [#L491](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L491) [#L519](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L519) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L520) [#L547](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L547) [#L579](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L579) [#L642](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L642) [#L649](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L649) 

</details>

---

<a name="NC-6"></a> 
### [NC-6] Contract name does not follow the Solidity Style Guide
According to the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html#contract-and-library-names), contracts and libraries should be named using the CapWords style and match their filenames.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

57: contract rUSDY is

```
[#L57](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L57) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

43: contract rUSDYFactory is IMulticall {

```
[#L43](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L43) 

</details>

---

<a name="NC-7"></a> 
### [NC-7] Contract uses both `require()`/`revert()` as well as custom errors
Consider using just one method in a single file.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```
[#L8](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L8) 

```solidity
File: contracts/usdy/rUSDY.sol

57: contract rUSDY is

```
[#L57](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L57) 

</details>

---

<a name="NC-8"></a> 
### [NC-8] Contracts should have full test coverage
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

<a name="NC-9"></a> 
### [NC-9] Events that mark critical parameter changes should contain both the old and the new value
This should especially be done if the new value is not required to be different from the old value.

<details>
<summary>
There are <b>16</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

113:     emit MessageReceived(srcChain, srcSender, amt, nonce);

212:     emit ApproverAdded(approver);

222:     emit ApproverRemoved(approver);

239:     emit ChainIdSupported(srcChain, srcContractAddress);

278:     emit ThresholdSet(srcChain, amounts, numOfApprovers);

351:       emit BridgeCompleted(txn.sender, txn.amount);

```
[#L113](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L113) [#L212](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L212) [#L222](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L222) [#L239](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L239) [#L278](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L278) [#L351](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L351) 

```solidity
File: contracts/bridge/SourceBridge.sol

143:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```
[#L143](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L143) 

```solidity
File: contracts/usdy/rUSDY.sol

421:     emit TransferShares(msg.sender, _recipient, _sharesAmount);

423:     emit Transfer(msg.sender, _recipient, tokensAmount);

438:     emit Transfer(address(0), msg.sender, getRUSDYByShares(_USDYAmount));

439:     emit TransferShares(address(0), msg.sender, _USDYAmount);

455:     emit TokensBurnt(msg.sender, _rUSDYAmount);

470:     emit Transfer(_sender, _recipient, _amount);

471:     emit TransferShares(_sender, _recipient, _sharesToTransfer);

494:     emit Approval(_owner, _spender, _amount);

682:     emit TokensBurnt(_account, _amount);

```
[#L421](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L421) [#L423](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L423) [#L438](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L438) [#L439](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L439) [#L455](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L455) [#L470](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L470) [#L471](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L471) [#L494](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L494) [#L682](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L682) 

</details>

---

<a name="NC-10"></a> 
### [NC-10] Custom errors has no error details
Consider adding parameters to the error to indicate which user or values caused the failure.

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

439:   error NotApprover();

440:   error NoThresholdMatch();

441:   error ThresholdsNotInAscendingOrder();

443:   error ChainNotSupported();

444:   error SourceNotSupported();

445:   error NonceSpent();

446:   error AlreadyApproved();

447:   error InvalidVersion();

448:   error ArrayLengthMismatch();

```
[#L439](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L439) [#L440](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L440) [#L441](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L441) [#L443](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L443) [#L444](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L444) [#L445](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L445) [#L446](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L446) [#L447](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L447) [#L448](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L448) 

```solidity
File: contracts/bridge/SourceBridge.sol

204:   error DestinationNotSupported();

205:   error GasFeeTooLow();

```
[#L204](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L204) [#L205](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L205) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

320:   error InvalidPrice();

321:   error InvalidRange();

322:   error PriceNotSet();

```
[#L320](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L320) [#L321](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L321) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L322) 

```solidity
File: contracts/usdy/rUSDY.sol

94:   error UnwrapTooSmall();

```
[#L94](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L94) 

</details>

---

<a name="NC-11"></a> 
### [NC-11] Custom errors should be used rather than `revert()`/`require()`
Custom errors are available from solidity version 0.8.4. Custom errors are more easily processed in try-catch blocks, and are easier to re-use and maintain.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

183:       require(success, "Call Failed");

```
[#L183](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L183) 

```solidity
File: contracts/usdy/rUSDY.sol

307:     require(currentAllowance >= _amount, "TRANSFER_AMOUNT_EXCEEDS_ALLOWANCE");

435:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

490:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

491:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

519:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

520:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

547:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

579:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

584:     require(_sharesAmount <= accountShares, "BURN_AMOUNT_EXCEEDS_BALANCE");

634:       require(!_isBlocked(msg.sender), "rUSDY: 'sender' address blocked");

635:       require(!_isSanctioned(msg.sender), "rUSDY: 'sender' address sanctioned");

644:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");

645:       require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

646:       require(_isAllowed(from), "rUSDY: 'from' address not on allowlist");

651:       require(!_isBlocked(to), "rUSDY: 'to' address blocked");

652:       require(!_isSanctioned(to), "rUSDY: 'to' address sanctioned");

653:       require(_isAllowed(to), "rUSDY: 'to' address not on allowlist");

```
[#L307](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L307) [#L435](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L450) [#L490](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L490) [#L491](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L491) [#L519](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L519) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L520) [#L547](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L547) [#L579](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L579) [#L584](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L584) [#L634](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L634) [#L635](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L635) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L644) [#L645](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L645) [#L646](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L646) [#L651](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L651) [#L652](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L652) [#L653](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L653) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

134:       require(success, "Call Failed");

155:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L134) [#L155](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L155) 

</details>

---

<a name="NC-12"></a> 
### [NC-12] `else` block not required
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

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

179:     if (t.numberOfApprovalsNeeded <= t.approvers.length) {
           return true;
         } else {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L179) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

66:         if (range.end <= block.timestamp) {
              return derivePrice(range, range.end - 1);
            } else {

118:         if (range.end <= blockTimeStamp) {
               return derivePrice(range, range.end - 1);
             } else {

```
[#L66](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L66) [#L118](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L118) 

</details>

---

<a name="NC-13"></a> 
### [NC-13] Enable IR-based code generation
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

<a name="NC-14"></a> 
### [NC-14] Names of structs, events, enums and errors should use CapWords style
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html)

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

146:   event rUSDYDeployed(

```
[#L146](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L146) 

</details>

---

<a name="NC-15"></a> 
### [NC-15] Events are emitted without the sender information
When an action is triggered based on a user's action, not being able to filter based on who triggered the action makes event processing a lot more cumbersome. Including the `msg.sender` the events of these types of action will make events much more useful to end users, especially when `msg.sender` is not `tx.origin`.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

113:     emit MessageReceived(srcChain, srcSender, amt, nonce);

212:     emit ApproverAdded(approver);

222:     emit ApproverRemoved(approver);

239:     emit ChainIdSupported(srcChain, srcContractAddress);

278:     emit ThresholdSet(srcChain, amounts, numOfApprovers);

```
[#L113](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L113) [#L212](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L212) [#L222](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L222) [#L239](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L239) [#L278](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L278) 

```solidity
File: contracts/bridge/SourceBridge.sol

143:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```
[#L143](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L143) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

150:     emit RangeSet(

215:     emit RangeOverriden(

```
[#L150](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L150) [#L215](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L215) 

```solidity
File: contracts/usdy/rUSDY.sol

470:     emit Transfer(_sender, _recipient, _amount);

471:     emit TransferShares(_sender, _recipient, _sharesToTransfer);

494:     emit Approval(_owner, _spender, _amount);

594:     emit SharesBurnt(

682:     emit TokensBurnt(_account, _amount);

```
[#L470](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L470) [#L471](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L471) [#L494](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L494) [#L594](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L594) [#L682](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L682) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

101:     emit rUSDYDeployed(

```
[#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L101) 

</details>

---

<a name="NC-16"></a> 
### [NC-16] Import declarations should import specific identifiers, rather than the whole file
Using import declarations of the form `import {<identifier_name>} from "some/file.sol"` avoids polluting the symbol namespace making flattened files smaller, and speeds up compilation (but does not save any gas).

<details>
<summary>
There are <b>32</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

18: import "contracts/interfaces/IAxelarGateway.sol";

19: import "contracts/interfaces/IAxelarGasService.sol";

20: import "contracts/external/axelar/AxelarExecutable.sol";

21: import "contracts/interfaces/IRWALike.sol";

22: import "contracts/interfaces/IAllowlist.sol";

23: import "contracts/external/openzeppelin/contracts/access/Ownable.sol";

24: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

25: import "contracts/bridge/MintRateLimiter.sol";

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L18) [#L19](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L20) [#L21](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L21) [#L22](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L22) [#L23](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L23) [#L24](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L24) [#L25](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L25) 

```solidity
File: contracts/bridge/SourceBridge.sol

18: import "contracts/interfaces/IAxelarGateway.sol";

19: import "contracts/interfaces/IAxelarGasService.sol";

20: import "contracts/interfaces/IMulticall.sol";

21: import "contracts/interfaces/IRWALike.sol";

23: import "contracts/external/openzeppelin/contracts/access/Ownable.sol";

24: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L18) [#L19](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L20) [#L21](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L21) [#L23](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L23) [#L24](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L24) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

4: import "contracts/rwaOracles/IRWAOracle.sol";

5: import "contracts/external/openzeppelin/contracts/access/AccessControlEnumerable.sol";

6: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

```
[#L4](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L4) [#L5](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L5) [#L6](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L6) 

```solidity
File: contracts/usdy/rUSDY.sol

18: import "contracts/external/openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol";

19: import "contracts/external/openzeppelin/contracts-upgradeable/token/ERC20/IERC20MetadataUpgradeable.sol";

20: import "contracts/external/openzeppelin/contracts-upgradeable/proxy/Initializable.sol";

21: import "contracts/external/openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol";

22: import "contracts/external/openzeppelin/contracts-upgradeable/security/PausableUpgradeable.sol";

23: import "contracts/external/openzeppelin/contracts-upgradeable/access/AccessControlEnumerableUpgradeable.sol";

24: import "contracts/usdy/blocklist/BlocklistClientUpgradeable.sol";

25: import "contracts/usdy/allowlist/AllowlistClientUpgradeable.sol";

26: import "contracts/sanctions/SanctionsListClientUpgradeable.sol";

27: import "contracts/interfaces/IUSDY.sol";

28: import "contracts/rwaOracles/IRWADynamicOracle.sol";

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L18) [#L19](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L20) [#L21](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L21) [#L22](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L22) [#L23](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L23) [#L24](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L24) [#L25](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L25) [#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L26) [#L27](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L27) [#L28](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L28) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

19: import "contracts/external/openzeppelin/contracts/proxy/ProxyAdmin.sol";

20: import "contracts/Proxy.sol";

21: import "contracts/usdy/rUSDY.sol";

22: import "contracts/interfaces/IMulticall.sol";

```
[#L19](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L20) [#L21](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L21) [#L22](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L22) 

</details>

---

<a name="NC-17"></a> 
### [NC-17] Large or complicated code bases should implement invariant tests
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

<a name="NC-18"></a> 
### [NC-18] Large multiples of ten should use scientific notation
Use a scientific notation rather than decimal literals (e.g. `1e6` instead of `1000000`), for better code readability.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

```
[#L91](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L91) 

</details>

---

<a name="NC-19"></a> 
### [NC-19] Magic numbers should be replaced with constants
Magic numbers are hard-coded values in code that can make it difficult for developers and maintainers to understand the code, and can also cause confusion or errors. To improve the readability and maintainability of code, it is recommended to replace magic numbers with constants that have good readability.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

269:     uint256 remainder = value % 1e10;

270:     if (remainder >= 0.5e10) {

271:       value += 1e10;

```
[#L269](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L269) [#L270](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L270) [#L271](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L271) 

```solidity
File: contracts/usdy/rUSDY.sol

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

391:     return (_rUSDYAmount * 1e18 * BPS_DENOMINATOR) / oracle.getPrice();

398:     return (_shares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

```
[#L217](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L217) [#L217](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L217) [#L217](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L217) [#L217](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L217) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L391) [#L398](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L398) 

</details>

---

<a name="NC-20"></a> 
### [NC-20] Missing zero address check in functions with address parameters
Adding a zero address check for each address type parameter can prevent errors.

<details>
<summary>
There are <b>23</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// Missing zero check for `_token`
/// Missing zero check for `_axelarGateway`
/// Missing zero check for `_allowlist`
/// Missing zero check for `_ondoApprover`
/// Missing zero check for `_owner`
55:   constructor(
        address _token,
        address _axelarGateway,
        address _allowlist,
        address _ondoApprover,
        address _owner,
        uint256 _mintLimit,
        uint256 _mintDuration
      )
        AxelarExecutable(_axelarGateway)
        MintTimeBasedRateLimiter(_mintDuration, _mintLimit)
      {

/// Missing zero check for `approver`
210:   function addApprover(address approver) external onlyOwner {

/// Missing zero check for `approver`
220:   function removeApprover(address approver) external onlyOwner {

/// Missing zero check for `_token`
322:   function rescueTokens(address _token) external onlyOwner {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L55) [#L210](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L210) [#L220](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L220) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L322) 

```solidity
File: contracts/bridge/SourceBridge.sol

/// Missing zero check for `_token`
/// Missing zero check for `_axelarGateway`
/// Missing zero check for `_gasService`
/// Missing zero check for `owner`
55:   constructor(
        address _token,
        address _axelarGateway,
        address _gasService,
        address owner
      ) {

/// Missing zero check for `contractAddress`
136:   function setDestinationChainContractAddress(
         string memory destinationChain,
         address contractAddress
       ) external onlyOwner {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L55) [#L136](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L136) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Missing zero check for `admin`
/// Missing zero check for `setter`
/// Missing zero check for `pauser`
16:   constructor(
        address admin,
        address setter,
        address pauser,
        uint256 firstRangeStart,
        uint256 firstRangeEnd,
        uint256 dailyIR,
        uint256 startPrice
      ) {

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L16) 

```solidity
File: contracts/usdy/rUSDY.sol

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
109:   function initialize(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) public virtual initializer {

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
120:   function __rUSDY_init(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
134:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing zero check for `_account`
226:   function balanceOf(address _account) public view returns (uint256) {

/// Missing zero check for `_recipient`
245:   function transfer(address _recipient, uint256 _amount) public returns (bool) {

/// Missing zero check for `_spender`
276:   function approve(address _spender, uint256 _amount) public returns (bool) {

/// Missing zero check for `_account`
381:   function sharesOf(address _account) public view returns (uint256) {

/// Missing zero check for `_sender`
/// Missing zero check for `_recipient`
463:   function _transfer(
         address _sender,
         address _recipient,
         uint256 _amount
       ) internal {

/// Missing zero check for `_account`
500:   function _sharesOf(address _account) internal view returns (uint256) {

/// Missing zero check for `_oracle`
662:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

/// Missing zero check for `_account`
672:   function burn(
         address _account,
         uint256 _amount
       ) external onlyRole(BURNER_ROLE) {

/// Missing zero check for `blocklist`
698:   function setBlocklist(
         address blocklist
       ) external override onlyRole(LIST_CONFIGURER_ROLE) {

/// Missing zero check for `allowlist`
709:   function setAllowlist(
         address allowlist
       ) external override onlyRole(LIST_CONFIGURER_ROLE) {

/// Missing zero check for `sanctionsList`
720:   function setSanctionsList(
         address sanctionsList
       ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L109) [#L120](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L120) [#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L134) [#L226](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L226) [#L245](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L245) [#L276](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L276) [#L381](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L381) [#L463](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L463) [#L500](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L500) [#L662](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L662) [#L672](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L672) [#L698](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L698) [#L709](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L709) [#L720](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L720) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing zero check for `_guardian`
51:   constructor(address _guardian) {

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `usdy`
/// Missing zero check for `oracle`
75:   function deployrUSDY(
        address blocklist,
        address allowlist,
        address sanctionsList,
        address usdy,
        address oracle
      ) external onlyGuardian returns (address, address, address) {

```
[#L51](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L51) [#L75](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L75) 

</details>

---

<a name="NC-21"></a> 
### [NC-21] Consider moving `msg.sender` checks to `modifier`s
If some functions are only allowed to be called by some specific users, consider using a modifier instead of checking with a require statement, especially if this check is done in multiple functions.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

634:       require(!_isBlocked(msg.sender), "rUSDY: 'sender' address blocked");

635:       require(!_isSanctioned(msg.sender), "rUSDY: 'sender' address sanctioned");

```
[#L634](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L634) [#L635](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L635) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

155:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```
[#L155](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L155) 

</details>

---

<a name="NC-22"></a> 
### [NC-22] Named mappings are recommended
[Named mappings](https://docs.soliditylang.org/en/v0.8.18/types.html#mapping-types) (with syntax `mapping(KeyType KeyName? => ValueType ValueName?)`) are recommended.It can make the mapping variables clearer, more readable and easier to maintain.

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

43:   mapping(address => bool) public approvers;

44:   mapping(string => bytes32) public chainToApprovedSender;

45:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

51:   mapping(bytes32 => TxnThreshold) public txnToThresholdSet;

52:   mapping(string => Threshold[]) public chainToThresholds;

53:   mapping(bytes32 => Transaction) public txnHashToTransaction;

```
[#L43](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L43) [#L44](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L44) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L45) [#L51](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L51) [#L52](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L52) [#L53](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L53) 

```solidity
File: contracts/bridge/SourceBridge.sol

30:   mapping(string => string) public destChainToContractAddr;

```
[#L30](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L30) 

```solidity
File: contracts/usdy/rUSDY.sol

76:   mapping(address => uint256) private shares;

79:   mapping(address => mapping(address => uint256)) private allowances;

```
[#L76](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L76) [#L79](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L79) 

</details>

---

<a name="NC-23"></a> 
### [NC-23] NatSpec documentation for contract is missing
e.g. `@dev` or `@notice`, and it must appear above the contract definition braces in order to be identified by the compiler as NatSpec.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

18: interface IRWADynamicOracle {

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L18) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```
[#L8](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L8) 

</details>

---

<a name="NC-24"></a> 
### [NC-24] NatSpec documentation for function is missing
It is recommended that Solidity contracts are fully annotated using NatSpec for all public interfaces (everything in the ABI). It is clearly stated in the Solidity official documentation. In complex projects such as DeFi, the interpretation of all functions and their arguments and returns is important for code readability and auditability.

<details>
<summary>
There are <b>11</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

55:   constructor(
        address _token,
        address _axelarGateway,
        address _allowlist,
        address _ondoApprover,
        address _owner,
        uint256 _mintLimit,
        uint256 _mintDuration
      )
        AxelarExecutable(_axelarGateway)
        MintTimeBasedRateLimiter(_mintDuration, _mintLimit)
      {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L55) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

16:   constructor(
        address admin,
        address setter,
        address pauser,
        uint256 firstRangeStart,
        uint256 firstRangeEnd,
        uint256 dailyIR,
        uint256 startPrice
      ) {

331:   function _rpow(
         uint256 x,
         uint256 n,
         uint256 base
       ) internal pure returns (uint256 z) {

386:   function _rmul(uint256 x, uint256 y) internal pure returns (uint256 z) {

390:   function _mul(uint256 x, uint256 y) internal pure returns (uint256 z) {

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L16) [#L331](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L331) [#L386](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L386) [#L390](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L390) 

```solidity
File: contracts/usdy/rUSDY.sol

109:   function initialize(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) public virtual initializer {

120:   function __rUSDY_init(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

134:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

685:   function pause() external onlyRole(PAUSER_ROLE) {

689:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L109) [#L120](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L120) [#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L134) [#L685](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L685) [#L689](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L689) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

51:   constructor(address _guardian) {

```
[#L51](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L51) 

</details>

---

<a name="NC-25"></a> 
### [NC-25] Modifier declarations should have NatSpec descriptions

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

154:   modifier onlyGuardian() {

```
[#L154](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L154) 

</details>

---

<a name="NC-26"></a> 
### [NC-26] Missing NatSpec `@param`
Some functions have an incomplete NatSpec: add a `@param` notation to describe the function parameters to improve the code documentation.

<details>
<summary>
There are <b>28</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// Missing @param for _token
/// Missing @param for _axelarGateway
/// Missing @param for _allowlist
/// Missing @param for _ondoApprover
/// Missing @param for _owner
/// Missing @param for _mintLimit
/// Missing @param for _mintDuration
55:   constructor(
        address _token,
        address _axelarGateway,
        address _allowlist,
        address _ondoApprover,
        address _owner,
        uint256 _mintLimit,
        uint256 _mintDuration
      )
        AxelarExecutable(_axelarGateway)
        MintTimeBasedRateLimiter(_mintDuration, _mintLimit)
      {

```
[#L55](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L55) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Missing @param for admin
/// Missing @param for setter
/// Missing @param for pauser
/// Missing @param for firstRangeStart
/// Missing @param for firstRangeEnd
/// Missing @param for dailyIR
/// Missing @param for startPrice
16:   constructor(
        address admin,
        address setter,
        address pauser,
        uint256 firstRangeStart,
        uint256 firstRangeEnd,
        uint256 dailyIR,
        uint256 startPrice
      ) {

/// Missing @param for x
/// Missing @param for n
/// Missing @param for base
331:   function _rpow(
         uint256 x,
         uint256 n,
         uint256 base
       ) internal pure returns (uint256 z) {

/// Missing @param for x
/// Missing @param for y
386:   function _rmul(uint256 x, uint256 y) internal pure returns (uint256 z) {

/// Missing @param for x
/// Missing @param for y
390:   function _mul(uint256 x, uint256 y) internal pure returns (uint256 z) {

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L16) [#L331](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L331) [#L386](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L386) [#L390](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L390) 

```solidity
File: contracts/usdy/rUSDY.sol

/// Missing @param for blocklist
/// Missing @param for allowlist
/// Missing @param for sanctionsList
/// Missing @param for _usdy
/// Missing @param for guardian
/// Missing @param for _oracle
109:   function initialize(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) public virtual initializer {

/// Missing @param for blocklist
/// Missing @param for allowlist
/// Missing @param for sanctionsList
/// Missing @param for _usdy
/// Missing @param for guardian
/// Missing @param for _oracle
120:   function __rUSDY_init(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing @param for _usdy
/// Missing @param for guardian
/// Missing @param for _oracle
134:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing @param for _account
226:   function balanceOf(address _account) public view returns (uint256) {

/// Missing @param for _recipient
/// Missing @param for _amount
245:   function transfer(address _recipient, uint256 _amount) public returns (bool) {

/// Missing @param for _owner
/// Missing @param for _spender
256:   function allowance(
         address _owner,
         address _spender
       ) public view returns (uint256) {

/// Missing @param for _spender
/// Missing @param for _amount
276:   function approve(address _spender, uint256 _amount) public returns (bool) {

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _amount
301:   function transferFrom(
         address _sender,
         address _recipient,
         uint256 _amount
       ) public returns (bool) {

/// Missing @param for _spender
/// Missing @param for _addedValue
327:   function increaseAllowance(
         address _spender,
         uint256 _addedValue
       ) public returns (bool) {

/// Missing @param for _spender
/// Missing @param for _subtractedValue
353:   function decreaseAllowance(
         address _spender,
         uint256 _subtractedValue
       ) public returns (bool) {

/// Missing @param for _account
381:   function sharesOf(address _account) public view returns (uint256) {

/// Missing @param for _rUSDYAmount
388:   function getSharesByRUSDY(
         uint256 _rUSDYAmount
       ) public view returns (uint256) {

/// Missing @param for _shares
397:   function getRUSDYByShares(uint256 _shares) public view returns (uint256) {

/// Missing @param for _recipient
/// Missing @param for _sharesAmount
416:   function transferShares(
         address _recipient,
         uint256 _sharesAmount
       ) public returns (uint256) {

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _amount
463:   function _transfer(
         address _sender,
         address _recipient,
         uint256 _amount
       ) internal {

/// Missing @param for _owner
/// Missing @param for _spender
/// Missing @param for _amount
485:   function _approve(
         address _owner,
         address _spender,
         uint256 _amount
       ) internal whenNotPaused {

/// Missing @param for _account
500:   function _sharesOf(address _account) internal view returns (uint256) {

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _sharesAmount
514:   function _transferShares(
         address _sender,
         address _recipient,
         uint256 _sharesAmount
       ) internal whenNotPaused {

/// Missing @param for _recipient
/// Missing @param for _sharesAmount
543:   function _mintShares(
         address _recipient,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

/// Missing @param for _account
/// Missing @param for _sharesAmount
575:   function _burnShares(
         address _account,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

/// Missing @param for from
/// Missing @param for to
626:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L109) [#L120](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L120) [#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L134) [#L226](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L226) [#L245](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L245) [#L256](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L256) [#L276](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L276) [#L301](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L301) [#L327](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L327) [#L353](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L353) [#L381](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L381) [#L388](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L388) [#L397](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L397) [#L416](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L416) [#L463](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L463) [#L485](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L485) [#L500](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L500) [#L514](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L514) [#L543](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L543) [#L575](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L575) [#L626](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L626) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing @param for _guardian
51:   constructor(address _guardian) {

/// Missing @param for oracle
75:   function deployrUSDY(
        address blocklist,
        address allowlist,
        address sanctionsList,
        address usdy,
        address oracle
      ) external onlyGuardian returns (address, address, address) {

```
[#L51](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L51) [#L75](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L75) 

</details>

---

<a name="NC-27"></a> 
### [NC-27] Public variable declarations should have NatSpec descriptions

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

44:   mapping(string => bytes32) public chainToApprovedSender;

45:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

52:   mapping(string => Threshold[]) public chainToThresholds;

53:   mapping(bytes32 => Transaction) public txnHashToTransaction;

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L44) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L45) [#L52](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L52) [#L53](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L53) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

11:   Range[] public ranges;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) [#L11](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L11) [#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) 

```solidity
File: contracts/usdy/rUSDY.sol

85:   IRWADynamicOracle public oracle;

88:   IUSDY public usdy;

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L85](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L85) [#L88](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L88) [#L91](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L91) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L101) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

44:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

47:   rUSDY public rUSDYImplementation;

48:   ProxyAdmin public rUSDYProxyAdmin;

49:   TokenProxy public rUSDYProxy;

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L44) [#L47](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L47) [#L48](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L48) [#L49](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L49) 

</details>

---

<a name="NC-28"></a> 
### [NC-28] NatSpec `@return` is missing
It is recommended that Solidity contracts are fully annotated using NatSpec

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

177:   function _checkThresholdMet(bytes32 txnHash) internal view returns (bool) {

361:   function getNumApproved(bytes32 txnHash) external view returns (uint256) {

```
[#L177](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L177) [#L361](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L361) 

```solidity
File: contracts/bridge/SourceBridge.sol

175:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L175](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L175) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

20:   function getPrice() external view returns (uint256);

```
[#L20](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L20) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

90:   function simulateRange(
        uint256 blockTimeStamp,
        uint256 dailyIR,
        uint256 endTime,
        uint256 startTime,
        uint256 rangeStartPrice
      ) external view returns (uint256 price) {

248:   function derivePrice(
         Range memory currentRange,
         uint256 currentTime
       ) internal pure returns (uint256 price) {

268:   function roundUpTo8(uint256 value) internal pure returns (uint256) {

331:   function _rpow(
         uint256 x,
         uint256 n,
         uint256 base
       ) internal pure returns (uint256 z) {

386:   function _rmul(uint256 x, uint256 y) internal pure returns (uint256 z) {

390:   function _mul(uint256 x, uint256 y) internal pure returns (uint256 z) {

```
[#L90](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L90) [#L248](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L248) [#L268](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L268) [#L331](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L331) [#L386](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L386) [#L390](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L390) 

```solidity
File: contracts/usdy/rUSDY.sol

327:   function increaseAllowance(
         address _spender,
         uint256 _addedValue
       ) public returns (bool) {

353:   function decreaseAllowance(
         address _spender,
         uint256 _subtractedValue
       ) public returns (bool) {

543:   function _mintShares(
         address _recipient,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

575:   function _burnShares(
         address _account,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

```
[#L327](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L327) [#L353](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L353) [#L543](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L543) [#L575](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L575) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

126:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyGuardian returns (bytes[] memory results) {

```
[#L126](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L126) 

</details>

---

<a name="NC-29"></a> 
### [NC-29] There is no need to initialize variables with 0
Since the variables are automatically set to 0 when created, it is redundant to initialize it with 0 again.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

134:     for (uint256 i = 0; i < thresholds.length; ++i) {

160:       for (uint256 i = 0; i < t.approvers.length; ++i) {

264:     for (uint256 i = 0; i < amounts.length; ++i) {

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

179:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L179) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

63:     for (uint256 i = 0; i < length; ++i) {

99:     for (uint256 i = 0; i < length; ++i) {

115:     for (uint256 i = 0; i < length + 1; ++i) {

```
[#L63](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L63) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L99) [#L115](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L115) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="NC-30"></a> 
### [NC-30] Put all system-wide constants in one file
Putting all the system-wide constants in a single file improves code readability, makes it easier to understand the basic configuration and limitations of the system, and makes maintenance easier.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

48:   bytes32 public constant VERSION = "1.0";

```
[#L48](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L48) 

```solidity
File: contracts/bridge/SourceBridge.sol

42:   bytes32 public constant VERSION = "1.0";

```
[#L42](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L42) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

329:   uint256 private constant ONE = 10 ** 27;

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) [#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) [#L329](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L329) 

```solidity
File: contracts/usdy/rUSDY.sol

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L91](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L91) [#L97](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L101) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

44:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L44) 

</details>

---

<a name="NC-31"></a> 
### [NC-31] SPDX identifier should be the in the first line of a solidity file

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// SPDX-License-Identifier
1: 

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L1) 

```solidity
File: contracts/bridge/SourceBridge.sol

/// SPDX-License-Identifier
1: 

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L1) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

/// SPDX-License-Identifier
1: 

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L1) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// SPDX-License-Identifier
1: 

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L1) 

```solidity
File: contracts/usdy/rUSDY.sol

/// SPDX-License-Identifier
1: 

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L1) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// SPDX-License-Identifier
1: 

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L1) 

</details>

---

<a name="NC-32"></a> 
### [NC-32] State variables should include comments
Consider adding some comments on critical state variables to explain what they are supposed to do: this will help for future code reviews.

<details>
<summary>
There are <b>11</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

44:   mapping(string => bytes32) public chainToApprovedSender;

45:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

52:   mapping(string => Threshold[]) public chainToThresholds;

53:   mapping(bytes32 => Transaction) public txnHashToTransaction;

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L44) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L45) [#L52](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L52) [#L53](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L53) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) [#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) 

```solidity
File: contracts/usdy/rUSDY.sol

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L101) 

</details>

---

<a name="NC-33"></a> 
### [NC-33] Contract declarations should have NatSpec `@title` annotations
Some contract definitions have an incomplete NatSpec: add a `@title` notation to describe the contract to improve the code documentation.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

26: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L26](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L26) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

18: interface IRWADynamicOracle {

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L18) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```
[#L8](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L8) 

</details>

---

<a name="NC-34"></a> 
### [NC-34] Unused errors
The following `error`s are defined but not used. It is recommended to check the code for logical omissions that cause them not to be used. If it's determined that they are not needed anywhere, it's best to remove them from the codebase to improve code clarity and minimize confusion. Note that there may be cases where an error appears to be used because it has multiple definitions in different files. In such cases, the definitions should be moved to a separate file.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

320:   error InvalidPrice();

322:   error PriceNotSet();

```
[#L320](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L320) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L322) 

</details>

---

<a name="NC-35"></a> 
### [NC-35] Unused named return
Declaring named returns, but not using them, is confusing to the reader. Consider either completely removing them (by declaring just the type without a name), or remove the return statement and do a variable assignment. This would improve the readability of the code, and it may also help reduce regressions during future code refactors.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `price` not used
61:   function getPrice() public view whenNotPaused returns (uint256 price) {

/// `price` not used
90:   function simulateRange(
        uint256 blockTimeStamp,
        uint256 dailyIR,
        uint256 endTime,
        uint256 startTime,
        uint256 rangeStartPrice
      ) external view returns (uint256 price) {

/// `price` not used
248:   function derivePrice(
         Range memory currentRange,
         uint256 currentTime
       ) internal pure returns (uint256 price) {

```
[#L61](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L61) [#L90](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L90) [#L248](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L248) 

</details>

---

<a name="NC-36"></a> 
### [NC-36] Unused contract variables
The following state variables are defined but not used. It is recommended to check the code for logical omissions that cause them not to be used. If it's determined that they are not needed anywhere, it's best to remove them from the codebase to improve code clarity and minimize confusion.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) 

</details>

---

<a name="NC-37"></a> 
### [NC-37] Consider using `delete` rather than assigning zero to clear values
The `delete` keyword more closely matches the semantics of what is being done, and draws more attention to the changing of state, which may lead to a more thorough audit of its associated logic.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

134:     for (uint256 i = 0; i < thresholds.length; ++i) {

160:       for (uint256 i = 0; i < t.approvers.length; ++i) {

264:     for (uint256 i = 0; i < amounts.length; ++i) {

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

179:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L179) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

63:     for (uint256 i = 0; i < length; ++i) {

99:     for (uint256 i = 0; i < length; ++i) {

115:     for (uint256 i = 0; i < length + 1; ++i) {

```
[#L63](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L63) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L99) [#L115](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L115) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="NC-38"></a> 
### [NC-38] Expressions for constant values should use `immutable` rather than `constant`
While it doesn't save any gas because the compiler knows that developers often make this mistake, it's still best to use the right tool for the task at hand. There is a difference between `constant` variables and `immutable` variables, and they should each be used in their appropriate contexts. `constants` should be used for literal values written into the code, and `immutable` variables should be used for expressions, or values calculated in, or passed into the constructor.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

48:   bytes32 public constant VERSION = "1.0";

```
[#L48](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L48) 

```solidity
File: contracts/bridge/SourceBridge.sol

42:   bytes32 public constant VERSION = "1.0";

```
[#L42](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L42) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

329:   uint256 private constant ONE = 10 ** 27;

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) [#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) [#L329](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L329) 

```solidity
File: contracts/usdy/rUSDY.sol

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L91](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L91) [#L97](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L101) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

44:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L44) 

</details>

---

<a name="NC-39"></a> 
### [NC-39] Use the latest solidity version for deployment
Upgrading to a newer Solidity release can optimize gas usage, take advantage of new features and improve overall contract efficiency. Where possible, based on compatibility requirements, it is recommended to use newer/latest solidity version to take advantage of the latest optimizations and features.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L16) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```
[#L2](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L2) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="NC-40"></a> 
### [NC-40] Use of `override` is unnecessary
Starting with Solidity version [0.8.8](https://docs.soliditylang.org/en/v0.8.20/contracts.html#function-overriding), using the `override` keyword when the function solely overrides an interface function, and the function doesn't exist in multiple base contracts, is unnecessary.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

89:   ) internal override whenNotPaused {

```
[#L89](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L89) 

```solidity
File: contracts/bridge/SourceBridge.sol

177:   ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L177](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L177) 

```solidity
File: contracts/usdy/rUSDY.sol

700:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

711:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

722:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```
[#L700](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L700) [#L711](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L711) [#L722](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L722) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

128:   ) external payable override onlyGuardian returns (bytes[] memory results) {

```
[#L128](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L128) 

</details>

---

<a name="NC-41"></a> 
### [NC-41] Use scientific notation (e.g. `1e18`) rather than exponentiation (e.g. `10**18`)
While the compiler knows to optimize away the exponentiation, it's still better coding practice to use idioms that do not require compiler optimization, if they exist.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

329:   uint256 private constant ONE = 10 ** 27;

```
[#L329](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L329) 

</details>

---

<a name="NC-42"></a> 
### [NC-42] Missing checks for `address(0)` when assigning values to address state variables

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

52:     guardian = _guardian;

```
[#L52](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L52) 

</details>

---

<a name="NC-43"></a> 
### [NC-43] Common functions should be refactored to a common base contract
The functions below have the same implementation as is seen in other files. The functions should be refactored into functions of a common base contract.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// Seen in contracts/bridge/SourceBridge.sol
304:   function pause() external onlyOwner {

/// Seen in contracts/bridge/SourceBridge.sol
313:   function unpause() external onlyOwner {

```
[#L304](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L304) [#L313](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L313) 

```solidity
File: contracts/bridge/SourceBridge.sol

/// Seen in contracts/bridge/DestinationBridge.sol
151:   function pause() external onlyOwner {

/// Seen in contracts/bridge/DestinationBridge.sol
160:   function unpause() external onlyOwner {

/// Seen in contracts/usdy/rUSDYFactory.sol
175:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L151](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L151) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L160) [#L175](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L175) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Seen in contracts/bridge/SourceBridge.sol
227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

/// Seen in contracts/bridge/SourceBridge.sol
234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L227) [#L234](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L234) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Seen in contracts/bridge/SourceBridge.sol
126:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyGuardian returns (bytes[] memory results) {

```
[#L126](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L126) 

</details>

---

<a name="NC-44"></a> 
### [NC-44] Names of `private`/`internal` functions should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

248:   function derivePrice(
         Range memory currentRange,
         uint256 currentTime
       ) internal pure returns (uint256 price) {

268:   function roundUpTo8(uint256 value) internal pure returns (uint256) {

```
[#L248](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L248) [#L268](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L268) 

</details>

---

<a name="NC-45"></a> 
### [NC-45] Names of `private`/`internal` state variables should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

329:   uint256 private constant ONE = 10 ** 27;

```
[#L329](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L329) 

```solidity
File: contracts/usdy/rUSDY.sol

76:   mapping(address => uint256) private shares;

79:   mapping(address => mapping(address => uint256)) private allowances;

82:   uint256 private totalShares;

```
[#L76](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L76) [#L79](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L79) [#L82](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L82) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

46:   address internal immutable guardian;

```
[#L46](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L46) 

</details>

---

<a name="NC-46"></a> 
### [NC-46]  `require()` / `revert()` statements should have descriptive reason strings

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

391:     require(y == 0 || (z = x * y) / y == x);

```
[#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L391) 

</details>

---

<a name="NC-47"></a> 
### [NC-47] Return values of `approve()` not checked
Not all IERC20 implementations `revert()` when there's a failure in `approve()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually approving anything

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

111:     _approve(txnHash);

201:     _approve(txnHash);

```
[#L111](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L111) [#L201](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L201) 

```solidity
File: contracts/usdy/rUSDY.sol

277:     _approve(msg.sender, _spender, _amount);

310:     _approve(_sender, msg.sender, currentAllowance - _amount);

331:     _approve(

362:     _approve(msg.sender, _spender, currentAllowance - _subtractedValue);

```
[#L277](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L277) [#L310](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L310) [#L331](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L331) [#L362](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L362) 

</details>

---

<a name="NC-48"></a> 
### [NC-48] Variables should be named in mixedCase style
As the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html#naming-styles) suggests: arguments, local variables and mutable state variables should be named in mixedCase style.

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

34:   IRWALike public immutable TOKEN;

37:   IAxelarGateway public immutable AXELAR_GATEWAY;

40:   IAllowlist public immutable ALLOWLIST;

48:   bytes32 public constant VERSION = "1.0";

```
[#L34](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L34) [#L37](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L37) [#L40](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L40) [#L48](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L48) 

```solidity
File: contracts/bridge/SourceBridge.sol

33:   IRWALike public immutable TOKEN;

36:   IAxelarGateway public immutable AXELAR_GATEWAY;

39:   IAxelarGasService public immutable GAS_RECEIVER;

42:   bytes32 public constant VERSION = "1.0";

```
[#L33](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L33) [#L36](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L36) [#L39](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L39) [#L42](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L42) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

30:     uint256 trueStart = (startPrice * ONE) / dailyIR;

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) [#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) [#L30](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L30) 

```solidity
File: contracts/usdy/rUSDY.sol

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L91](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L91) [#L97](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L101) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

37:  *         i) Grant the `DEFAULT_ADMIN_ROLE` & PAUSER_ROLE to the `guardian` address

```
[#L37](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L37) 

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
File: contracts/bridge/DestinationBridge.sol

389:   event ApproverRemoved(address approver);

396:   event ApproverAdded(address approver);

405:   event ChainIdSupported(string srcChain, string approvedSource);

414:   event ThresholdSet(string chain, uint256[] amounts, uint256[] numOfApprovers);

422:   event BridgeCompleted(address user, uint256 amount);

432:   event MessageReceived(

```
[#L389](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L389) [#L396](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L396) [#L405](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L405) [#L414](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L414) [#L422](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L422) [#L432](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L432) 

```solidity
File: contracts/bridge/SourceBridge.sol

198:   event DestinationChainContractAddressSet(

```
[#L198](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L198) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

295:   event RangeSet(

312:   event RangeOverriden(

```
[#L295](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L295) [#L312](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L312) 

```solidity
File: contracts/usdy/rUSDY.sol

154:   event TransferShares(

172:   event SharesBurnt(

189:   event TokensBurnt(address indexed account, uint256 tokensBurnt);

```
[#L154](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L154) [#L172](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L172) [#L189](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L189) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

146:   event rUSDYDeployed(

```
[#L146](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L146) 

</details>

---

<a name="NC-50"></a> 
### [NC-50] Functions not used internally could be marked external

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

194:   function name() public pure returns (string memory) {

202:   function symbol() public pure returns (string memory) {

209:   function decimals() public pure returns (uint8) {

216:   function totalSupply() public view returns (uint256) {

226:   function balanceOf(address _account) public view returns (uint256) {

245:   function transfer(address _recipient, uint256 _amount) public returns (bool) {

256:   function allowance(

276:   function approve(address _spender, uint256 _amount) public returns (bool) {

301:   function transferFrom(

327:   function increaseAllowance(

353:   function decreaseAllowance(

372:   function getTotalShares() public view returns (uint256) {

381:   function sharesOf(address _account) public view returns (uint256) {

416:   function transferShares(

```
[#L194](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L194) [#L202](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L202) [#L209](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L209) [#L216](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L216) [#L226](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L226) [#L245](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L245) [#L256](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L256) [#L276](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L276) [#L301](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L301) [#L327](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L327) [#L353](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L353) [#L372](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L372) [#L381](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L381) [#L416](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L416) 

</details>

---


## Gas Optimizations

<a name="GAS-1"></a> 
### [GAS-1] Consider activating via-ir for deploying
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

<a name="GAS-2"></a> 
### [GAS-2] Divisions can be `unchecked` to save gas
The expression `type(int).min/(-1)` is the only case where division causes an overflow. Therefore, uncheck can be used to [save gas](https://gist.github.com/DadeKuma/3bc597338ae774b8b3bd43280d55271f) in scenarios where it is certain that such an overflow will not occur.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

30:     uint256 trueStart = (startPrice * ONE) / dailyIR;

103:       uint256 trueStart = (rangeStartPrice * ONE) / dailyIR;

205:       uint256 trueStart = (newPrevRangeClosePrice * ONE) / newDailyIR;

252:     uint256 elapsedDays = (currentTime - currentRange.start) / DAY;

387:     z = _mul(x, y) / ONE;

391:     require(y == 0 || (z = x * y) / y == x);

```
[#L30](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L30) [#L103](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L103) [#L205](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L205) [#L252](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L252) [#L387](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L387) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L391) 

```solidity
File: contracts/usdy/rUSDY.sol

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

227:     return (_sharesOf(_account) * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

391:     return (_rUSDYAmount * 1e18 * BPS_DENOMINATOR) / oracle.getPrice();

398:     return (_shares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L217](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L217) [#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L227) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L391) [#L398](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L398) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="GAS-3"></a> 
### [GAS-3] Don't transfer with zero amount to save gas
In Solidity, unnecessary operations can waste gas. For example, a transfer function without a zero amount check uses gas even if called with a zero amount, since the contract state remains unchanged. Implementing a zero amount check avoids these unnecessary function calls, saving gas and improving efficiency.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

324:     IRWALike(_token).transfer(owner(), balance);

```
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L454](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L680) 

</details>

---

<a name="GAS-4"></a> 
### [GAS-4] Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

271:       value += 1e10;

273:     value -= remainder;

```
[#L271](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L271) [#L273](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L273) 

```solidity
File: contracts/usdy/rUSDY.sol

551:     totalShares += _sharesAmount;

588:     totalShares -= _sharesAmount;

```
[#L551](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L551) [#L588](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L588) 

</details>

---

<a name="GAS-5"></a> 
### [GAS-5] Increments can be `unchecked` to save gas
Using `unchecked` increments can save gas by bypassing the built-in overflow checks. This can save 30-40 gas per iteration. So it is recommended to use unchecked increments when overflow is not possible.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

134:     for (uint256 i = 0; i < thresholds.length; ++i) {

160:       for (uint256 i = 0; i < t.approvers.length; ++i) {

264:     for (uint256 i = 0; i < amounts.length; ++i) {

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

179:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L179) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

63:     for (uint256 i = 0; i < length; ++i) {

99:     for (uint256 i = 0; i < length; ++i) {

115:     for (uint256 i = 0; i < length + 1; ++i) {

```
[#L63](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L63) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L99) [#L115](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L115) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="GAS-6"></a> 
### [GAS-6] Initializers can be marked as payable to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. Initializers can be safely marked as payable, because only the deployer or the factory contract would call the function without carrying any funds.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

109:   function initialize(

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L109) 

</details>

---

<a name="GAS-7"></a> 
### [GAS-7] `internal` functions only called once can be inlined to save gas
If an `internal` function is only used once, there is no need to modularize it, unless the function calling it would otherwise be too long and complex. Not inlining costs 20 to 40 gas because of two extra JUMP instructions and additional stack operations needed for function calls.

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `_attachThreshold` is used only once
128:   function _attachThreshold(

/// `_checkThresholdMet` is used only once
177:   function _checkThresholdMet(bytes32 txnHash) internal view returns (bool) {

```
[#L128](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L128) [#L177](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L177) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `roundUpTo8` is used only once
268:   function roundUpTo8(uint256 value) internal pure returns (uint256) {

/// `_rpow` is used only once
331:   function _rpow(

/// `_rmul` is used only once
386:   function _rmul(uint256 x, uint256 y) internal pure returns (uint256 z) {

/// `_mul` is used only once
390:   function _mul(uint256 x, uint256 y) internal pure returns (uint256 z) {

```
[#L268](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L268) [#L331](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L331) [#L386](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L386) [#L390](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L390) 

```solidity
File: contracts/usdy/rUSDY.sol

/// `__rUSDY_init` is used only once
120:   function __rUSDY_init(

/// `__rUSDY_init_unchained` is used only once
134:   function __rUSDY_init_unchained(

/// `_mintShares` is used only once
543:   function _mintShares(

```
[#L120](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L120) [#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L134) [#L543](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L543) 

</details>

---

<a name="GAS-8"></a> 
### [GAS-8] `keccak256()` hash of literals should only be computed once
The result of the hash should be stored in an immutable variable, and the variable should be used instead. If the hash is being used as a part of a function selector, the cast to `bytes4` should also only be done once.

<details>
<summary>
There are <b>7</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) 

```solidity
File: contracts/usdy/rUSDY.sol

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

102:     keccak256("LIST_CONFIGURER_ROLE");

```
[#L97](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L102](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L102) 

</details>

---

<a name="GAS-9"></a> 
### [GAS-9] Low level `call` can be optimized with assembly
When using low-level calls, the `returnData` is copied to memory even if the variable is not utilized. The proper way to handle this is through a low level assembly call.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

180:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L180](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L180) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L131](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L131) 

</details>

---

<a name="GAS-10"></a> 
### [GAS-10] Multiple accesses of the same mapping/array key/index should be cached
The instances below point to the second+ access of a value inside a mapping/array, within a function. Caching a mapping's value in a local `storage` or `calldata` variable when the value is accessed [multiple times](https://gist.github.com/IllIllI000/ec23a57daa30a8f8ca8b9681c8ccefb0), saves ~42 gas per access due to not having to recalculate the key's keccak256 hash (Gkeccak256 - 30 gas) and that calculation's associated stack operations. Caching an array's struct avoids recalculating the array offsets into memory/calldata

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `chainToApprovedSender[srcChain]` is also accessed on line 96
99:     if (chainToApprovedSender[srcChain] != keccak256(abi.encode(srcAddr))) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 96
99:     if (chainToApprovedSender[srcChain] != keccak256(abi.encode(srcAddr))) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 96
102:     if (isSpentNonce[chainToApprovedSender[srcChain]][nonce]) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 96
102:     if (isSpentNonce[chainToApprovedSender[srcChain]][nonce]) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 96
106:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `isSpentNonce[chainToApprovedSender[srcChain]` is also accessed on line 102
106:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `chainToApprovedSender[srcChain]` is also accessed on line 96
106:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `isSpentNonce[chainToApprovedSender[srcChain]` is also accessed on line 102
106:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `txnToThresholdSet[txnHash]` is also accessed on line 137
144:     if (txnToThresholdSet[txnHash].numberOfApprovalsNeeded == 0) {

/// `chainToThresholds[srcChain]` is also accessed on line 263
266:         chainToThresholds[srcChain].push(

/// `chainToThresholds[srcChain]` is also accessed on line 263
270:         if (chainToThresholds[srcChain][i - 1].amount > amounts[i]) {

/// `chainToThresholds[srcChain]` is also accessed on line 263
273:         chainToThresholds[srcChain].push(

/// `txnHashToTransaction[txnHash]` is also accessed on line 339
350:       delete txnHashToTransaction[txnHash];

```
[#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L99) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L99) [#L102](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L102) [#L102](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L102) [#L106](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L106) [#L106](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L106) [#L106](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L106) [#L106](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L106) [#L144](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L144) [#L266](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L266) [#L270](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L270) [#L273](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L273) [#L350](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L350) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// ` = ` is also accessed on line 97
100:       rangeList[i] = ranges[i];

/// `ranges[indexToModify - 1]` is also accessed on line 193
198:       if (newStart < ranges[indexToModify - 1].end) revert InvalidRange();

/// `ranges[indexToModify + 1]` is also accessed on line 187
200:       if (newEnd > ranges[indexToModify + 1].start) revert InvalidRange();

/// `ranges[indexToModify]` is also accessed on line 206
208:       ranges[indexToModify] = Range(

```
[#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L100) [#L198](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L198) [#L200](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L200) [#L208](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L208) 

```solidity
File: contracts/usdy/rUSDY.sol

/// `shares[_sender]` is also accessed on line 524
530:     shares[_sender] = currentSenderShares - _sharesAmount;

/// `shares[_account]` is also accessed on line 583
590:     shares[_account] = accountShares - _sharesAmount;

```
[#L530](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L530) [#L590](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L590) 

</details>

---

<a name="GAS-11"></a> 
### [GAS-11] Newer versions of solidity are more gas efficient
The solidity language continues to pursue more efficient gas optimization schemes. Adopting a newer version of solidity can be more gas efficient.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L16) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```
[#L2](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L2) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="GAS-12"></a> 
### [GAS-12] Operator `>=`/`<=` costs less gas than operator `>`/`<`
The compiler uses opcodes `GT` and `ISZERO` for code that uses `>`, but only requires `LT` for `>=`. A similar behavior applies for `>`, which uses opcodes `LT` and `ISZERO`, but only requires `GT` for `<=`. It can save 3 gas for each. It should be converted to the `<=`/`>=` equivalent when comparing against integer literals.

<details>
<summary>
There are <b>18</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

134:     for (uint256 i = 0; i < thresholds.length; ++i) {

159:     if (t.approvers.length > 0) {

160:       for (uint256 i = 0; i < t.approvers.length; ++i) {

264:     for (uint256 i = 0; i < amounts.length; ++i) {

270:         if (chainToThresholds[srcChain][i - 1].amount > amounts[i]) {

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L134) [#L159](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L159) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L264) [#L270](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L270) 

```solidity
File: contracts/bridge/SourceBridge.sol

179:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L179) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

63:     for (uint256 i = 0; i < length; ++i) {

99:     for (uint256 i = 0; i < length; ++i) {

115:     for (uint256 i = 0; i < length + 1; ++i) {

187:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)

187:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)

193:       if (newStart < ranges[indexToModify - 1].end) revert InvalidRange();

198:       if (newStart < ranges[indexToModify - 1].end) revert InvalidRange();

200:       if (newEnd > ranges[indexToModify + 1].start) revert InvalidRange();

```
[#L63](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L63) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L99) [#L115](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L115) [#L187](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L187) [#L187](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L187) [#L193](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L193) [#L198](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L198) [#L200](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L200) 

```solidity
File: contracts/usdy/rUSDY.sol

435:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

452:     if (usdyAmount < BPS_DENOMINATOR) revert UnwrapTooSmall();

```
[#L435](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L450) [#L452](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L452) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="GAS-13"></a> 
### [GAS-13] Reduce gas usage by moving to Solidity 0.8.19 or later
Solidity version 0.8.19 introduced a number of gas optimizations, refer to the [Solidity 0.8.19 Release Announcement](https://soliditylang.org/blog/2023/02/22/solidity-0.8.19-release-announcement/) for details.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L16) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```
[#L2](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L2) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="GAS-14"></a> 
### [GAS-14] Redundant state variable getters
Getters for public state variables are automatically generated so there is no need to code them manually and waste gas.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

372:   function getTotalShares() public view returns (uint256) {
         return totalShares;

```
[#L372](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L372) 

</details>

---

<a name="GAS-15"></a> 
### [GAS-15] Remove or replace unused state variables
Saves a storage slot. If the variable is assigned a non-zero value, saves Gsset (20000 gas). If it's assigned a zero value, saves Gsreset (2900 gas). If the variable remains unassigned, there is no gas savings unless the variable is `public`, in which case the compiler-generated non-payable getter deployment cost is saved. If the state variable is overriding an interface's public function, mark the variable as `constant` or `immutable` so that it does not use a storage slot.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) 

</details>

---

<a name="GAS-16"></a> 
### [GAS-16] `require()`/`revert()` strings longer than 32 bytes cost extra gas
Each extra memory word of bytes past the original 32 [incurs an MSTORE](https://gist.github.com/hrkrshnn/ee8fabd532058307229d65dcd5836ddc#consider-having-short-revert-strings) which costs 3 gas

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

307:     require(currentAllowance >= _amount, "TRANSFER_AMOUNT_EXCEEDS_ALLOWANCE");

435:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

```
[#L307](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L307) [#L435](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L450) 

</details>

---

<a name="GAS-17"></a> 
### [GAS-17] The result of a function call should be cached rather than re-calling the function
The function calls in solidity are expensive. If the same result of the same function calls are to be used several times, the result should be cached to reduce the gas consumption of repeated calls.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `keccak256` is called 2 times
85:   function _execute(
        string calldata srcChain,
        string calldata srcAddr,
        bytes calldata payload
      ) internal override whenNotPaused {

/// `Threshold` is called 2 times
255:   function setThresholds(
         string calldata srcChain,
         uint256[] calldata amounts,
         uint256[] calldata numOfApprovers
       ) external onlyOwner {

/// `IRWALike` is called 2 times
322:   function rescueTokens(address _token) external onlyOwner {

```
[#L85](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L85) [#L255](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L255) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L322) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `derivePrice` is called 2 times
61:   function getPrice() public view whenNotPaused returns (uint256 price) {

/// `derivePrice` is called 3 times
90:   function simulateRange(
        uint256 blockTimeStamp,
        uint256 dailyIR,
        uint256 endTime,
        uint256 startTime,
        uint256 rangeStartPrice
      ) external view returns (uint256 price) {

/// `Range` is called 2 times
90:   function simulateRange(
        uint256 blockTimeStamp,
        uint256 dailyIR,
        uint256 endTime,
        uint256 startTime,
        uint256 rangeStartPrice
      ) external view returns (uint256 price) {

/// `InvalidRange` is called 5 times
172:   function overrideRange(
         uint256 indexToModify,
         uint256 newStart,
         uint256 newEnd,
         uint256 newDailyIR,
         uint256 newPrevRangeClosePrice
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

/// `Range` is called 2 times
172:   function overrideRange(
         uint256 indexToModify,
         uint256 newStart,
         uint256 newEnd,
         uint256 newDailyIR,
         uint256 newPrevRangeClosePrice
       ) external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L61](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L61) [#L90](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L90) [#L90](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L90) [#L172](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L172) [#L172](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L172) 

```solidity
File: contracts/usdy/rUSDY.sol

/// `_grantRole` is called 6 times
134:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// `getRUSDYByShares` is called 2 times
575:   function _burnShares(
         address _account,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

/// `_isBlocked` is called 3 times
626:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

/// `_isSanctioned` is called 3 times
626:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

/// `_isAllowed` is called 3 times
626:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L134) [#L575](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L575) [#L626](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L626) [#L626](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L626) [#L626](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L626) 

</details>

---

<a name="GAS-18"></a> 
### [GAS-18] Unlimited gas consumption risk due to external call recipients
When calling an external function without specifying a gas limit , the called contract may consume all the remaining gas, causing the tx to be reverted. To mitigate this, it is recommended to explicitly set a gas limit when making low level external calls.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

180:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L180](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L180) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L131](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L131) 

</details>

---

<a name="GAS-19"></a> 
### [GAS-19] Unused named return variables without optimizer waste gas
Consider changing the variable to be an unnamed one, since the variable is never assigned, nor is it returned by name. If the optimizer is not turned on, leaving the code as it is will also waste gas for the stack variable.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `price` not used
61:   function getPrice() public view whenNotPaused returns (uint256 price) {

/// `price` not used
90:   function simulateRange(
        uint256 blockTimeStamp,
        uint256 dailyIR,
        uint256 endTime,
        uint256 startTime,
        uint256 rangeStartPrice
      ) external view returns (uint256 price) {

/// `price` not used
248:   function derivePrice(
         Range memory currentRange,
         uint256 currentTime
       ) internal pure returns (uint256 price) {

```
[#L61](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L61) [#L90](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L90) [#L248](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L248) 

</details>

---

<a name="GAS-20"></a> 
### [GAS-20] Use assembly to compute hashes to save gas
If the arguments to the encode call can fit into the scratch space (two words or fewer), then it's more efficient to use assembly to generate the hash (80 gas):

`keccak256(abi.encodePacked(x, y)) -> assembly {mstore(0x00, a); mstore(0x20, b); let hash := keccak256(0x00, 0x40); }`

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

99:     if (chainToApprovedSender[srcChain] != keccak256(abi.encode(srcAddr))) {

108:     bytes32 txnHash = keccak256(payload);

238:     chainToApprovedSender[srcChain] = keccak256(abi.encode(srcContractAddress));

```
[#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L99) [#L108](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L108) [#L238](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L238) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) 

```solidity
File: contracts/usdy/rUSDY.sol

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

102:     keccak256("LIST_CONFIGURER_ROLE");

```
[#L97](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L102](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L102) 

</details>

---

<a name="GAS-21"></a> 
### [GAS-21] Use assembly to emit events
To efficiently emit events, it's possible to utilize assembly by making use of scratch space and the free memory pointer. This approach has the advantage of potentially avoiding the costs associated with memory expansion.

However, it's important to note that in order to safely optimize this process, it is preferable to cache and restore the free memory pointer.

A good example of such practice can be seen in [Solady's](https://github.com/Vectorized/solady/blob/main/src/tokens/ERC1155.sol#L167) codebase.

<details>
<summary>
There are <b>20</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

113:     emit MessageReceived(srcChain, srcSender, amt, nonce);

212:     emit ApproverAdded(approver);

222:     emit ApproverRemoved(approver);

239:     emit ChainIdSupported(srcChain, srcContractAddress);

278:     emit ThresholdSet(srcChain, amounts, numOfApprovers);

351:       emit BridgeCompleted(txn.sender, txn.amount);

```
[#L113](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L113) [#L212](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L212) [#L222](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L222) [#L239](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L239) [#L278](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L278) [#L351](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L351) 

```solidity
File: contracts/bridge/SourceBridge.sol

143:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```
[#L143](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L143) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

150:     emit RangeSet(

215:     emit RangeOverriden(

```
[#L150](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L150) [#L215](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L215) 

```solidity
File: contracts/usdy/rUSDY.sol

421:     emit TransferShares(msg.sender, _recipient, _sharesAmount);

423:     emit Transfer(msg.sender, _recipient, tokensAmount);

438:     emit Transfer(address(0), msg.sender, getRUSDYByShares(_USDYAmount));

439:     emit TransferShares(address(0), msg.sender, _USDYAmount);

455:     emit TokensBurnt(msg.sender, _rUSDYAmount);

470:     emit Transfer(_sender, _recipient, _amount);

471:     emit TransferShares(_sender, _recipient, _sharesToTransfer);

494:     emit Approval(_owner, _spender, _amount);

594:     emit SharesBurnt(

682:     emit TokensBurnt(_account, _amount);

```
[#L421](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L421) [#L423](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L423) [#L438](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L438) [#L439](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L439) [#L455](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L455) [#L470](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L470) [#L471](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L471) [#L494](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L494) [#L594](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L594) [#L682](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L682) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

101:     emit rUSDYDeployed(

```
[#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L101) 

</details>

---

<a name="GAS-22"></a> 
### [GAS-22] Using a double `if` statement instead of a logical AND (`&&`)
Using a double `if` statement instead of a logical AND (`&&`) can provide similar short-circuiting behavior whereas double if is slightly [more gas efficient](https://gist.github.com/DadeKuma/931ce6794a050201ec6544dbcc31316c).

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

187:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)

```
[#L187](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L187) 

```solidity
File: contracts/usdy/rUSDY.sol

633:     if (from != msg.sender && to != msg.sender) {

```
[#L633](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L633) 

</details>

---

<a name="GAS-23"></a> 
### [GAS-23] Use a more recent version of solidity
- Use a solidity version of at least 0.8.2 to get simple compiler automatic inlining.
- Use a solidity version of at least 0.8.3 to get better struct packing and cheaper multiple storage reads.
- Use a solidity version of at least 0.8.4 to get custom errors, which are cheaper at deployment than revert()/require() strings.
- Use a solidity version of at least 0.8.10 to have external calls skip contract existence checks if the external call has a return value.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L16) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```
[#L2](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L2) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="GAS-24"></a> 
### [GAS-24] Use `storage` instead of `memory` for structs/arrays
When fetching data from a storage location, assigning the data to a `memory` variable causes all fields of the struct/array to be read from storage, which incurs a Gcoldsload (**2100 gas**) for *each* field of the struct/array. If the fields are read from the new memory variable, they incur an additional `MLOAD` rather than a cheap stack read. Instead of declaring the variable with the `memory` keyword, declaring the variable with the `storage` keyword and caching any fields that need to be re-read in stack variables, will be much cheaper, only incurring the Gcoldsload for the fields actually read. The only time it makes sense to read the whole struct/array into a `memory` variable, is if the full struct/array is being returned by the function, is being passed to a function that requires `memory`, or if the array/struct is being read from another `memory` array/struct.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

133:     Threshold[] memory thresholds = chainToThresholds[srcChain];

135:       Threshold memory t = thresholds[i];

178:     TxnThreshold memory t = txnToThresholdSet[txnHash];

339:     Transaction memory txn = txnHashToTransaction[txnHash];

```
[#L133](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L133) [#L135](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L135) [#L178](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L178) [#L339](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L339) 

```solidity
File: contracts/bridge/SourceBridge.sol

81:     string memory destContract = destChainToContractAddr[destinationChain];

```
[#L81](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L81) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

106:       Range memory lastRange = ranges[ranges.length - 1];

116:       Range memory range = rangeList[(length) - i];

141:     Range memory lastRange = ranges[ranges.length - 1];

```
[#L106](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L106) [#L116](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L116) [#L141](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L141) 

</details>

---

<a name="GAS-25"></a> 
### [GAS-25] Use `unchecked` block for safe subtractions
If it can be confirmed that the subtraction operation will not overflow, using an unchecked block can save gas. For example, `require(x <= y); z = y - x;` can be optimized to `require(x <= y); unchecked { z = y - x; }`

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

/// Checked on line 307
310:     _approve(_sender, msg.sender, currentAllowance - _amount);

/// Checked on line 359
362:     _approve(msg.sender, _spender, currentAllowance - _subtractedValue);

/// Checked on line 526
530:     shares[_sender] = currentSenderShares - _sharesAmount;

/// Checked on line 584
590:     shares[_account] = accountShares - _sharesAmount;

```
[#L310](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L310) [#L362](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L362) [#L530](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L530) [#L590](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L590) 

</details>

---

<a name="GAS-26"></a> 
### [GAS-26] Using bitmap to store bool states can save gas
Using a bitmap instead of a bool array or a bool mapping to store boolean states can save gas fees. This is because the bitmap can store 256 boolean values in a single slot instead of 256 slots, which can save gas when writing bool values or when reading multiple bool values from the same slot.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

43:   mapping(address => bool) public approvers;

45:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

```
[#L43](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L43) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L45) 

</details>

---

<a name="GAS-27"></a> 
### [GAS-27] `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants)
When updating a value in an array with arithmetic, using `array[index] += amount` is cheaper than `array[index] = array[index] + amount`.
This is because you avoid an additonal `mload` when the array is stored in memory, and an `sload` when the array is stored in storage.
This can be applied for any arithmetic operation including `+=`, `-=`,`/=`,`*=`,`^=`,`&=`, `%=`, `<<=`,`>>=`, and `>>>=`.
This optimization can be particularly significant if the pattern occurs during a loop.

*Saves 28 gas for a storage array, 38 for a memory array*

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

531:     shares[_recipient] = shares[_recipient] + _sharesAmount;

553:     shares[_recipient] = shares[_recipient] + _sharesAmount;

```
[#L531](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L531) [#L553](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L553) 

</details>

---

<a name="GAS-28"></a> 
### [GAS-28] Using bools for storage incurs overhead
Use uint256(1) and uint256(2) for true/false to avoid a Gwarmaccess (100 gas), and to avoid Gsset (20000 gas) when changing from ‘false’ to ‘true’, after having been ‘true’ in the past. See [source](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/58f635312aa21f947cae5f8578638a85aa2519f5/contracts/security/ReentrancyGuard.sol#L23-L27).

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

43:   mapping(address => bool) public approvers;

45:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

```
[#L43](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L43) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L45) 

</details>

---

<a name="GAS-29"></a> 
### [GAS-29] Cache array length outside of loop
If not cached, the solidity compiler will always read the length of the array during each iteration. That is, if it is a storage array, this is an extra sload operation (100 additional extra gas for each iteration except for the first) and if it is a memory array, this is an extra mload operation (3 additional gas for each iteration except for the first).

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

134:     for (uint256 i = 0; i < thresholds.length; ++i) {

160:       for (uint256 i = 0; i < t.approvers.length; ++i) {

264:     for (uint256 i = 0; i < amounts.length; ++i) {

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

179:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L179) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="GAS-30"></a> 
### [GAS-30] State variables should be cached in stack variables rather than re-reading them from storage
The instances below point to the second+ access of a state variable within a function. Caching of a state variable replaces each Gwarmaccess (100 gas) with a much cheaper stack read. Other less obvious fixes/optimizations include having local memory caches of state variable structs, or having local caches of state variable contracts/addresses.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// More than 1 read for `ranges`, line 100 and 97
100:       rangeList[i] = ranges[i];

/// More than 1 read for `ranges`, line 102 and 97
102:     if (startTime == ranges[0].start) {

/// More than 1 read for `ranges`, line 106 and 97
106:       Range memory lastRange = ranges[ranges.length - 1];

```
[#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L100) [#L102](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L102) [#L106](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L106) 

```solidity
File: contracts/usdy/rUSDY.sol

/// More than 1 read for `shares`, line 531 and 524
531:     shares[_recipient] = shares[_recipient] + _sharesAmount;

```
[#L531](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L531) 

</details>

---

<a name="GAS-31"></a> 
### [GAS-31] Use `calldata` instead of `memory` for function arguments that do not get mutated
Mark data types as `calldata` instead of `memory` where possible. This makes it so that the data is not automatically loaded into memory. If the data passed into the function does not need to be changed (like updating values in an array), it can be passed in as `calldata`. The one exception to this is if the argument must later be passed into another function that takes an argument that specifies `memory` storage.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

137:     string memory destinationChain,

```
[#L137](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L137) 

</details>

---

<a name="GAS-32"></a> 
### [GAS-32] Use Custom Errors
[Source](https://blog.soliditylang.org/2021/04/21/custom-errors/)
Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

183:       require(success, "Call Failed");

```
[#L183](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L183) 

```solidity
File: contracts/usdy/rUSDY.sol

307:     require(currentAllowance >= _amount, "TRANSFER_AMOUNT_EXCEEDS_ALLOWANCE");

435:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

490:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

491:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

519:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

520:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

547:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

579:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

584:     require(_sharesAmount <= accountShares, "BURN_AMOUNT_EXCEEDS_BALANCE");

634:       require(!_isBlocked(msg.sender), "rUSDY: 'sender' address blocked");

635:       require(!_isSanctioned(msg.sender), "rUSDY: 'sender' address sanctioned");

644:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");

645:       require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

646:       require(_isAllowed(from), "rUSDY: 'from' address not on allowlist");

651:       require(!_isBlocked(to), "rUSDY: 'to' address blocked");

652:       require(!_isSanctioned(to), "rUSDY: 'to' address sanctioned");

653:       require(_isAllowed(to), "rUSDY: 'to' address not on allowlist");

```
[#L307](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L307) [#L435](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L450) [#L490](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L490) [#L491](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L491) [#L519](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L519) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L520) [#L547](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L547) [#L579](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L579) [#L584](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L584) [#L634](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L634) [#L635](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L635) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L644) [#L645](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L645) [#L646](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L646) [#L651](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L651) [#L652](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L652) [#L653](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L653) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

134:       require(success, "Call Failed");

155:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L134) [#L155](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L155) 

</details>

---

<a name="GAS-33"></a> 
### [GAS-33] Don't initialize variables with default value

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

134:     for (uint256 i = 0; i < thresholds.length; ++i) {

160:       for (uint256 i = 0; i < t.approvers.length; ++i) {

264:     for (uint256 i = 0; i < amounts.length; ++i) {

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

179:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L179](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L179) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

63:     for (uint256 i = 0; i < length; ++i) {

99:     for (uint256 i = 0; i < length; ++i) {

115:     for (uint256 i = 0; i < length + 1; ++i) {

```
[#L63](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L63) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L99) [#L115](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L115) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="GAS-34"></a> 
### [GAS-34] Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead
Using `int`s/`uint`s smaller than 32 bytes may cost more gas. This is because the EVM operates on 32 bytes at a time, so if an element is smaller than 32 bytes, the EVM must perform more operations to reduce the size of the element from 32 bytes to the desired size.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

209:   function decimals() public pure returns (uint8) {

```
[#L209](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L209) 

</details>

---

<a name="GAS-35"></a> 
### [GAS-35] Constructors can be marked as `payable` to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. A constructor can be safely marked as payable, because only the deployer would be able to pass funds, and the project itself would not pass any funds.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

105:   constructor() {

```
[#L105](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L105) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

51:   constructor(address _guardian) {

```
[#L51](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L51) 

</details>

---

<a name="GAS-36"></a> 
### [GAS-36] Functions guaranteed to revert when called by normal users can be marked `payable`
If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function. Marking the function as `payable` will lower the gas cost for legitimate callers because the compiler will not include checks for whether a payment was provided.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

210:   function addApprover(address approver) external onlyOwner {

220:   function removeApprover(address approver) external onlyOwner {

286:   function setMintLimit(uint256 mintLimit) external onlyOwner {

295:   function setMintLimitDuration(uint256 mintDuration) external onlyOwner {

304:   function pause() external onlyOwner {

313:   function unpause() external onlyOwner {

322:   function rescueTokens(address _token) external onlyOwner {

```
[#L210](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L210) [#L220](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L220) [#L286](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L286) [#L295](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L295) [#L304](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L304) [#L313](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L313) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L322) 

```solidity
File: contracts/bridge/SourceBridge.sol

151:   function pause() external onlyOwner {

160:   function unpause() external onlyOwner {

```
[#L151](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L151) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L160) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L227](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L227) [#L234](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L234) 

```solidity
File: contracts/usdy/rUSDY.sol

662:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

685:   function pause() external onlyRole(PAUSER_ROLE) {

689:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

```
[#L662](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L662) [#L685](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L685) [#L689](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L689) 

</details>

---

<a name="GAS-37"></a> 
### [GAS-37] `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too)
*Saves 5 gas per loop*

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

94:     bytes memory payload = abi.encode(VERSION, msg.sender, amount, nonce++);

```
[#L94](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L94) 

</details>

---

<a name="GAS-38"></a> 
### [GAS-38] Using `private` rather than `public` for constants, saves gas
If needed, the values can be read from the verified contract source code, or if there are multiple values there can be a single getter function that [returns a tuple](https://github.com/code-423n4/2022-08-frax/blob/90f55a9ce4e25bceed3a74290b854341d8de6afa/src/contracts/FraxlendPair.sol#L156-L178) of the values of all currently-public constants. Saves **3406-3606 gas** in deployment gas due to the compiler not having to create non-payable getter functions for deployment calldata, not having to store the bytes of the value outside of where it's used, and not adding another entry to the method ID table

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

48:   bytes32 public constant VERSION = "1.0";

```
[#L48](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L48) 

```solidity
File: contracts/bridge/SourceBridge.sol

42:   bytes32 public constant VERSION = "1.0";

```
[#L42](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L42) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L9](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L9) [#L13](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L13) [#L14](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L14) 

```solidity
File: contracts/usdy/rUSDY.sol

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L91](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L91) [#L97](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L101) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

44:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDYFactory.sol#L44) 

</details>

---

<a name="GAS-39"></a> 
### [GAS-39] Use `!= 0` instead of `> 0` for unsigned integer comparison
Using `== 0`, `!= 0` instead of `> 0`, `>= 1`, `< 1`, `<= 0` can save gas.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

159:     if (t.approvers.length > 0) {

```
[#L159](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L159) 

```solidity
File: contracts/usdy/rUSDY.sol

435:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

```
[#L435](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L450) 

</details>

---

<a name="GAS-40"></a> 
### [GAS-40] Using assembly to check for zero can save gas
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

<details>
<summary>
There are <b>16</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

96:     if (chainToApprovedSender[srcChain] == bytes32(0)) {

144:     if (txnToThresholdSet[txnHash].numberOfApprovalsNeeded == 0) {

265:       if (i == 0) {

```
[#L96](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L96) [#L144](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L144) [#L265](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/DestinationBridge.sol#L265) 

```solidity
File: contracts/bridge/SourceBridge.sol

83:     if (bytes(destContract).length == 0) {

87:     if (msg.value == 0) {

```
[#L83](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L83) [#L87](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/bridge/SourceBridge.sol#L87) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

184:     if (indexToModify == 0) {

204:     if (indexToModify == 0) {

391:     require(y == 0 || (z = x * y) / y == x);

```
[#L184](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L184) [#L204](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L204) [#L391](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/rwaOracles/RWADynamicOracle.sol#L391) 

```solidity
File: contracts/usdy/rUSDY.sol

490:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

491:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

519:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

520:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

547:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

579:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

642:     if (from != address(0)) {

649:     if (to != address(0)) {

```
[#L490](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L490) [#L491](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L491) [#L519](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L519) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L520) [#L547](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L547) [#L579](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L579) [#L642](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L642) [#L649](https://github.com/code-423n4/2023-09-ondo/blob/623dd3c0ff3c4d8ce4ed563b96da50d08cd803c5/contracts/usdy/rUSDY.sol#L649) 

</details>

---

