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


Total <b>14</b> instances over <b>6</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Governance functions should be controlled by time locks | 3 |
| [L-2](#L-2) | Missing storage gap for upgradable contracts | 1 |
| [L-3](#L-3) | Using zero as a parameter | 4 |
| [L-4](#L-4) | Missing zero address check in initializer | 1 |
| [L-5](#L-5) | Initializers could be front-run | 1 |
| [L-6](#L-6) | Unsafe ERC20 operation(s) | 4 |

## Non Critical Issues


Total <b>319</b> instances over <b>35</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | `assert()` should be replaced with `require()` or `revert()` | 1 |
| [NC-2](#NC-2) | Contract declarations should have NatSpec `@author` annotations | 3 |
| [NC-3](#NC-3) | Consider adding formal verification proofs | 1 |
| [NC-4](#NC-4) | Constants should be put on the left side of comparisons | 16 |
| [NC-5](#NC-5) | Contracts should have full test coverage | 1 |
| [NC-6](#NC-6) | Events that mark critical parameter changes should contain both the old and the new value | 16 |
| [NC-7](#NC-7) | Custom errors has no error details | 15 |
| [NC-8](#NC-8) | Custom errors should be used rather than `revert()`/`require()` | 21 |
| [NC-9](#NC-9) | `else` block not required | 3 |
| [NC-10](#NC-10) | Enable IR-based code generation | 1 |
| [NC-11](#NC-11) | Events are emitted without the sender information | 14 |
| [NC-12](#NC-12) | Import declarations should import specific identifiers, rather than the whole file | 32 |
| [NC-13](#NC-13) | Large or complicated code bases should implement invariant tests | 1 |
| [NC-14](#NC-14) | Missing zero address check in functions with address parameters | 23 |
| [NC-15](#NC-15) | Consider moving `msg.sender` checks to `modifier`s | 3 |
| [NC-16](#NC-16) | Named mappings are recommended | 9 |
| [NC-17](#NC-17) | NatSpec documentation for contract is missing | 3 |
| [NC-18](#NC-18) | NatSpec documentation for function is missing | 11 |
| [NC-19](#NC-19) | Modifier declarations should have NatSpec descriptions | 1 |
| [NC-20](#NC-20) | Missing NatSpec `@param` | 28 |
| [NC-21](#NC-21) | Public variable declarations should have NatSpec descriptions | 10 |
| [NC-22](#NC-22) | NatSpec `@return` is missing | 15 |
| [NC-23](#NC-23) | State variables should include comments | 11 |
| [NC-24](#NC-24) | Contract declarations should have NatSpec `@title` annotations | 3 |
| [NC-25](#NC-25) | Unused named return | 3 |
| [NC-26](#NC-26) | Consider using `delete` rather than assigning zero to clear values | 8 |
| [NC-27](#NC-27) | Expressions for constant values should use `immutable` rather than `constant` | 13 |
| [NC-28](#NC-28) | Use the latest solidity version for deployment | 6 |
| [NC-29](#NC-29) | Common functions should be refactored to a common base contract | 8 |
| [NC-30](#NC-30) | Names of `private`/`internal` functions should be prefixed with an underscore | 2 |
| [NC-31](#NC-31) | Names of `private`/`internal` state variables should be prefixed with an underscore | 3 |
| [NC-32](#NC-32) |  `require()` / `revert()` statements should have descriptive reason strings | 1 |
| [NC-33](#NC-33) | Return values of `approve()` not checked | 6 |
| [NC-34](#NC-34) | Event is missing `indexed` fields | 13 |
| [NC-35](#NC-35) | Functions not used internally could be marked external | 14 |

## Gas Optimizations


Total <b>199</b> instances over <b>29</b> issues:

|ID|Issue|Instances|Gas|
|-|:-|:-:|:-:|
| [GAS-1](#GAS-1) | Consider activating via-ir for deploying | 1 | - |
| [GAS-2](#GAS-2) | Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables | 4 | 452 |
| [GAS-3](#GAS-3) | `internal` functions only called once can be inlined to save gas | 9 | 270 |
| [GAS-4](#GAS-4) | `keccak256()` hash of literals should only be computed once | 7 | 294 |
| [GAS-5](#GAS-5) | Multiple accesses of the same mapping/array key/index should be cached | 2 | 84 |
| [GAS-6](#GAS-6) | Newer versions of solidity are more gas efficient | 6 | - |
| [GAS-7](#GAS-7) | Operator `>=`/`<=` costs less gas than operator `>`/`<` | 18 | 54 |
| [GAS-8](#GAS-8) | Reduce gas usage by moving to Solidity 0.8.19 or later | 6 | 6000 |
| [GAS-9](#GAS-9) | Redundant state variable getters | 1 | - |
| [GAS-10](#GAS-10) | `require()`/`revert()` strings longer than 32 bytes cost extra gas | 3 | 9 |
| [GAS-11](#GAS-11) | The result of a function call should be cached rather than re-calling the function | 13 | 1300 |
| [GAS-12](#GAS-12) | Unused named return variables without optimizer waste gas | 3 | 27 |
| [GAS-13](#GAS-13) | Use assembly to compute hashes to save gas | 10 | 800 |
| [GAS-14](#GAS-14) | Use assembly to emit events | 20 | 760 |
| [GAS-15](#GAS-15) | Using a double `if` statement instead of a logical AND (`&&`) | 2 | 60 |
| [GAS-16](#GAS-16) | Use a more recent version of solidity | 6 | - |
| [GAS-17](#GAS-17) | `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants) | 2 | - |
| [GAS-18](#GAS-18) | Using bools for storage incurs overhead | 2 | - |
| [GAS-19](#GAS-19) | Cache array length outside of loop | 5 | - |
| [GAS-20](#GAS-20) | Use `calldata` instead of `memory` for function arguments that do not get mutated | 1 | - |
| [GAS-21](#GAS-21) | Use Custom Errors | 21 | 1050 |
| [GAS-22](#GAS-22) | Don't initialize variables with default value | 8 | - |
| [GAS-23](#GAS-23) | Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead | 1 | 55 |
| [GAS-24](#GAS-24) | Constructors can be marked as `payable` to save deployment gas | 2 | 42 |
| [GAS-25](#GAS-25) | Functions guaranteed to revert when called by normal users can be marked `payable` | 14 | 294 |
| [GAS-26](#GAS-26) | `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too) | 1 | 5 |
| [GAS-27](#GAS-27) | Using `private` rather than `public` for constants, saves gas | 12 | - |
| [GAS-28](#GAS-28) | Use `!= 0` instead of `> 0` for unsigned integer comparison | 3 | 12 |
| [GAS-29](#GAS-29) | Using assembly to check for zero can save gas | 16 | 96 |

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

165:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L165](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L165) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```
[#L131](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L131) 

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
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

437:     usdy.transferFrom(msg.sender, address(this), _USDYAmount);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L437](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L437) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L680) 

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
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

437:     usdy.transferFrom(msg.sender, address(this), _USDYAmount);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L437](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L437) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L680) 

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
[#L30](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L30) [#L210](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L210) [#L220](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L220) [#L237](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L237) [#L259](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L259) [#L286](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L286) [#L295](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L295) [#L304](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L304) [#L313](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L313) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L322) 

```solidity
File: contracts/bridge/SourceBridge.sol

11: contract SourceBridge is Ownable, Pausable, IMulticall {

124:   ) external onlyOwner {

136:   function pause() external onlyOwner {

145:   function unpause() external onlyOwner {

162:   ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L11](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L11) [#L124](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L124) [#L136](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L136) [#L145](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L145) [#L162](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L162) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

22: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

154:   ) external onlyRole(SETTER_ROLE) {

192:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

241:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

248:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L22) [#L154](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L154) [#L192](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L192) [#L241](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L241) [#L248](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L248) 

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
[#L662](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L662) [#L675](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L675) [#L685](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L685) [#L689](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L689) [#L700](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L700) [#L711](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L711) [#L722](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L722) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

81:   ) external onlyGuardian returns (address, address, address) {

128:   ) external payable override onlyGuardian returns (bytes[] memory results) {

```
[#L81](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L81) [#L128](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L128) 

</details>

---


## Low Issues

<a name="L-1"></a> 
### [L-1] Governance functions should be controlled by time locks
Governance functions (such as upgrading contracts, setting critical parameters) should be controlled using time locks to introduce a delay between a proposal and its execution. This gives users time to exit before a potentially dangerous or malicious operation is applied.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

286:   function setMintLimit(uint256 mintLimit) external onlyOwner {

295:   function setMintLimitDuration(uint256 mintDuration) external onlyOwner {

```
[#L286](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L286) [#L295](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L295) 

```solidity
File: contracts/usdy/rUSDY.sol

662:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

```
[#L662](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L662) 

</details>

---

<a name="L-2"></a> 
### [L-2] Missing storage gap for upgradable contracts
Each upgradable contract should include a state variable (usually named `__gap`) to provide reserved space in storage. This allows the team to freely add new state variables in the future upgrades without compromising the storage compatibility with existing deployments.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

76:   mapping(address => uint256) private shares;
    
      /// @dev Allowances are nominated in tokens, not token shares.

```
[#L76](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L76) 

</details>

---

<a name="L-3"></a> 
### [L-3] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

453:     _burnShares(msg.sender, usdyAmount);

455:     emit TokensBurnt(msg.sender, _rUSDYAmount);

561:     // address to `address`, but we cannot reflect this as it would require sending an unbounded

604:     // works by redistributing the amount of tokens corresponding to the burned shares between

```
[#L453](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L453) [#L455](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L455) [#L561](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L561) [#L604](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L604) 

</details>

---

<a name="L-4"></a> 
### [L-4] Missing zero address check in initializer

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
130:     __SanctionsListClientInitializable_init(sanctionsList);
         __rUSDY_init_unchained(_usdy, guardian, _oracle);
       }
     
       function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L130) 

</details>

---

<a name="L-5"></a> 
### [L-5] Initializers could be front-run
Initializers could be front-run, allowing an attacker to either set their own values, take ownership of the contract, and in the best case forcing a re-deployment

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

109:   function initialize(

```
[#L109](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L109) 

</details>

---

<a name="L-6"></a> 
### [L-6] Unsafe ERC20 operation(s)

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

324:     IRWALike(_token).transfer(owner(), balance);

```
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L324) 

```solidity
File: contracts/usdy/rUSDY.sol

437:     usdy.transferFrom(msg.sender, address(this), _USDYAmount);

454:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```
[#L437](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L437) [#L454](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L454) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L680) 

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
[#L100](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L100) 

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

11: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L11](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L11) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

18: interface IRWADynamicOracle {

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L18) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

22: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```
[#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L22) 

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
### [NC-4] Constants should be put on the left side of comparisons
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
[#L144](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L144) [#L265](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L265) 

```solidity
File: contracts/bridge/SourceBridge.sol

68:     if (bytes(destContract).length == 0) {

72:     if (msg.value == 0) {

```
[#L68](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L68) [#L72](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L72) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

198:     if (indexToModify == 0) {

218:     if (indexToModify == 0) {

284:     if (remainder >= 0.5e10) {

405:     require(y == 0 || (z = x * y) / y == x);

```
[#L198](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L198) [#L218](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L218) [#L284](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L284) [#L405](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L405) 

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
[#L490](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L490) [#L491](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L491) [#L519](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L519) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L520) [#L547](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L547) [#L579](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L579) [#L642](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L642) [#L649](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L649) 

</details>

---

<a name="NC-5"></a> 
### [NC-5] Contracts should have full test coverage
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

<a name="NC-6"></a> 
### [NC-6] Events that mark critical parameter changes should contain both the old and the new value
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
[#L113](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L113) [#L212](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L212) [#L222](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L222) [#L239](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L239) [#L278](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L278) [#L351](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L351) 

```solidity
File: contracts/bridge/SourceBridge.sol

128:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```
[#L128](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L128) 

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
[#L421](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L421) [#L423](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L423) [#L438](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L438) [#L439](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L439) [#L455](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L455) [#L470](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L470) [#L471](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L471) [#L494](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L494) [#L682](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L682) 

</details>

---

<a name="NC-7"></a> 
### [NC-7] Custom errors has no error details
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
[#L439](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L439) [#L440](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L440) [#L441](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L441) [#L443](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L443) [#L444](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L444) [#L445](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L445) [#L446](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L446) [#L447](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L447) [#L448](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L448) 

```solidity
File: contracts/bridge/SourceBridge.sol

189:   error DestinationNotSupported();

190:   error GasFeeTooLow();

```
[#L189](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L189) [#L190](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L190) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

334:   error InvalidPrice();

335:   error InvalidRange();

336:   error PriceNotSet();

```
[#L334](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L334) [#L335](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L335) [#L336](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L336) 

```solidity
File: contracts/usdy/rUSDY.sol

94:   error UnwrapTooSmall();

```
[#L94](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L94) 

</details>

---

<a name="NC-8"></a> 
### [NC-8] Custom errors should be used rather than `revert()`/`require()`
Custom errors are available from solidity version 0.8.4. Custom errors are more easily processed in try-catch blocks, and are easier to re-use and maintain.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

168:       require(success, "Call Failed");

```
[#L168](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L168) 

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
[#L307](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L307) [#L435](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L450) [#L490](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L490) [#L491](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L491) [#L519](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L519) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L520) [#L547](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L547) [#L579](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L579) [#L584](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L584) [#L634](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L634) [#L635](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L635) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L644) [#L645](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L645) [#L646](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L646) [#L651](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L651) [#L652](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L652) [#L653](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L653) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

134:       require(success, "Call Failed");

155:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L134) [#L155](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L155) 

</details>

---

<a name="NC-9"></a> 
### [NC-9] `else` block not required
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

197:   function approve(bytes32 txnHash) external {
         if (!approvers[msg.sender]) {
           revert NotApprover();
         }
         _approve(txnHash);

```
[#L197](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L197) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

97:    * @param blockTimeStamp  The unixTimestamp of the point in time you wish to simulate
       * @param dailyIR         The daily Interest Rate for the range to simulate

151:   function setRange(
         uint256 endTimestamp,
         uint256 dailyInterestRate
       ) external onlyRole(SETTER_ROLE) {
         Range memory lastRange = ranges[ranges.length - 1];

```
[#L97](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L97) [#L151](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L151) 

</details>

---

<a name="NC-10"></a> 
### [NC-10] Enable IR-based code generation
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

<a name="NC-11"></a> 
### [NC-11] Events are emitted without the sender information
When an action is triggered based on a user's action, not being able to filter based on who triggered the action makes event processing a lot more cumbersome. Including the `msg.sender` the events of these types of action will make events much more useful to end users, especially when `msg.sender` is not `tx.origin`.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

128:   function _attachThreshold(

231:    * @param srcChain            The chain to support

238:     chainToApprovedSender[srcChain] = keccak256(abi.encode(srcContractAddress));

252:    *      and will thresholds corresponding to the params of this function. Passing

302:    * @dev Only used for bridge functions

```
[#L128](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L128) [#L231](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L231) [#L238](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L238) [#L252](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L252) [#L302](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L302) 

```solidity
File: contracts/bridge/SourceBridge.sol

128:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```
[#L128](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L128) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

180:    * @param newPrevRangeClosePrice  The previous ranges close price

257:    * @notice Internal helper function used to derive the price of USDY

```
[#L180](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L180) [#L257](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L257) 

```solidity
File: contracts/usdy/rUSDY.sol

491:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

493:     allowances[_owner][_spender] = _amount;

517:     uint256 _sharesAmount

609:     // We're emitting `SharesBurnt` event to provide an explicit rebase log record nonetheless.

711:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```
[#L491](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L491) [#L493](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L493) [#L517](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L517) [#L609](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L609) [#L711](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L711) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

124:    *       3) value - eth value to call target with

```
[#L124](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L124) 

</details>

---

<a name="NC-12"></a> 
### [NC-12] Import declarations should import specific identifiers, rather than the whole file
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
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L18) [#L19](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L20) [#L21](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L21) [#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L22) [#L23](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L23) [#L24](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L24) [#L25](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L25) 

```solidity
File: contracts/bridge/SourceBridge.sol

3: import "contracts/interfaces/IAxelarGateway.sol";

4: import "contracts/interfaces/IAxelarGasService.sol";

5: import "contracts/interfaces/IMulticall.sol";

6: import "contracts/interfaces/IRWALike.sol";

8: import "contracts/external/openzeppelin/contracts/access/Ownable.sol";

9: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

```
[#L3](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L3) [#L4](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L4) [#L5](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L5) [#L6](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L6) [#L8](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L8) [#L9](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L9) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

18: import "contracts/rwaOracles/IRWAOracle.sol";

19: import "contracts/external/openzeppelin/contracts/access/AccessControlEnumerable.sol";

20: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L18) [#L19](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L20) 

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
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L18) [#L19](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L20) [#L21](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L21) [#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L22) [#L23](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L23) [#L24](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L24) [#L25](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L25) [#L26](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L26) [#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L27) [#L28](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L28) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

19: import "contracts/external/openzeppelin/contracts/proxy/ProxyAdmin.sol";

20: import "contracts/Proxy.sol";

21: import "contracts/usdy/rUSDY.sol";

22: import "contracts/interfaces/IMulticall.sol";

```
[#L19](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L19) [#L20](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L20) [#L21](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L21) [#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L22) 

</details>

---

<a name="NC-13"></a> 
### [NC-13] Large or complicated code bases should implement invariant tests
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

<a name="NC-14"></a> 
### [NC-14] Missing zero address check in functions with address parameters
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
76:   //////////////////////////////////////////////////////////////*/
    
      /**
       * @notice Internal overriden function that is executed when contract is called by Axelar Gateway
       *
       * @param srcChain The string of the source chain eg: arbitrum
       * @param srcAddr  The string of the address of the source contract

/// Missing zero check for `approver`
228:    * @notice This will initalize a nested mapping in which spent nonces from this `srcAddress`
        *         are logged and prevented from being reused

/// Missing zero check for `approver`
236:     string calldata srcContractAddress
       ) external onlyOwner {
         chainToApprovedSender[srcChain] = keccak256(abi.encode(srcContractAddress));

/// Missing zero check for `_token`
337:   function _mintIfThresholdMet(bytes32 txnHash) internal {
         bool thresholdMet = _checkThresholdMet(txnHash);
         Transaction memory txn = txnHashToTransaction[txnHash];

```
[#L76](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L76) [#L228](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L228) [#L236](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L236) [#L337](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L337) 

```solidity
File: contracts/bridge/SourceBridge.sol

/// Missing zero check for `_token`
/// Missing zero check for `_axelarGateway`
/// Missing zero check for `_gasService`
/// Missing zero check for `owner`
40:   constructor(
        address _token,
        address _axelarGateway,
        address _gasService,
        address owner
      ) {

/// Missing zero check for `contractAddress`
121:   function setDestinationChainContractAddress(
         string memory destinationChain,
         address contractAddress
       ) external onlyOwner {

```
[#L40](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L40) [#L121](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L121) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Missing zero check for `admin`
/// Missing zero check for `setter`
/// Missing zero check for `pauser`
50:   //////////////////////////////////////////////////////////////*/
    
      /**
       * @notice Function which returns the daily price of USDY given the range previously set
       *
       * @return price      The current price of USDY

```
[#L50](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L50) 

```solidity
File: contracts/usdy/rUSDY.sol

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
130:     __SanctionsListClientInitializable_init(sanctionsList);
         __rUSDY_init_unchained(_usdy, guardian, _oracle);
       }
     
       function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
141:     _grantRole(DEFAULT_ADMIN_ROLE, guardian);
         _grantRole(USDY_MANAGER_ROLE, guardian);
         _grantRole(PAUSER_ROLE, guardian);
         _grantRole(MINTER_ROLE, guardian);
         _grantRole(BURNER_ROLE, guardian);

/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
154:   event TransferShares(
         address indexed from,
         address indexed to,
         uint256 sharesValue
       );
     
       /**
        * @notice An executed `burnShares` request

/// Missing zero check for `_account`
243:    * @dev The `_amount` argument is the amount of tokens, not shares.
        */
       function transfer(address _recipient, uint256 _amount) public returns (bool) {

/// Missing zero check for `_recipient`
264:    * @notice Sets `_amount` as the allowance of `_spender` over the caller's tokens.
        *
        * @return a boolean value indicating whether the operation succeeded.

/// Missing zero check for `_spender`
294:    * - `_sender` and `_recipient` cannot be the zero addresses.
        * - `_sender` must have a balance of at least `_amount`.
        * - the caller must have allowance for `_sender`'s tokens of at least `_amount`.

/// Missing zero check for `_account`
402:    * @notice Moves `_sharesAmount` token shares from the caller's account to the `_recipient` account.

/// Missing zero check for `_sender`
/// Missing zero check for `_recipient`
483:    * - the contract must not be paused.
        */
       function _approve(
         address _owner,
         address _spender,
         uint256 _amount

/// Missing zero check for `_account`
520:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");
     
         _beforeTokenTransfer(_sender, _recipient, _sharesAmount);

/// Missing zero check for `_oracle`
680:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);
     
         emit TokensBurnt(_account, _amount);
       }
     
       function pause() external onlyRole(PAUSER_ROLE) {

/// Missing zero check for `_account`
700:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {
         _setBlocklist(blocklist);
       }
     
       /**
        * @notice Sets the allowlist address

/// Missing zero check for `blocklist`
723:     _setSanctionsList(sanctionsList);
       }
     }
     

/// Missing zero check for `allowlist`
726: 

/// Missing zero check for `sanctionsList`
726: 

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L130) [#L141](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L141) [#L154](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L154) [#L243](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L243) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L264) [#L294](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L294) [#L402](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L402) [#L483](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L483) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L520) [#L680](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L680) [#L700](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L700) [#L723](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L723) [#L726](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L726) [#L726](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L726) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing zero check for `_guardian`
67:    * @notice 1) Will automatically revoke all deployer roles granted to
       *            address(this).

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `usdy`
/// Missing zero check for `oracle`
99:     rUSDYProxyAdmin.transferOwnership(guardian);
        assert(rUSDYProxyAdmin.owner() == guardian);
        emit rUSDYDeployed(
          address(rUSDYProxy),
          address(rUSDYProxyAdmin),
          address(rUSDYImplementation),
          "Ondo Rebasing U.S. Dollar Yield",

```
[#L67](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L67) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L99) 

</details>

---

<a name="NC-15"></a> 
### [NC-15] Consider moving `msg.sender` checks to `modifier`s
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
[#L634](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L634) [#L635](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L635) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

155:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```
[#L155](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L155) 

</details>

---

<a name="NC-16"></a> 
### [NC-16] Named mappings are recommended
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
[#L43](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L43) [#L44](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L44) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L45) [#L51](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L51) [#L52](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L52) [#L53](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L53) 

```solidity
File: contracts/bridge/SourceBridge.sol

15:   mapping(string => string) public destChainToContractAddr;

```
[#L15](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L15) 

```solidity
File: contracts/usdy/rUSDY.sol

76:   mapping(address => uint256) private shares;

79:   mapping(address => mapping(address => uint256)) private allowances;

```
[#L76](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L76) [#L79](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L79) 

</details>

---

<a name="NC-17"></a> 
### [NC-17] NatSpec documentation for contract is missing
e.g. `@dev` or `@notice`, and it must appear above the contract definition braces in order to be identified by the compiler as NatSpec.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

11: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L11](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L11) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

18: interface IRWADynamicOracle {

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L18) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

22: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```
[#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L22) 

</details>

---

<a name="NC-18"></a> 
### [NC-18] NatSpec documentation for function is missing
It is recommended that Solidity contracts are fully annotated using NatSpec for all public interfaces (everything in the ABI). It is clearly stated in the Solidity official documentation. In complex projects such as DeFi, the interpretation of all functions and their arguments and returns is important for code readability and auditability.

<details>
<summary>
There are <b>11</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

76:   //////////////////////////////////////////////////////////////*/
    
      /**
       * @notice Internal overriden function that is executed when contract is called by Axelar Gateway
       *
       * @param srcChain The string of the source chain eg: arbitrum
       * @param srcAddr  The string of the address of the source contract

```
[#L76](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L76) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

50:   //////////////////////////////////////////////////////////////*/
    
      /**
       * @notice Function which returns the daily price of USDY given the range previously set
       *
       * @return price      The current price of USDY

377:             revert(0, 0)
               }
               let xxRound := add(xx, half)
               if lt(xxRound, xx) {
                 revert(0, 0)

408: 

408: 

```
[#L50](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L50) [#L377](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L377) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) 

```solidity
File: contracts/usdy/rUSDY.sol

130:     __SanctionsListClientInitializable_init(sanctionsList);
         __rUSDY_init_unchained(_usdy, guardian, _oracle);
       }
     
       function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

141:     _grantRole(DEFAULT_ADMIN_ROLE, guardian);
         _grantRole(USDY_MANAGER_ROLE, guardian);
         _grantRole(PAUSER_ROLE, guardian);
         _grantRole(MINTER_ROLE, guardian);
         _grantRole(BURNER_ROLE, guardian);

154:   event TransferShares(
         address indexed from,
         address indexed to,
         uint256 sharesValue
       );
     
       /**
        * @notice An executed `burnShares` request

712:     _setAllowlist(allowlist);
       }
     
       /**
        * @notice Sets the sanctions list address

718:    * @param sanctionsList New sanctions list address
        */
       function setSanctionsList(

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L130) [#L141](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L141) [#L154](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L154) [#L712](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L712) [#L718](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L718) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

67:    * @notice 1) Will automatically revoke all deployer roles granted to
       *            address(this).

```
[#L67](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L67) 

</details>

---

<a name="NC-19"></a> 
### [NC-19] Modifier declarations should have NatSpec descriptions

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

159: 

```
[#L159](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L159) 

</details>

---

<a name="NC-20"></a> 
### [NC-20] Missing NatSpec `@param`
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
76:   //////////////////////////////////////////////////////////////*/
    
      /**
       * @notice Internal overriden function that is executed when contract is called by Axelar Gateway
       *
       * @param srcChain The string of the source chain eg: arbitrum
       * @param srcAddr  The string of the address of the source contract

```
[#L76](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L76) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Missing @param for admin
/// Missing @param for setter
/// Missing @param for pauser
/// Missing @param for firstRangeStart
/// Missing @param for firstRangeEnd
/// Missing @param for dailyIR
/// Missing @param for startPrice
50:   //////////////////////////////////////////////////////////////*/
    
      /**
       * @notice Function which returns the daily price of USDY given the range previously set
       *
       * @return price      The current price of USDY

/// Missing @param for x
/// Missing @param for n
/// Missing @param for base
377:             revert(0, 0)
               }
               let xxRound := add(xx, half)
               if lt(xxRound, xx) {
                 revert(0, 0)

/// Missing @param for x
/// Missing @param for y
408: 

/// Missing @param for x
/// Missing @param for y
408: 

```
[#L50](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L50) [#L377](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L377) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) 

```solidity
File: contracts/usdy/rUSDY.sol

/// Missing @param for blocklist
/// Missing @param for allowlist
/// Missing @param for sanctionsList
/// Missing @param for _usdy
/// Missing @param for guardian
/// Missing @param for _oracle
130:     __SanctionsListClientInitializable_init(sanctionsList);
         __rUSDY_init_unchained(_usdy, guardian, _oracle);
       }
     
       function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing @param for blocklist
/// Missing @param for allowlist
/// Missing @param for sanctionsList
/// Missing @param for _usdy
/// Missing @param for guardian
/// Missing @param for _oracle
141:     _grantRole(DEFAULT_ADMIN_ROLE, guardian);
         _grantRole(USDY_MANAGER_ROLE, guardian);
         _grantRole(PAUSER_ROLE, guardian);
         _grantRole(MINTER_ROLE, guardian);
         _grantRole(BURNER_ROLE, guardian);

/// Missing @param for _usdy
/// Missing @param for guardian
/// Missing @param for _oracle
154:   event TransferShares(
         address indexed from,
         address indexed to,
         uint256 sharesValue
       );
     
       /**
        * @notice An executed `burnShares` request

/// Missing @param for _account
243:    * @dev The `_amount` argument is the amount of tokens, not shares.
        */
       function transfer(address _recipient, uint256 _amount) public returns (bool) {

/// Missing @param for _recipient
/// Missing @param for _amount
264:    * @notice Sets `_amount` as the allowance of `_spender` over the caller's tokens.
        *
        * @return a boolean value indicating whether the operation succeeded.

/// Missing @param for _owner
/// Missing @param for _spender
277:     _approve(msg.sender, _spender, _amount);
         return true;
       }
     
       /**
        * @notice Moves `_amount` tokens from `_sender` to `_recipient` using the

/// Missing @param for _spender
/// Missing @param for _amount
294:    * - `_sender` and `_recipient` cannot be the zero addresses.
        * - `_sender` must have a balance of at least `_amount`.
        * - the caller must have allowance for `_sender`'s tokens of at least `_amount`.

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _amount
319:    * https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/IERC20.sol#L42
        * Emits an `Approval` event indicating the updated allowance.

/// Missing @param for _spender
/// Missing @param for _addedValue
345:    * Emits an `Approval` event indicating the updated allowance.
        *
        * Requirements:
        *
        * - `_spender` cannot be the zero address.
        * - `_spender` must have allowance for the caller of at least `_subtractedValue`.

/// Missing @param for _spender
/// Missing @param for _subtractedValue
372:   function getTotalShares() public view returns (uint256) {
         return totalShares;
       }
     
       /**
        * @return the amount of shares owned by `_account`.

/// Missing @param for _account
402:    * @notice Moves `_sharesAmount` token shares from the caller's account to the `_recipient` account.

/// Missing @param for _rUSDYAmount
406:    * Emits a `Transfer` event.
        *
        * Requirements:
        *
        * - `_recipient` cannot be the zero address.
        * - the caller must have at least `_sharesAmount` shares.

/// Missing @param for _shares
414:    * @dev The `_sharesAmount` argument is the amount of shares, not tokens.
        */
       function transferShares(
         address _recipient,
         uint256 _sharesAmount

/// Missing @param for _recipient
/// Missing @param for _sharesAmount
434:   function wrap(uint256 _USDYAmount) external whenNotPaused {
         require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _amount
483:    * - the contract must not be paused.
        */
       function _approve(
         address _owner,
         address _spender,
         uint256 _amount

/// Missing @param for _owner
/// Missing @param for _spender
/// Missing @param for _amount
509:    * - `_sender` cannot be the zero address.
        * - `_recipient` cannot be the zero address.
        * - `_sender` must hold at least `_sharesAmount` shares.

/// Missing @param for _account
520:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");
     
         _beforeTokenTransfer(_sender, _recipient, _sharesAmount);

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _sharesAmount
535:    * @notice Creates `_sharesAmount` shares and assigns them to `_recipient`, increasing the total amount of shares.
        * @dev This doesn't increase the token total supply.

/// Missing @param for _recipient
/// Missing @param for _sharesAmount
559:     // token holders, proportionally to their share. The total supply of the token doesn't change
         // as the result. This is equivalent to performing a send from each other token holder's

/// Missing @param for _account
/// Missing @param for _sharesAmount
594:     emit SharesBurnt(
           _account,
           preRebaseTokenAmount,
           postRebaseTokenAmount,
           _sharesAmount
         );
     
         return totalShares;

/// Missing @param for from
/// Missing @param for to
644:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");
           require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L130) [#L141](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L141) [#L154](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L154) [#L243](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L243) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L264) [#L277](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L277) [#L294](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L294) [#L319](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L319) [#L345](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L345) [#L372](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L372) [#L402](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L402) [#L406](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L406) [#L414](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L414) [#L434](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L434) [#L483](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L483) [#L509](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L509) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L520) [#L535](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L535) [#L559](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L559) [#L594](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L594) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L644) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing @param for _guardian
67:    * @notice 1) Will automatically revoke all deployer roles granted to
       *            address(this).

/// Missing @param for oracle
99:     rUSDYProxyAdmin.transferOwnership(guardian);
        assert(rUSDYProxyAdmin.owner() == guardian);
        emit rUSDYDeployed(
          address(rUSDYProxy),
          address(rUSDYProxyAdmin),
          address(rUSDYImplementation),
          "Ondo Rebasing U.S. Dollar Yield",

```
[#L67](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L67) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L99) 

</details>

---

<a name="NC-21"></a> 
### [NC-21] Public variable declarations should have NatSpec descriptions

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

60:     address _owner,

64:     AxelarExecutable(_axelarGateway)

74:   /*//////////////////////////////////////////////////////////////

75:                          Axelar Functions

```
[#L60](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L60) [#L64](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L64) [#L74](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L74) [#L75](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L75) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

45:     ranges.push(Range(firstRangeStart, firstRangeEnd, dailyIR, trueStart));

```
[#L45](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L45) 

```solidity
File: contracts/usdy/rUSDY.sol

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

104:   /// @custom:oz-upgrades-unsafe-allow constructor

```
[#L101](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L101) [#L104](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L104) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

65:    * @return address The address of the implementation contract.

66:    *

67:    * @notice 1) Will automatically revoke all deployer roles granted to

```
[#L65](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L65) [#L66](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L66) [#L67](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L67) 

</details>

---

<a name="NC-22"></a> 
### [NC-22] NatSpec `@return` is missing
It is recommended that Solidity contracts are fully annotated using NatSpec

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

193:    *         approver that is added and associated with Ondo.
        *
        * @param txnHash The keccak256 hash of the payload

385:    * @notice event emitted when an address is removed as an approver
        *
        * @param approver The address being removed
        */

```
[#L193](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L193) [#L385](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L385) 

```solidity
File: contracts/bridge/SourceBridge.sol

160:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L160](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L160) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

22: 

```
[#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L22) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

121:       uint256 prevClosePrice = derivePrice(lastRange, lastRange.end - 1);
           rangeList[length] = Range(
             lastRange.end,
             endTime,
             dailyIR,
             prevClosePrice
           );
         }

283:     uint256 remainder = value % 1e10;
         if (remainder >= 0.5e10) {
           value += 1e10;
         }
         value -= remainder;
         return value;

305:    * @param start             The start time for the range
        * @param end               The end time for the range

377:             revert(0, 0)
               }
               let xxRound := add(xx, half)
               if lt(xxRound, xx) {
                 revert(0, 0)

408: 

408: 

```
[#L121](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L121) [#L283](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L283) [#L305](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L305) [#L377](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L377) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) 

```solidity
File: contracts/usdy/rUSDY.sol

345:    * Emits an `Approval` event indicating the updated allowance.
        *
        * Requirements:
        *
        * - `_spender` cannot be the zero address.
        * - `_spender` must have allowance for the caller of at least `_subtractedValue`.

372:   function getTotalShares() public view returns (uint256) {
         return totalShares;
       }
     
       /**
        * @return the amount of shares owned by `_account`.

559:     // token holders, proportionally to their share. The total supply of the token doesn't change
         // as the result. This is equivalent to performing a send from each other token holder's

594:     emit SharesBurnt(
           _account,
           preRebaseTokenAmount,
           postRebaseTokenAmount,
           _sharesAmount
         );
     
         return totalShares;

```
[#L345](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L345) [#L372](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L372) [#L559](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L559) [#L594](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L594) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

143:    * @param proxyAdmin        The address for the proxy admin contract
        * @param implementation    The address for the implementation contract
        */
       event rUSDYDeployed(

```
[#L143](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L143) 

</details>

---

<a name="NC-23"></a> 
### [NC-23] State variables should include comments
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
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L44) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L45) [#L52](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L52) [#L53](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L53) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

23:   uint256 public constant DAY = 1 days;

27:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

28:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L23](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L23) [#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L27) [#L28](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L28) 

```solidity
File: contracts/usdy/rUSDY.sol

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L98](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L101) 

</details>

---

<a name="NC-24"></a> 
### [NC-24] Contract declarations should have NatSpec `@title` annotations
Some contract definitions have an incomplete NatSpec: add a `@title` notation to describe the contract to improve the code documentation.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

11: contract SourceBridge is Ownable, Pausable, IMulticall {

```
[#L11](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L11) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

18: interface IRWADynamicOracle {

```
[#L18](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L18) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

22: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```
[#L22](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L22) 

</details>

---

<a name="NC-25"></a> 
### [NC-25] Unused named return
Declaring named returns, but not using them, is confusing to the reader. Consider either completely removing them (by declaring just the type without a name), or remove the return statement and do a variable assignment. This would improve the readability of the code, and it may also help reduce regressions during future code refactors.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `price` not used
93:    * @dev If you are simulating the first range, you MUST set `startTime` and `rangeStartPrice`

/// `price` not used
121:       uint256 prevClosePrice = derivePrice(lastRange, lastRange.end - 1);
           rangeList[length] = Range(
             lastRange.end,
             endTime,
             dailyIR,
             prevClosePrice
           );
         }

/// `price` not used
283:     uint256 remainder = value % 1e10;
         if (remainder >= 0.5e10) {
           value += 1e10;
         }
         value -= remainder;
         return value;

```
[#L93](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L93) [#L121](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L121) [#L283](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L283) 

</details>

---

<a name="NC-26"></a> 
### [NC-26] Consider using `delete` rather than assigning zero to clear values
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
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L164](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L164) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

77:     for (uint256 i = 0; i < length; ++i) {

113:     for (uint256 i = 0; i < length; ++i) {

129:     for (uint256 i = 0; i < length + 1; ++i) {

```
[#L77](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L77) [#L113](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L113) [#L129](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L129) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="NC-27"></a> 
### [NC-27] Expressions for constant values should use `immutable` rather than `constant`
While it doesn't save any gas because the compiler knows that developers often make this mistake, it's still best to use the right tool for the task at hand. There is a difference between `constant` variables and `immutable` variables, and they should each be used in their appropriate contexts. `constants` should be used for literal values written into the code, and `immutable` variables should be used for expressions, or values calculated in, or passed into the constructor.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

48:   bytes32 public constant VERSION = "1.0";

```
[#L48](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L48) 

```solidity
File: contracts/bridge/SourceBridge.sol

27:   bytes32 public constant VERSION = "1.0";

```
[#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L27) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

23:   uint256 public constant DAY = 1 days;

27:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

28:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

343:   uint256 private constant ONE = 10 ** 27;

```
[#L23](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L23) [#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L27) [#L28](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L28) [#L343](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L343) 

```solidity
File: contracts/usdy/rUSDY.sol

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L91](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L91) [#L97](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L101) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

44:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L44) 

</details>

---

<a name="NC-28"></a> 
### [NC-28] Use the latest solidity version for deployment
Upgrading to a newer Solidity release can optimize gas usage, take advantage of new features and improve overall contract efficiency. Where possible, based on compatibility requirements, it is recommended to use newer/latest solidity version to take advantage of the latest optimizations and features.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L1) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L16) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="NC-29"></a> 
### [NC-29] Common functions should be refactored to a common base contract
The functions below have the same implementation as is seen in other files. The functions should be refactored into functions of a common base contract.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// Seen in contracts/bridge/SourceBridge.sol
327:   /*//////////////////////////////////////////////////////////////
                             Public Functions

/// Seen in contracts/bridge/SourceBridge.sol
332:    * @notice internal function to mint a transaction if it has passed the threshold
        *         for the number of approvers

```
[#L327](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L327) [#L332](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L332) 

```solidity
File: contracts/bridge/SourceBridge.sol

/// Seen in contracts/bridge/DestinationBridge.sol
136:   function pause() external onlyOwner {

/// Seen in contracts/bridge/DestinationBridge.sol
145:   function unpause() external onlyOwner {

/// Seen in contracts/usdy/rUSDYFactory.sol
160:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyOwner returns (bytes[] memory results) {

```
[#L136](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L136) [#L145](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L145) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L160) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Seen in contracts/bridge/SourceBridge.sol
260:    * @param currentTime  The current unixTimestamp of the blockchain
        */
       function derivePrice(
         Range memory currentRange,

/// Seen in contracts/bridge/SourceBridge.sol
265:   ) internal pure returns (uint256 price) {
         uint256 elapsedDays = (currentTime - currentRange.start) / DAY;

```
[#L260](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L260) [#L265](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L265) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Seen in contracts/bridge/SourceBridge.sol
143:    * @param proxyAdmin        The address for the proxy admin contract
        * @param implementation    The address for the implementation contract
        */
       event rUSDYDeployed(

```
[#L143](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L143) 

</details>

---

<a name="NC-30"></a> 
### [NC-30] Names of `private`/`internal` functions should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

283:     uint256 remainder = value % 1e10;
         if (remainder >= 0.5e10) {
           value += 1e10;
         }
         value -= remainder;
         return value;

305:    * @param start             The start time for the range
        * @param end               The end time for the range

```
[#L283](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L283) [#L305](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L305) 

</details>

---

<a name="NC-31"></a> 
### [NC-31] Names of `private`/`internal` state variables should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

```
[#L97](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L98) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L100) 

</details>

---

<a name="NC-32"></a> 
### [NC-32]  `require()` / `revert()` statements should have descriptive reason strings

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

408: 

```
[#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) 

</details>

---

<a name="NC-33"></a> 
### [NC-33] Return values of `approve()` not checked
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
[#L111](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L111) [#L201](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L201) 

```solidity
File: contracts/usdy/rUSDY.sol

277:     _approve(msg.sender, _spender, _amount);

310:     _approve(_sender, msg.sender, currentAllowance - _amount);

331:     _approve(

362:     _approve(msg.sender, _spender, currentAllowance - _subtractedValue);

```
[#L277](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L277) [#L310](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L310) [#L331](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L331) [#L362](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L362) 

</details>

---

<a name="NC-34"></a> 
### [NC-34] Event is missing `indexed` fields
Index event fields make the field more quickly accessible to off-chain tools that parse events. However, note that each index field costs extra gas during emission, so it's not necessarily best to index the maximum allowed per event (three fields). Each event should use three indexed fields if there are three or more fields, and gas usage is not particularly of concern for the events in question. If there are fewer than three fields, all of the fields should be indexed.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

410:    * @param chain           The chain for which the threshold was set

412:    * @param numOfApprovers  The number of approvals needed

420:    * @param amount  The amount of tokens that have been minted

429:    * @param amt       The amount of tokens being bridged

441:   error ThresholdsNotInAscendingOrder();

450: 

```
[#L410](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L410) [#L412](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L412) [#L420](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L420) [#L429](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L429) [#L441](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L441) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L450) 

```solidity
File: contracts/bridge/SourceBridge.sol

183:   event DestinationChainContractAddressSet(

```
[#L183](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L183) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

324:    * @param newPrevRangeClosePrice The new prevRangeClosePrice for the modified range

349:   ) internal pure returns (uint256 z) {

```
[#L324](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L324) [#L349](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L349) 

```solidity
File: contracts/usdy/rUSDY.sol

170:    * @param sharesAmount amount of burnt shares

194:   function name() public pure returns (string memory) {

214:    * @return the amount of tokens in existence.

```
[#L170](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L170) [#L194](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L194) [#L214](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L214) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

159: 

```
[#L159](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L159) 

</details>

---

<a name="NC-35"></a> 
### [NC-35] Functions not used internally could be marked external

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

217:     return (totalShares * oracle.getPrice()) / (1e18 * BPS_DENOMINATOR);

224:    *      by the price of USDY

231:    * @notice Moves `_amount` tokens from the caller's account to the `_recipient` account.

233:    * @return a boolean value indicating whether the operation succeeded.

243:    * @dev The `_amount` argument is the amount of tokens, not shares.

264:    * @notice Sets `_amount` as the allowance of `_spender` over the caller's tokens.

277:     _approve(msg.sender, _spender, _amount);

294:    * - `_sender` and `_recipient` cannot be the zero addresses.

319:    * https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/IERC20.sol#L42

345:    * Emits an `Approval` event indicating the updated allowance.

372:   function getTotalShares() public view returns (uint256) {

395:    * @return the amount of rUSDY that corresponds to `_shares` of usdy.

402:    * @notice Moves `_sharesAmount` token shares from the caller's account to the `_recipient` account.

434:   function wrap(uint256 _USDYAmount) external whenNotPaused {

```
[#L217](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L217) [#L224](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L224) [#L231](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L231) [#L233](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L233) [#L243](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L243) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L264) [#L277](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L277) [#L294](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L294) [#L319](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L319) [#L345](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L345) [#L372](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L372) [#L395](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L395) [#L402](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L402) [#L434](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L434) 

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
### [GAS-2] Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

285:       value += 1e10;

287:     value -= remainder;

```
[#L285](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L285) [#L287](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L287) 

```solidity
File: contracts/usdy/rUSDY.sol

551:     totalShares += _sharesAmount;

588:     totalShares -= _sharesAmount;

```
[#L551](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L551) [#L588](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L588) 

</details>

---

<a name="GAS-3"></a> 
### [GAS-3] `internal` functions only called once can be inlined to save gas
If an `internal` function is only used once, there is no need to modularize it, unless the function calling it would otherwise be too long and complex. Not inlining costs 20 to 40 gas because of two extra JUMP instructions and additional stack operations needed for function calls.

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `_attachThreshold` is used only once
150:    * @notice Internal function used to approve and conditionally mint for a

/// `_checkThresholdMet` is used only once
193:    *         approver that is added and associated with Ondo.

```
[#L150](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L150) [#L193](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L193) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `roundUpTo8` is used only once
305:    * @param start             The start time for the range

/// `_rpow` is used only once
377:             revert(0, 0)

/// `_rmul` is used only once
408: 

/// `_mul` is used only once
408: 

```
[#L305](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L305) [#L377](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L377) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) 

```solidity
File: contracts/usdy/rUSDY.sol

/// `__rUSDY_init` is used only once
141:     _grantRole(DEFAULT_ADMIN_ROLE, guardian);

/// `__rUSDY_init_unchained` is used only once
154:   event TransferShares(

/// `_mintShares` is used only once
559:     // token holders, proportionally to their share. The total supply of the token doesn't change

```
[#L141](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L141) [#L154](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L154) [#L559](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L559) 

</details>

---

<a name="GAS-4"></a> 
### [GAS-4] `keccak256()` hash of literals should only be computed once
The result of the hash should be stored in an immutable variable, and the variable should be used instead. If the hash is being used as a part of a function selector, the cast to `bytes4` should also only be done once.

<details>
<summary>
There are <b>7</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

27:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

28:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L27) [#L28](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L28) 

```solidity
File: contracts/usdy/rUSDY.sol

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

102:     keccak256("LIST_CONFIGURER_ROLE");

```
[#L97](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L100) [#L102](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L102) 

</details>

---

<a name="GAS-5"></a> 
### [GAS-5] Multiple accesses of the same mapping/array key/index should be cached
The instances below point to the second+ access of a value inside a mapping/array, within a function. Caching a mapping's value in a local `storage` or `calldata` variable when the value is accessed [multiple times](https://gist.github.com/IllIllI000/ec23a57daa30a8f8ca8b9681c8ccefb0), saves ~42 gas per access due to not having to recalculate the key's keccak256 hash (Gkeccak256 - 30 gas) and that calculation's associated stack operations. Caching an array's struct avoids recalculating the array offsets into memory/calldata

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `ranges[indexToModify - 1]` is also accessed on line 207
212:       if (newStart < ranges[indexToModify - 1].end) revert InvalidRange();

/// `ranges[indexToModify]` is also accessed on line 220
222:       ranges[indexToModify] = Range(

```
[#L212](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L212) [#L222](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L222) 

</details>

---

<a name="GAS-6"></a> 
### [GAS-6] Newer versions of solidity are more gas efficient
The solidity language continues to pursue more efficient gas optimization schemes. Adopting a newer version of solidity can be more gas efficient.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L1) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L16) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="GAS-7"></a> 
### [GAS-7] Operator `>=`/`<=` costs less gas than operator `>`/`<`
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
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L134) [#L159](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L159) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L264) [#L270](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L270) 

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L164](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L164) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

77:     for (uint256 i = 0; i < length; ++i) {

113:     for (uint256 i = 0; i < length; ++i) {

129:     for (uint256 i = 0; i < length + 1; ++i) {

201:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)

201:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)

207:       if (newStart < ranges[indexToModify - 1].end) revert InvalidRange();

212:       if (newStart < ranges[indexToModify - 1].end) revert InvalidRange();

214:       if (newEnd > ranges[indexToModify + 1].start) revert InvalidRange();

```
[#L77](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L77) [#L113](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L113) [#L129](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L129) [#L201](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L201) [#L201](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L201) [#L207](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L207) [#L212](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L212) [#L214](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L214) 

```solidity
File: contracts/usdy/rUSDY.sol

435:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

452:     if (usdyAmount < BPS_DENOMINATOR) revert UnwrapTooSmall();

```
[#L435](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L450) [#L452](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L452) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="GAS-8"></a> 
### [GAS-8] Reduce gas usage by moving to Solidity 0.8.19 or later
Solidity version 0.8.19 introduced a number of gas optimizations, refer to the [Solidity 0.8.19 Release Announcement](https://soliditylang.org/blog/2023/02/22/solidity-0.8.19-release-announcement/) for details.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L1) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L16) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="GAS-9"></a> 
### [GAS-9] Redundant state variable getters
Getters for public state variables are automatically generated so there is no need to code them manually and waste gas.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

395:    * @return the amount of rUSDY that corresponds to `_shares` of usdy.
        */

```
[#L395](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L395) 

</details>

---

<a name="GAS-10"></a> 
### [GAS-10] `require()`/`revert()` strings longer than 32 bytes cost extra gas
Each extra memory word of bytes past the original 32 [incurs an MSTORE](https://gist.github.com/hrkrshnn/ee8fabd532058307229d65dcd5836ddc#consider-having-short-revert-strings) which costs 3 gas

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

322:    * Requirements:
        *
        * - `_spender` cannot be the the zero address.

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

468:     uint256 _sharesToTransfer = getSharesByRUSDY(_amount);

```
[#L322](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L322) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L450) [#L468](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L468) 

</details>

---

<a name="GAS-11"></a> 
### [GAS-11] The result of a function call should be cached rather than re-calling the function
The function calls in solidity are expensive. If the same result of the same function calls are to be used several times, the result should be cached to reduce the gas consumption of repeated calls.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `keccak256` is called 2 times
102:     if (isSpentNonce[chainToApprovedSender[srcChain]][nonce]) {
           revert NonceSpent();
         }
     
         isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;
     
         bytes32 txnHash = keccak256(payload);

/// `Threshold` is called 2 times
273:         chainToThresholds[srcChain].push(
               Threshold(amounts[i], numOfApprovers[i])
             );
           }
         }
         emit ThresholdSet(srcChain, amounts, numOfApprovers);

/// `IRWALike` is called 2 times
337:   function _mintIfThresholdMet(bytes32 txnHash) internal {
         bool thresholdMet = _checkThresholdMet(txnHash);
         Transaction memory txn = txnHashToTransaction[txnHash];

```
[#L102](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L102) [#L273](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L273) [#L337](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L337) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `derivePrice` is called 2 times
93:    * @dev If you are simulating the first range, you MUST set `startTime` and `rangeStartPrice`

/// `derivePrice` is called 3 times
121:       uint256 prevClosePrice = derivePrice(lastRange, lastRange.end - 1);
           rangeList[length] = Range(
             lastRange.end,
             endTime,
             dailyIR,
             prevClosePrice
           );
         }

/// `Range` is called 2 times
121:       uint256 prevClosePrice = derivePrice(lastRange, lastRange.end - 1);
           rangeList[length] = Range(
             lastRange.end,
             endTime,
             dailyIR,
             prevClosePrice
           );
         }

/// `InvalidRange` is called 5 times
201:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)
             revert InvalidRange();
         }
         // Case 2: The range being modified is the last range
         else if (indexToModify == rangeLength - 1) {
           // Ensure that the newStart time is not less than the end time of the previous range

/// `Range` is called 2 times
201:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)
             revert InvalidRange();
         }
         // Case 2: The range being modified is the last range
         else if (indexToModify == rangeLength - 1) {
           // Ensure that the newStart time is not less than the end time of the previous range

```
[#L93](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L93) [#L121](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L121) [#L121](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L121) [#L201](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L201) [#L201](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L201) 

```solidity
File: contracts/usdy/rUSDY.sol

/// `_grantRole` is called 6 times
154:   event TransferShares(
         address indexed from,
         address indexed to,
         uint256 sharesValue
       );
     
       /**
        * @notice An executed `burnShares` request

/// `getRUSDYByShares` is called 2 times
594:     emit SharesBurnt(
           _account,
           preRebaseTokenAmount,
           postRebaseTokenAmount,
           _sharesAmount
         );
     
         return totalShares;

/// `_isBlocked` is called 3 times
644:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");
           require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

/// `_isSanctioned` is called 3 times
644:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");
           require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

/// `_isAllowed` is called 3 times
644:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");
           require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

```
[#L154](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L154) [#L594](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L594) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L644) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L644) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L644) 

</details>

---

<a name="GAS-12"></a> 
### [GAS-12] Unused named return variables without optimizer waste gas
Consider changing the variable to be an unnamed one, since the variable is never assigned, nor is it returned by name. If the optimizer is not turned on, leaving the code as it is will also waste gas for the stack variable.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// `price` not used
93:    * @dev If you are simulating the first range, you MUST set `startTime` and `rangeStartPrice`

/// `price` not used
121:       uint256 prevClosePrice = derivePrice(lastRange, lastRange.end - 1);
           rangeList[length] = Range(
             lastRange.end,
             endTime,
             dailyIR,
             prevClosePrice
           );
         }

/// `price` not used
283:     uint256 remainder = value % 1e10;
         if (remainder >= 0.5e10) {
           value += 1e10;
         }
         value -= remainder;
         return value;

```
[#L93](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L93) [#L121](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L121) [#L283](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L283) 

</details>

---

<a name="GAS-13"></a> 
### [GAS-13] Use assembly to compute hashes to save gas
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
[#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L99) [#L108](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L108) [#L238](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L238) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

27:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

28:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L27) [#L28](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L28) 

```solidity
File: contracts/usdy/rUSDY.sol

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

102:     keccak256("LIST_CONFIGURER_ROLE");

```
[#L97](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L100) [#L102](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L102) 

</details>

---

<a name="GAS-14"></a> 
### [GAS-14] Use assembly to emit events
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
[#L113](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L113) [#L212](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L212) [#L222](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L222) [#L239](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L239) [#L278](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L278) [#L351](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L351) 

```solidity
File: contracts/bridge/SourceBridge.sol

128:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```
[#L128](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L128) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

164:     emit RangeSet(

229:     emit RangeOverriden(

```
[#L164](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L164) [#L229](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L229) 

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
[#L421](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L421) [#L423](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L423) [#L438](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L438) [#L439](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L439) [#L455](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L455) [#L470](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L470) [#L471](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L471) [#L494](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L494) [#L594](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L594) [#L682](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L682) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

101:     emit rUSDYDeployed(

```
[#L101](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L101) 

</details>

---

<a name="GAS-15"></a> 
### [GAS-15] Using a double `if` statement instead of a logical AND (`&&`)
Using a double `if` statement instead of a logical AND (`&&`) can provide similar short-circuiting behavior whereas double if is slightly [more gas efficient](https://gist.github.com/DadeKuma/931ce6794a050201ec6544dbcc31316c).

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

201:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)

```
[#L201](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L201) 

```solidity
File: contracts/usdy/rUSDY.sol

633:     if (from != msg.sender && to != msg.sender) {

```
[#L633](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L633) 

</details>

---

<a name="GAS-16"></a> 
### [GAS-16] Use a more recent version of solidity
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
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L16) 

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```
[#L1](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L1) 

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/IRWADynamicOracle.sol#L16) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L16) 

```solidity
File: contracts/usdy/rUSDY.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L16) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

16: pragma solidity 0.8.16;

```
[#L16](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L16) 

</details>

---

<a name="GAS-17"></a> 
### [GAS-17] `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants)
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

550: 

566:    * @notice Destroys `_sharesAmount` shares from `_account`'s holdings, decreasing the total amount of shares.

```
[#L550](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L550) [#L566](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L566) 

</details>

---

<a name="GAS-18"></a> 
### [GAS-18] Using bools for storage incurs overhead
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
[#L43](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L43) [#L45](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L45) 

</details>

---

<a name="GAS-19"></a> 
### [GAS-19] Cache array length outside of loop
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
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L164](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L164) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="GAS-20"></a> 
### [GAS-20] Use `calldata` instead of `memory` for function arguments that do not get mutated
Mark data types as `calldata` instead of `memory` where possible. This makes it so that the data is not automatically loaded into memory. If the data passed into the function does not need to be changed (like updating values in an array), it can be passed in as `calldata`. The one exception to this is if the argument must later be passed into another function that takes an argument that specifies `memory` storage.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

122:     string memory destinationChain,

```
[#L122](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L122) 

</details>

---

<a name="GAS-21"></a> 
### [GAS-21] Use Custom Errors
[Source](https://blog.soliditylang.org/2021/04/21/custom-errors/)
Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

168:       require(success, "Call Failed");

```
[#L168](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L168) 

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
[#L307](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L307) [#L435](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L450) [#L490](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L490) [#L491](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L491) [#L519](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L519) [#L520](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L520) [#L547](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L547) [#L579](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L579) [#L584](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L584) [#L634](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L634) [#L635](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L635) [#L644](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L644) [#L645](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L645) [#L646](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L646) [#L651](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L651) [#L652](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L652) [#L653](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L653) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

134:       require(success, "Call Failed");

155:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L134) [#L155](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L155) 

</details>

---

<a name="GAS-22"></a> 
### [GAS-22] Don't initialize variables with default value

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
[#L134](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L134) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L160) [#L264](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L264) 

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L164](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L164) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

77:     for (uint256 i = 0; i < length; ++i) {

113:     for (uint256 i = 0; i < length; ++i) {

129:     for (uint256 i = 0; i < length + 1; ++i) {

```
[#L77](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L77) [#L113](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L113) [#L129](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L129) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

130:     for (uint256 i = 0; i < exCallData.length; ++i) {

```
[#L130](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L130) 

</details>

---

<a name="GAS-23"></a> 
### [GAS-23] Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead
Using `int`s/`uint`s smaller than 32 bytes may cost more gas. This is because the EVM operates on 32 bytes at a time, so if an element is smaller than 32 bytes, the EVM must perform more operations to reduce the size of the element from 32 bytes to the desired size.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

209:   function decimals() public pure returns (uint8) {

```
[#L209](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L209) 

</details>

---

<a name="GAS-24"></a> 
### [GAS-24] Constructors can be marked as `payable` to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. A constructor can be safely marked as payable, because only the deployer would be able to pass funds, and the project itself would not pass any funds.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

105:   constructor() {

```
[#L105](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L105) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

51:   constructor(address _guardian) {

```
[#L51](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L51) 

</details>

---

<a name="GAS-25"></a> 
### [GAS-25] Functions guaranteed to revert when called by normal users can be marked `payable`
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
[#L210](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L210) [#L220](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L220) [#L286](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L286) [#L295](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L295) [#L304](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L304) [#L313](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L313) [#L322](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L322) 

```solidity
File: contracts/bridge/SourceBridge.sol

136:   function pause() external onlyOwner {

145:   function unpause() external onlyOwner {

```
[#L136](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L136) [#L145](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L145) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

241:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

248:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```
[#L241](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L241) [#L248](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L248) 

```solidity
File: contracts/usdy/rUSDY.sol

662:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

685:   function pause() external onlyRole(PAUSER_ROLE) {

689:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

```
[#L662](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L662) [#L685](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L685) [#L689](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L689) 

</details>

---

<a name="GAS-26"></a> 
### [GAS-26] `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too)
*Saves 5 gas per loop*

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

79:     bytes memory payload = abi.encode(VERSION, msg.sender, amount, nonce++);

```
[#L79](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L79) 

</details>

---

<a name="GAS-27"></a> 
### [GAS-27] Using `private` rather than `public` for constants, saves gas
If needed, the values can be read from the verified contract source code, or if there are multiple values there can be a single getter function that [returns a tuple](https://github.com/code-423n4/2022-08-frax/blob/90f55a9ce4e25bceed3a74290b854341d8de6afa/src/contracts/FraxlendPair.sol#L156-L178) of the values of all currently-public constants. Saves **3406-3606 gas** in deployment gas due to the compiler not having to create non-payable getter functions for deployment calldata, not having to store the bytes of the value outside of where it's used, and not adding another entry to the method ID table

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

48:   bytes32 public constant VERSION = "1.0";

```
[#L48](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L48) 

```solidity
File: contracts/bridge/SourceBridge.sol

27:   bytes32 public constant VERSION = "1.0";

```
[#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L27) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

23:   uint256 public constant DAY = 1 days;

27:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

28:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```
[#L23](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L23) [#L27](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L27) [#L28](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L28) 

```solidity
File: contracts/usdy/rUSDY.sol

91:   uint256 public constant BPS_DENOMINATOR = 10_000;

97:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

98:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

99:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

100:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

101:   bytes32 public constant LIST_CONFIGURER_ROLE =

```
[#L91](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L91) [#L97](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L97) [#L98](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L98) [#L99](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L99) [#L100](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L100) [#L101](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L101) 

```solidity
File: contracts/usdy/rUSDYFactory.sol

44:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

```
[#L44](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDYFactory.sol#L44) 

</details>

---

<a name="GAS-28"></a> 
### [GAS-28] Use `!= 0` instead of `> 0` for unsigned integer comparison
Using `== 0`, `!= 0` instead of `> 0`, `>= 1`, `< 1`, `<= 0` can save gas.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

159:     if (t.approvers.length > 0) {

```
[#L159](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L159) 

```solidity
File: contracts/usdy/rUSDY.sol

435:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

450:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

```
[#L435](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L435) [#L450](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L450) 

</details>

---

<a name="GAS-29"></a> 
### [GAS-29] Using assembly to check for zero can save gas
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

<details>
<summary>
There are <b>16</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

113:     emit MessageReceived(srcChain, srcSender, amt, nonce);

160:       for (uint256 i = 0; i < t.approvers.length; ++i) {

287:     _setMintLimit(mintLimit);

```
[#L113](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L113) [#L160](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L160) [#L287](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/DestinationBridge.sol#L287) 

```solidity
File: contracts/bridge/SourceBridge.sol

68:     if (bytes(destContract).length == 0) {

72:     if (msg.value == 0) {

```
[#L68](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L68) [#L72](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/bridge/SourceBridge.sol#L72) 

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

209:     // Case 3: The range being modified is between first and last range

246:    * @notice Function to unpause the oracle

408: 

```
[#L209](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L209) [#L246](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L246) [#L408](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/rwaOracles/RWADynamicOracle.sol#L408) 

```solidity
File: contracts/usdy/rUSDY.sol

511:    * - `_sender` must hold at least `_sharesAmount` shares.

512:    * - the contract must not be paused.

536:    * @dev This doesn't increase the token total supply.

540:    * - `_recipient` cannot be the zero address.

560:     // as the result. This is equivalent to performing a send from each other token holder's

601:     return totalShares;

659:    * @dev The new oracle must comply with the `IPricerReader` interface

667:    * @notice Admin burn function to burn rUSDY tokens from any account

```
[#L511](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L511) [#L512](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L512) [#L536](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L536) [#L540](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L540) [#L560](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L560) [#L601](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L601) [#L659](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L659) [#L667](https://github.com/code-423n4/2023-09-ondo/blob/47d34d6d4a5303af5f46e907ac2292e6a7745f6c/contracts/usdy/rUSDY.sol#L667) 

</details>

---

