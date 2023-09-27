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


Total <b>64</b> instances over <b>15</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Array is `push()`ed but not `pop()`ed | 5 |
| [L-2](#L-2) | Enum values should be used instead of constant array indexes | 2 |
| [L-3](#L-3) | External call recipient can consume all remaining gas | 2 |
| [L-4](#L-4) | Governance functions should be controlled by time locks | 29 |
| [L-5](#L-5) | Missing contract existence checks before low-level calls | 2 |
| [L-6](#L-6) | Missing zero address check in constructor | 4 |
| [L-7](#L-7) | External call recipient can consume all remaining gas | 1 |
| [L-8](#L-8) | Missing storage gap for upgradable contracts | 1 |
| [L-9](#L-9) | prevent re-setting a state variable with the same value | 4 |
| [L-10](#L-10) | Timestamp may be manipulation | 4 |
| [L-11](#L-11) | Unsafe solidity low-level call can cause gas grief attack | 2 |
| [L-12](#L-12) | Use Ownable2Step instead of Ownable | 2 |
| [L-13](#L-13) | Using zero as a parameter | 4 |
| [L-14](#L-14) | Missing zero address check in initializer | 1 |
| [L-15](#L-15) | Initializers could be front-run | 1 |

## Non Critical Issues


Total <b>351</b> instances over <b>38</b> issues:

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
| [NC-21](#NC-21) | Public variable declarations should have NatSpec descriptions | 19 |
| [NC-22](#NC-22) | NatSpec `@return` is missing | 15 |
| [NC-23](#NC-23) | State variables should include comments | 11 |
| [NC-24](#NC-24) | Contract declarations should have NatSpec `@title` annotations | 3 |
| [NC-25](#NC-25) | Unused named return | 3 |
| [NC-26](#NC-26) | Unused contract variables | 1 |
| [NC-27](#NC-27) | Consider using `delete` rather than assigning zero to clear values | 8 |
| [NC-28](#NC-28) | Expressions for constant values should use `immutable` rather than `constant` | 13 |
| [NC-29](#NC-29) | Use the latest solidity version for deployment | 6 |
| [NC-30](#NC-30) | Missing checks for `address(0)` when assigning values to address state variables | 1 |
| [NC-31](#NC-31) | Common functions should be refactored to a common base contract | 8 |
| [NC-32](#NC-32) | Names of `private`/`internal` functions should be prefixed with an underscore | 2 |
| [NC-33](#NC-33) | Names of `private`/`internal` state variables should be prefixed with an underscore | 5 |
| [NC-34](#NC-34) |  `require()` / `revert()` statements should have descriptive reason strings | 1 |
| [NC-35](#NC-35) | Return values of `approve()` not checked | 6 |
| [NC-36](#NC-36) | Variables should be named in mixedCase style | 19 |
| [NC-37](#NC-37) | Event is missing `indexed` fields | 13 |
| [NC-38](#NC-38) | Functions not used internally could be marked external | 14 |

## Gas Optimizations


Total <b>221</b> instances over <b>31</b> issues:

|ID|Issue|Instances|Gas|
|-|:-|:-:|:-:|
| [GAS-1](#GAS-1) | Consider activating via-ir for deploying | 1 | - |
| [GAS-2](#GAS-2) | Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables | 4 | 452 |
| [GAS-3](#GAS-3) | `internal` functions only called once can be inlined to save gas | 9 | 270 |
| [GAS-4](#GAS-4) | `keccak256()` hash of literals should only be computed once | 7 | 294 |
| [GAS-5](#GAS-5) | Multiple accesses of the same mapping/array key/index should be cached | 19 | 798 |
| [GAS-6](#GAS-6) | Newer versions of solidity are more gas efficient | 6 | - |
| [GAS-7](#GAS-7) | Operator `>=`/`<=` costs less gas than operator `>`/`<` | 18 | 54 |
| [GAS-8](#GAS-8) | Reduce gas usage by moving to Solidity 0.8.19 or later | 6 | 6000 |
| [GAS-9](#GAS-9) | Redundant state variable getters | 1 | - |
| [GAS-10](#GAS-10) | Remove or replace unused state variables | 1 | - |
| [GAS-11](#GAS-11) | `require()`/`revert()` strings longer than 32 bytes cost extra gas | 3 | 9 |
| [GAS-12](#GAS-12) | The result of a function call should be cached rather than re-calling the function | 13 | 1300 |
| [GAS-13](#GAS-13) | Unused named return variables without optimizer waste gas | 3 | 27 |
| [GAS-14](#GAS-14) | Use assembly to compute hashes to save gas | 10 | 800 |
| [GAS-15](#GAS-15) | Use assembly to emit events | 20 | 760 |
| [GAS-16](#GAS-16) | Using a double `if` statement instead of a logical AND (`&&`) | 2 | 60 |
| [GAS-17](#GAS-17) | Use a more recent version of solidity | 6 | - |
| [GAS-18](#GAS-18) | `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants) | 2 | - |
| [GAS-19](#GAS-19) | Using bools for storage incurs overhead | 2 | - |
| [GAS-20](#GAS-20) | Cache array length outside of loop | 5 | - |
| [GAS-21](#GAS-21) | State variables should be cached in stack variables rather than re-reading them from storage | 4 | 388 |
| [GAS-22](#GAS-22) | Use `calldata` instead of `memory` for function arguments that do not get mutated | 1 | - |
| [GAS-23](#GAS-23) | Use Custom Errors | 21 | 1050 |
| [GAS-24](#GAS-24) | Don't initialize variables with default value | 8 | - |
| [GAS-25](#GAS-25) | Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead | 1 | 55 |
| [GAS-26](#GAS-26) | Constructors can be marked as `payable` to save deployment gas | 2 | 42 |
| [GAS-27](#GAS-27) | Functions guaranteed to revert when called by normal users can be marked `payable` | 14 | 294 |
| [GAS-28](#GAS-28) | `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too) | 1 | 5 |
| [GAS-29](#GAS-29) | Using `private` rather than `public` for constants, saves gas | 12 | - |
| [GAS-30](#GAS-30) | Use `!= 0` instead of `> 0` for unsigned integer comparison | 3 | 12 |
| [GAS-31](#GAS-31) | Using assembly to check for zero can save gas | 16 | 96 |

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

```solidity
File: contracts/usdy/rUSDYFactory.sol

116:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```

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

309:     IRWALike(_token).transfer(owner(), balance);

```

```solidity
File: contracts/usdy/rUSDY.sol

422:     usdy.transferFrom(msg.sender, address(this), _USDYAmount);

439:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

665:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```

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

309:     IRWALike(_token).transfer(owner(), balance);

```

```solidity
File: contracts/usdy/rUSDY.sol

422:     usdy.transferFrom(msg.sender, address(this), _USDYAmount);

439:     usdy.transfer(msg.sender, usdyAmount / BPS_DENOMINATOR);

665:     usdy.transfer(msg.sender, sharesAmount / BPS_DENOMINATOR);

```

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

15:   Ownable,

195:   function addApprover(address approver) external onlyOwner {

205:   function removeApprover(address approver) external onlyOwner {

222:   ) external onlyOwner {

244:   ) external onlyOwner {

271:   function setMintLimit(uint256 mintLimit) external onlyOwner {

280:   function setMintLimitDuration(uint256 mintDuration) external onlyOwner {

289:   function pause() external onlyOwner {

298:   function unpause() external onlyOwner {

307:   function rescueTokens(address _token) external onlyOwner {

```

```solidity
File: contracts/bridge/SourceBridge.sol

11: contract SourceBridge is Ownable, Pausable, IMulticall {

124:   ) external onlyOwner {

136:   function pause() external onlyOwner {

145:   function unpause() external onlyOwner {

162:   ) external payable override onlyOwner returns (bytes[] memory results) {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

140:   ) external onlyRole(SETTER_ROLE) {

178:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/usdy/rUSDY.sol

647:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

660:   ) external onlyRole(BURNER_ROLE) {

670:   function pause() external onlyRole(PAUSER_ROLE) {

674:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

685:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

696:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

707:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

66:   ) external onlyGuardian returns (address, address, address) {

113:   ) external payable override onlyGuardian returns (bytes[] memory results) {

```

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

151:     t.approvers.push(msg.sender);

251:         chainToThresholds[srcChain].push(

258:         chainToThresholds[srcChain].push(

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

31:     ranges.push(Range(firstRangeStart, firstRangeEnd, dailyIR, trueStart));

147:     ranges.push(

```

</details>

---

<a name="L-2"></a> 
### [L-2] Enum values should be used instead of constant array indexes
Create a commented enum value to use instead of constant array indexes, this makes the code far easier to understand.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

330:           ALLOWLIST.getValidTermIndexes()[0],

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

102:     if (startTime == ranges[0].start) {

```

</details>

---

<a name="L-3"></a> 
### [L-3] External call recipient can consume all remaining gas
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

165:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

116:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```

</details>

---

<a name="L-4"></a> 
### [L-4] Governance functions should be controlled by time locks
Governance functions (such as upgrading contracts, setting critical parameters) should be controlled using time locks to introduce a delay between a proposal and its execution. This gives users time to exit before a potentially dangerous or malicious operation is applied.

<details>
<summary>
There are <b>29</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

15:   Ownable,

195:   function addApprover(address approver) external onlyOwner {

205:   function removeApprover(address approver) external onlyOwner {

222:   ) external onlyOwner {

244:   ) external onlyOwner {

271:   function setMintLimit(uint256 mintLimit) external onlyOwner {

280:   function setMintLimitDuration(uint256 mintDuration) external onlyOwner {

289:   function pause() external onlyOwner {

298:   function unpause() external onlyOwner {

307:   function rescueTokens(address _token) external onlyOwner {

```

```solidity
File: contracts/bridge/SourceBridge.sol

11: contract SourceBridge is Ownable, Pausable, IMulticall {

124:   ) external onlyOwner {

136:   function pause() external onlyOwner {

145:   function unpause() external onlyOwner {

162:   ) external payable override onlyOwner returns (bytes[] memory results) {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

140:   ) external onlyRole(SETTER_ROLE) {

178:   ) external onlyRole(DEFAULT_ADMIN_ROLE) {

227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/usdy/rUSDY.sol

647:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

660:   ) external onlyRole(BURNER_ROLE) {

670:   function pause() external onlyRole(PAUSER_ROLE) {

674:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

685:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

696:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

707:   ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

66:   ) external onlyGuardian returns (address, address, address) {

113:   ) external payable override onlyGuardian returns (bytes[] memory results) {

```

</details>

---

<a name="L-5"></a> 
### [L-5] Missing contract existence checks before low-level calls
Low-level calls return success if there is no code present at the specified address. In addition to the zero-address checks, add a check to verify that `<address>.code.length > 0`

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

165:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

116:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```

</details>

---

<a name="L-6"></a> 
### [L-6] Missing zero address check in constructor
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
40:   constructor(
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

```

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

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing zero check for `_guardian`
36:   constructor(address _guardian) {

```

</details>

---

<a name="L-7"></a> 
### [L-7] External call recipient can consume all remaining gas
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

37:     guardian = _guardian;

```

</details>

---

<a name="L-8"></a> 
### [L-8] Missing storage gap for upgradable contracts
Each upgradable contract should include a state variable (usually named `__gap`) to provide reserved space in storage. This allows the team to freely add new state variables in the future upgrades without compromising the storage compatibility with existing deployments.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

42: contract rUSDY is
      Initializable,
      ContextUpgradeable,

```

</details>

---

<a name="L-9"></a> 
### [L-9] prevent re-setting a state variable with the same value
Not only is wasteful in terms of gas, but this is especially problematic when an event is emitted and the old and new values set are the same, as listeners might not expect this kind of scenario.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

124:     usdy = IUSDY(_usdy);

125:     oracle = IRWADynamicOracle(_oracle);

648:     oracle = IRWADynamicOracle(_oracle);

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

37:     guardian = _guardian;

```

</details>

---

<a name="L-10"></a> 
### [L-10] Timestamp may be manipulation
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

</details>

---

<a name="L-11"></a> 
### [L-11] Unsafe solidity low-level call can cause gas grief attack
Using the low-level calls of a solidity address can leave the contract open to gas grief attacks. These attacks occur when the called contract returns a large amount of data. So when calling an external contract, it is necessary to check the length of the return data before reading/copying it (using `returndatasize()`).

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

165:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

116:       (bool success, bytes memory ret) = address(exCallData[i].target).call{

```

</details>

---

<a name="L-12"></a> 
### [L-12] Use Ownable2Step instead of Ownable
`Ownable2Step` and `Ownable2StepUpgradeable` prevent the contract ownership from mistakenly being transferred to an address that cannot handle it (e.g. due to a typo in the address), by requiring that the recipient of the owner permissions actively accept via a contract call of its own.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

12: contract DestinationBridge is
      AxelarExecutable,
      MintTimeBasedRateLimiter,
      Ownable,

```

```solidity
File: contracts/bridge/SourceBridge.sol

11: contract SourceBridge is Ownable, Pausable, IMulticall {

```

</details>

---

<a name="L-13"></a> 
### [L-13] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

423:     emit Transfer(address(0), msg.sender, getRUSDYByShares(_USDYAmount));

424:     emit TransferShares(address(0), msg.sender, _USDYAmount);

534:     _beforeTokenTransfer(address(0), _recipient, _sharesAmount);

566:     _beforeTokenTransfer(_account, address(0), _sharesAmount);

```

</details>

---

<a name="L-14"></a> 
### [L-14] Missing zero address check in initializer

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
94:   function initialize(
        address blocklist,
        address allowlist,
        address sanctionsList,
        address _usdy,
        address guardian,
        address _oracle
      ) public virtual initializer {

```

</details>

---

<a name="L-15"></a> 
### [L-15] Initializers could be front-run
Initializers could be front-run, allowing an attacker to either set their own values, take ownership of the contract, and in the best case forcing a re-deployment

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

94:   function initialize(

```

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

85:     assert(rUSDYProxyAdmin.owner() == guardian);

```

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

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

4: interface IRWADynamicOracle {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```

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

129:     if (txnToThresholdSet[txnHash].numberOfApprovalsNeeded == 0) {

250:       if (i == 0) {

```

```solidity
File: contracts/bridge/SourceBridge.sol

68:     if (bytes(destContract).length == 0) {

72:     if (msg.value == 0) {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

184:     if (indexToModify == 0) {

204:     if (indexToModify == 0) {

270:     if (remainder >= 0.5e10) {

391:     require(y == 0 || (z = x * y) / y == x);

```

```solidity
File: contracts/usdy/rUSDY.sol

475:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

476:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

504:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

505:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

532:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

564:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

627:     if (from != address(0)) {

634:     if (to != address(0)) {

```

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

98:     emit MessageReceived(srcChain, srcSender, amt, nonce);

197:     emit ApproverAdded(approver);

207:     emit ApproverRemoved(approver);

224:     emit ChainIdSupported(srcChain, srcContractAddress);

263:     emit ThresholdSet(srcChain, amounts, numOfApprovers);

336:       emit BridgeCompleted(txn.sender, txn.amount);

```

```solidity
File: contracts/bridge/SourceBridge.sol

128:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```

```solidity
File: contracts/usdy/rUSDY.sol

406:     emit TransferShares(msg.sender, _recipient, _sharesAmount);

408:     emit Transfer(msg.sender, _recipient, tokensAmount);

423:     emit Transfer(address(0), msg.sender, getRUSDYByShares(_USDYAmount));

424:     emit TransferShares(address(0), msg.sender, _USDYAmount);

440:     emit TokensBurnt(msg.sender, _rUSDYAmount);

455:     emit Transfer(_sender, _recipient, _amount);

456:     emit TransferShares(_sender, _recipient, _sharesToTransfer);

479:     emit Approval(_owner, _spender, _amount);

667:     emit TokensBurnt(_account, _amount);

```

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

424:   error NotApprover();

425:   error NoThresholdMatch();

426:   error ThresholdsNotInAscendingOrder();

428:   error ChainNotSupported();

429:   error SourceNotSupported();

430:   error NonceSpent();

431:   error AlreadyApproved();

432:   error InvalidVersion();

433:   error ArrayLengthMismatch();

```

```solidity
File: contracts/bridge/SourceBridge.sol

189:   error DestinationNotSupported();

190:   error GasFeeTooLow();

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

320:   error InvalidPrice();

321:   error InvalidRange();

322:   error PriceNotSet();

```

```solidity
File: contracts/usdy/rUSDY.sol

79:   error UnwrapTooSmall();

```

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

```solidity
File: contracts/usdy/rUSDY.sol

292:     require(currentAllowance >= _amount, "TRANSFER_AMOUNT_EXCEEDS_ALLOWANCE");

420:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

435:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

475:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

476:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

504:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

505:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

532:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

564:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

569:     require(_sharesAmount <= accountShares, "BURN_AMOUNT_EXCEEDS_BALANCE");

619:       require(!_isBlocked(msg.sender), "rUSDY: 'sender' address blocked");

620:       require(!_isSanctioned(msg.sender), "rUSDY: 'sender' address sanctioned");

629:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");

630:       require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

631:       require(_isAllowed(from), "rUSDY: 'from' address not on allowlist");

636:       require(!_isBlocked(to), "rUSDY: 'to' address blocked");

637:       require(!_isSanctioned(to), "rUSDY: 'to' address sanctioned");

638:       require(_isAllowed(to), "rUSDY: 'to' address not on allowlist");

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

119:       require(success, "Call Failed");

140:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```

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

164:     if (t.numberOfApprovalsNeeded <= t.approvers.length) {
           return true;
         } else {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

66:         if (range.end <= block.timestamp) {
              return derivePrice(range, range.end - 1);
            } else {

118:         if (range.end <= blockTimeStamp) {
               return derivePrice(range, range.end - 1);
             } else {

```

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

98:     emit MessageReceived(srcChain, srcSender, amt, nonce);

197:     emit ApproverAdded(approver);

207:     emit ApproverRemoved(approver);

224:     emit ChainIdSupported(srcChain, srcContractAddress);

263:     emit ThresholdSet(srcChain, amounts, numOfApprovers);

```

```solidity
File: contracts/bridge/SourceBridge.sol

128:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

150:     emit RangeSet(

215:     emit RangeOverriden(

```

```solidity
File: contracts/usdy/rUSDY.sol

455:     emit Transfer(_sender, _recipient, _amount);

456:     emit TransferShares(_sender, _recipient, _sharesToTransfer);

479:     emit Approval(_owner, _spender, _amount);

579:     emit SharesBurnt(

667:     emit TokensBurnt(_account, _amount);

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

86:     emit rUSDYDeployed(

```

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

3: import "contracts/interfaces/IAxelarGateway.sol";

4: import "contracts/interfaces/IAxelarGasService.sol";

5: import "contracts/external/axelar/AxelarExecutable.sol";

6: import "contracts/interfaces/IRWALike.sol";

7: import "contracts/interfaces/IAllowlist.sol";

8: import "contracts/external/openzeppelin/contracts/access/Ownable.sol";

9: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

10: import "contracts/bridge/MintRateLimiter.sol";

```

```solidity
File: contracts/bridge/SourceBridge.sol

3: import "contracts/interfaces/IAxelarGateway.sol";

4: import "contracts/interfaces/IAxelarGasService.sol";

5: import "contracts/interfaces/IMulticall.sol";

6: import "contracts/interfaces/IRWALike.sol";

8: import "contracts/external/openzeppelin/contracts/access/Ownable.sol";

9: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

4: import "contracts/rwaOracles/IRWAOracle.sol";

5: import "contracts/external/openzeppelin/contracts/access/AccessControlEnumerable.sol";

6: import "contracts/external/openzeppelin/contracts/security/Pausable.sol";

```

```solidity
File: contracts/usdy/rUSDY.sol

3: import "contracts/external/openzeppelin/contracts-upgradeable/token/ERC20/IERC20Upgradeable.sol";

4: import "contracts/external/openzeppelin/contracts-upgradeable/token/ERC20/IERC20MetadataUpgradeable.sol";

5: import "contracts/external/openzeppelin/contracts-upgradeable/proxy/Initializable.sol";

6: import "contracts/external/openzeppelin/contracts-upgradeable/utils/ContextUpgradeable.sol";

7: import "contracts/external/openzeppelin/contracts-upgradeable/security/PausableUpgradeable.sol";

8: import "contracts/external/openzeppelin/contracts-upgradeable/access/AccessControlEnumerableUpgradeable.sol";

9: import "contracts/usdy/blocklist/BlocklistClientUpgradeable.sol";

10: import "contracts/usdy/allowlist/AllowlistClientUpgradeable.sol";

11: import "contracts/sanctions/SanctionsListClientUpgradeable.sol";

12: import "contracts/interfaces/IUSDY.sol";

13: import "contracts/rwaOracles/IRWADynamicOracle.sol";

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

4: import "contracts/external/openzeppelin/contracts/proxy/ProxyAdmin.sol";

5: import "contracts/Proxy.sol";

6: import "contracts/usdy/rUSDY.sol";

7: import "contracts/interfaces/IMulticall.sol";

```

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
40:   constructor(
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
195:   function addApprover(address approver) external onlyOwner {

/// Missing zero check for `approver`
205:   function removeApprover(address approver) external onlyOwner {

/// Missing zero check for `_token`
307:   function rescueTokens(address _token) external onlyOwner {

```

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

```solidity
File: contracts/usdy/rUSDY.sol

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `_usdy`
/// Missing zero check for `guardian`
/// Missing zero check for `_oracle`
94:   function initialize(
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
105:   function __rUSDY_init(
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
119:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing zero check for `_account`
211:   function balanceOf(address _account) public view returns (uint256) {

/// Missing zero check for `_recipient`
230:   function transfer(address _recipient, uint256 _amount) public returns (bool) {

/// Missing zero check for `_spender`
261:   function approve(address _spender, uint256 _amount) public returns (bool) {

/// Missing zero check for `_account`
366:   function sharesOf(address _account) public view returns (uint256) {

/// Missing zero check for `_sender`
/// Missing zero check for `_recipient`
448:   function _transfer(
         address _sender,
         address _recipient,
         uint256 _amount
       ) internal {

/// Missing zero check for `_account`
485:   function _sharesOf(address _account) internal view returns (uint256) {

/// Missing zero check for `_oracle`
647:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

/// Missing zero check for `_account`
657:   function burn(
         address _account,
         uint256 _amount
       ) external onlyRole(BURNER_ROLE) {

/// Missing zero check for `blocklist`
683:   function setBlocklist(
         address blocklist
       ) external override onlyRole(LIST_CONFIGURER_ROLE) {

/// Missing zero check for `allowlist`
694:   function setAllowlist(
         address allowlist
       ) external override onlyRole(LIST_CONFIGURER_ROLE) {

/// Missing zero check for `sanctionsList`
705:   function setSanctionsList(
         address sanctionsList
       ) external override onlyRole(LIST_CONFIGURER_ROLE) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing zero check for `_guardian`
36:   constructor(address _guardian) {

/// Missing zero check for `blocklist`
/// Missing zero check for `allowlist`
/// Missing zero check for `sanctionsList`
/// Missing zero check for `usdy`
/// Missing zero check for `oracle`
60:   function deployrUSDY(
        address blocklist,
        address allowlist,
        address sanctionsList,
        address usdy,
        address oracle
      ) external onlyGuardian returns (address, address, address) {

```

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

619:       require(!_isBlocked(msg.sender), "rUSDY: 'sender' address blocked");

620:       require(!_isSanctioned(msg.sender), "rUSDY: 'sender' address sanctioned");

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

140:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```

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

28:   mapping(address => bool) public approvers;

29:   mapping(string => bytes32) public chainToApprovedSender;

30:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

36:   mapping(bytes32 => TxnThreshold) public txnToThresholdSet;

37:   mapping(string => Threshold[]) public chainToThresholds;

38:   mapping(bytes32 => Transaction) public txnHashToTransaction;

```

```solidity
File: contracts/bridge/SourceBridge.sol

15:   mapping(string => string) public destChainToContractAddr;

```

```solidity
File: contracts/usdy/rUSDY.sol

61:   mapping(address => uint256) private shares;

64:   mapping(address => mapping(address => uint256)) private allowances;

```

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

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

4: interface IRWADynamicOracle {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```

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

40:   constructor(
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

```solidity
File: contracts/usdy/rUSDY.sol

94:   function initialize(
        address blocklist,
        address allowlist,
        address sanctionsList,
        address _usdy,
        address guardian,
        address _oracle
      ) public virtual initializer {

105:   function __rUSDY_init(
         address blocklist,
         address allowlist,
         address sanctionsList,
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

119:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

670:   function pause() external onlyRole(PAUSER_ROLE) {

674:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

36:   constructor(address _guardian) {

```

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

139:   modifier onlyGuardian() {

```

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
40:   constructor(
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

```solidity
File: contracts/usdy/rUSDY.sol

/// Missing @param for blocklist
/// Missing @param for allowlist
/// Missing @param for sanctionsList
/// Missing @param for _usdy
/// Missing @param for guardian
/// Missing @param for _oracle
94:   function initialize(
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
105:   function __rUSDY_init(
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
119:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// Missing @param for _account
211:   function balanceOf(address _account) public view returns (uint256) {

/// Missing @param for _recipient
/// Missing @param for _amount
230:   function transfer(address _recipient, uint256 _amount) public returns (bool) {

/// Missing @param for _owner
/// Missing @param for _spender
241:   function allowance(
         address _owner,
         address _spender
       ) public view returns (uint256) {

/// Missing @param for _spender
/// Missing @param for _amount
261:   function approve(address _spender, uint256 _amount) public returns (bool) {

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _amount
286:   function transferFrom(
         address _sender,
         address _recipient,
         uint256 _amount
       ) public returns (bool) {

/// Missing @param for _spender
/// Missing @param for _addedValue
312:   function increaseAllowance(
         address _spender,
         uint256 _addedValue
       ) public returns (bool) {

/// Missing @param for _spender
/// Missing @param for _subtractedValue
338:   function decreaseAllowance(
         address _spender,
         uint256 _subtractedValue
       ) public returns (bool) {

/// Missing @param for _account
366:   function sharesOf(address _account) public view returns (uint256) {

/// Missing @param for _rUSDYAmount
373:   function getSharesByRUSDY(
         uint256 _rUSDYAmount
       ) public view returns (uint256) {

/// Missing @param for _shares
382:   function getRUSDYByShares(uint256 _shares) public view returns (uint256) {

/// Missing @param for _recipient
/// Missing @param for _sharesAmount
401:   function transferShares(
         address _recipient,
         uint256 _sharesAmount
       ) public returns (uint256) {

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _amount
448:   function _transfer(
         address _sender,
         address _recipient,
         uint256 _amount
       ) internal {

/// Missing @param for _owner
/// Missing @param for _spender
/// Missing @param for _amount
470:   function _approve(
         address _owner,
         address _spender,
         uint256 _amount
       ) internal whenNotPaused {

/// Missing @param for _account
485:   function _sharesOf(address _account) internal view returns (uint256) {

/// Missing @param for _sender
/// Missing @param for _recipient
/// Missing @param for _sharesAmount
499:   function _transferShares(
         address _sender,
         address _recipient,
         uint256 _sharesAmount
       ) internal whenNotPaused {

/// Missing @param for _recipient
/// Missing @param for _sharesAmount
528:   function _mintShares(
         address _recipient,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

/// Missing @param for _account
/// Missing @param for _sharesAmount
560:   function _burnShares(
         address _account,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

/// Missing @param for from
/// Missing @param for to
611:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Missing @param for _guardian
36:   constructor(address _guardian) {

/// Missing @param for oracle
60:   function deployrUSDY(
        address blocklist,
        address allowlist,
        address sanctionsList,
        address usdy,
        address oracle
      ) external onlyGuardian returns (address, address, address) {

```

</details>

---

<a name="NC-21"></a> 
### [NC-21] Public variable declarations should have NatSpec descriptions

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

29:   mapping(string => bytes32) public chainToApprovedSender;

30:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

37:   mapping(string => Threshold[]) public chainToThresholds;

38:   mapping(bytes32 => Transaction) public txnHashToTransaction;

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

11:   Range[] public ranges;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```

```solidity
File: contracts/usdy/rUSDY.sol

70:   IRWADynamicOracle public oracle;

73:   IUSDY public usdy;

76:   uint256 public constant BPS_DENOMINATOR = 10_000;

83:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

84:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

85:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

86:   bytes32 public constant LIST_CONFIGURER_ROLE =

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

29:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

32:   rUSDY public rUSDYImplementation;

33:   ProxyAdmin public rUSDYProxyAdmin;

34:   TokenProxy public rUSDYProxy;

```

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

162:   function _checkThresholdMet(bytes32 txnHash) internal view returns (bool) {

346:   function getNumApproved(bytes32 txnHash) external view returns (uint256) {

```

```solidity
File: contracts/bridge/SourceBridge.sol

160:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyOwner returns (bytes[] memory results) {

```

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

6:   function getPrice() external view returns (uint256);

```

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

```solidity
File: contracts/usdy/rUSDY.sol

312:   function increaseAllowance(
         address _spender,
         uint256 _addedValue
       ) public returns (bool) {

338:   function decreaseAllowance(
         address _spender,
         uint256 _subtractedValue
       ) public returns (bool) {

528:   function _mintShares(
         address _recipient,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

560:   function _burnShares(
         address _account,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

111:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyGuardian returns (bytes[] memory results) {

```

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

29:   mapping(string => bytes32) public chainToApprovedSender;

30:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

37:   mapping(string => Threshold[]) public chainToThresholds;

38:   mapping(bytes32 => Transaction) public txnHashToTransaction;

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```

```solidity
File: contracts/usdy/rUSDY.sol

83:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

84:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

85:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

86:   bytes32 public constant LIST_CONFIGURER_ROLE =

```

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

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

4: interface IRWADynamicOracle {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

8: contract RWADynamicOracle is IRWAOracle, AccessControlEnumerable, Pausable {

```

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

</details>

---

<a name="NC-26"></a> 
### [NC-26] Unused contract variables
The following state variables are defined but not used. It is recommended to check the code for logical omissions that cause them not to be used. If it's determined that they are not needed anywhere, it's best to remove them from the codebase to improve code clarity and minimize confusion.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

```

</details>

---

<a name="NC-27"></a> 
### [NC-27] Consider using `delete` rather than assigning zero to clear values
The `delete` keyword more closely matches the semantics of what is being done, and draws more attention to the changing of state, which may lead to a more thorough audit of its associated logic.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

119:     for (uint256 i = 0; i < thresholds.length; ++i) {

145:       for (uint256 i = 0; i < t.approvers.length; ++i) {

249:     for (uint256 i = 0; i < amounts.length; ++i) {

```

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

63:     for (uint256 i = 0; i < length; ++i) {

99:     for (uint256 i = 0; i < length; ++i) {

115:     for (uint256 i = 0; i < length + 1; ++i) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

115:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

</details>

---

<a name="NC-28"></a> 
### [NC-28] Expressions for constant values should use `immutable` rather than `constant`
While it doesn't save any gas because the compiler knows that developers often make this mistake, it's still best to use the right tool for the task at hand. There is a difference between `constant` variables and `immutable` variables, and they should each be used in their appropriate contexts. `constants` should be used for literal values written into the code, and `immutable` variables should be used for expressions, or values calculated in, or passed into the constructor.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

33:   bytes32 public constant VERSION = "1.0";

```

```solidity
File: contracts/bridge/SourceBridge.sol

27:   bytes32 public constant VERSION = "1.0";

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

329:   uint256 private constant ONE = 10 ** 27;

```

```solidity
File: contracts/usdy/rUSDY.sol

76:   uint256 public constant BPS_DENOMINATOR = 10_000;

82:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

83:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

84:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

85:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

86:   bytes32 public constant LIST_CONFIGURER_ROLE =

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

29:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

```

</details>

---

<a name="NC-29"></a> 
### [NC-29] Use the latest solidity version for deployment
Upgrading to a newer Solidity release can optimize gas usage, take advantage of new features and improve overall contract efficiency. Where possible, based on compatibility requirements, it is recommended to use newer/latest solidity version to take advantage of the latest optimizations and features.

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDY.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

1: pragma solidity 0.8.16;

```

</details>

---

<a name="NC-30"></a> 
### [NC-30] Missing checks for `address(0)` when assigning values to address state variables

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDYFactory.sol

37:     guardian = _guardian;

```

</details>

---

<a name="NC-31"></a> 
### [NC-31] Common functions should be refactored to a common base contract
The functions below have the same implementation as is seen in other files. The functions should be refactored into functions of a common base contract.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// Seen in contracts/bridge/SourceBridge.sol
289:   function pause() external onlyOwner {

/// Seen in contracts/bridge/SourceBridge.sol
298:   function unpause() external onlyOwner {

```

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

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

/// Seen in contracts/bridge/SourceBridge.sol
227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

/// Seen in contracts/bridge/SourceBridge.sol
234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

/// Seen in contracts/bridge/SourceBridge.sol
111:   function multiexcall(
         ExCallData[] calldata exCallData
       ) external payable override onlyGuardian returns (bytes[] memory results) {

```

</details>

---

<a name="NC-32"></a> 
### [NC-32] Names of `private`/`internal` functions should be prefixed with an underscore
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

</details>

---

<a name="NC-33"></a> 
### [NC-33] Names of `private`/`internal` state variables should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

329:   uint256 private constant ONE = 10 ** 27;

```

```solidity
File: contracts/usdy/rUSDY.sol

61:   mapping(address => uint256) private shares;

64:   mapping(address => mapping(address => uint256)) private allowances;

67:   uint256 private totalShares;

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

31:   address internal immutable guardian;

```

</details>

---

<a name="NC-34"></a> 
### [NC-34]  `require()` / `revert()` statements should have descriptive reason strings

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

391:     require(y == 0 || (z = x * y) / y == x);

```

</details>

---

<a name="NC-35"></a> 
### [NC-35] Return values of `approve()` not checked
Not all IERC20 implementations `revert()` when there's a failure in `approve()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually approving anything

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

96:     _approve(txnHash);

186:     _approve(txnHash);

```

```solidity
File: contracts/usdy/rUSDY.sol

262:     _approve(msg.sender, _spender, _amount);

295:     _approve(_sender, msg.sender, currentAllowance - _amount);

316:     _approve(

347:     _approve(msg.sender, _spender, currentAllowance - _subtractedValue);

```

</details>

---

<a name="NC-36"></a> 
### [NC-36] Variables should be named in mixedCase style
As the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html#naming-styles) suggests: arguments, local variables and mutable state variables should be named in mixedCase style.

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

19:   IRWALike public immutable TOKEN;

22:   IAxelarGateway public immutable AXELAR_GATEWAY;

25:   IAllowlist public immutable ALLOWLIST;

33:   bytes32 public constant VERSION = "1.0";

```

```solidity
File: contracts/bridge/SourceBridge.sol

18:   IRWALike public immutable TOKEN;

21:   IAxelarGateway public immutable AXELAR_GATEWAY;

24:   IAxelarGasService public immutable GAS_RECEIVER;

27:   bytes32 public constant VERSION = "1.0";

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

30:     uint256 trueStart = (startPrice * ONE) / dailyIR;

```

```solidity
File: contracts/usdy/rUSDY.sol

76:   uint256 public constant BPS_DENOMINATOR = 10_000;

82:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

83:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

84:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

85:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

86:   bytes32 public constant LIST_CONFIGURER_ROLE =

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

22:  *         i) Grant the `DEFAULT_ADMIN_ROLE` & PAUSER_ROLE to the `guardian` address

```

</details>

---

<a name="NC-37"></a> 
### [NC-37] Event is missing `indexed` fields
Index event fields make the field more quickly accessible to off-chain tools that parse events. However, note that each index field costs extra gas during emission, so it's not necessarily best to index the maximum allowed per event (three fields). Each event should use three indexed fields if there are three or more fields, and gas usage is not particularly of concern for the events in question. If there are fewer than three fields, all of the fields should be indexed.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

374:   event ApproverRemoved(address approver);

381:   event ApproverAdded(address approver);

390:   event ChainIdSupported(string srcChain, string approvedSource);

399:   event ThresholdSet(string chain, uint256[] amounts, uint256[] numOfApprovers);

407:   event BridgeCompleted(address user, uint256 amount);

417:   event MessageReceived(

```

```solidity
File: contracts/bridge/SourceBridge.sol

183:   event DestinationChainContractAddressSet(

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

295:   event RangeSet(

312:   event RangeOverriden(

```

```solidity
File: contracts/usdy/rUSDY.sol

139:   event TransferShares(

157:   event SharesBurnt(

174:   event TokensBurnt(address indexed account, uint256 tokensBurnt);

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

131:   event rUSDYDeployed(

```

</details>

---

<a name="NC-38"></a> 
### [NC-38] Functions not used internally could be marked external

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

179:   function name() public pure returns (string memory) {

187:   function symbol() public pure returns (string memory) {

194:   function decimals() public pure returns (uint8) {

201:   function totalSupply() public view returns (uint256) {

211:   function balanceOf(address _account) public view returns (uint256) {

230:   function transfer(address _recipient, uint256 _amount) public returns (bool) {

241:   function allowance(

261:   function approve(address _spender, uint256 _amount) public returns (bool) {

286:   function transferFrom(

312:   function increaseAllowance(

338:   function decreaseAllowance(

357:   function getTotalShares() public view returns (uint256) {

366:   function sharesOf(address _account) public view returns (uint256) {

401:   function transferShares(

```

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

271:       value += 1e10;

273:     value -= remainder;

```

```solidity
File: contracts/usdy/rUSDY.sol

536:     totalShares += _sharesAmount;

573:     totalShares -= _sharesAmount;

```

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
113:   function _attachThreshold(

/// `_checkThresholdMet` is used only once
162:   function _checkThresholdMet(bytes32 txnHash) internal view returns (bool) {

```

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

```solidity
File: contracts/usdy/rUSDY.sol

/// `__rUSDY_init` is used only once
105:   function __rUSDY_init(

/// `__rUSDY_init_unchained` is used only once
119:   function __rUSDY_init_unchained(

/// `_mintShares` is used only once
528:   function _mintShares(

```

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

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```

```solidity
File: contracts/usdy/rUSDY.sol

82:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

83:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

84:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

85:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

87:     keccak256("LIST_CONFIGURER_ROLE");

```

</details>

---

<a name="GAS-5"></a> 
### [GAS-5] Multiple accesses of the same mapping/array key/index should be cached
The instances below point to the second+ access of a value inside a mapping/array, within a function. Caching a mapping's value in a local `storage` or `calldata` variable when the value is accessed [multiple times](https://gist.github.com/IllIllI000/ec23a57daa30a8f8ca8b9681c8ccefb0), saves ~42 gas per access due to not having to recalculate the key's keccak256 hash (Gkeccak256 - 30 gas) and that calculation's associated stack operations. Caching an array's struct avoids recalculating the array offsets into memory/calldata

<details>
<summary>
There are <b>19</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `chainToApprovedSender[srcChain]` is also accessed on line 81
84:     if (chainToApprovedSender[srcChain] != keccak256(abi.encode(srcAddr))) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 81
84:     if (chainToApprovedSender[srcChain] != keccak256(abi.encode(srcAddr))) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 81
87:     if (isSpentNonce[chainToApprovedSender[srcChain]][nonce]) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 81
87:     if (isSpentNonce[chainToApprovedSender[srcChain]][nonce]) {

/// `chainToApprovedSender[srcChain]` is also accessed on line 81
91:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `isSpentNonce[chainToApprovedSender[srcChain]` is also accessed on line 87
91:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `chainToApprovedSender[srcChain]` is also accessed on line 81
91:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `isSpentNonce[chainToApprovedSender[srcChain]` is also accessed on line 87
91:     isSpentNonce[chainToApprovedSender[srcChain]][nonce] = true;

/// `txnToThresholdSet[txnHash]` is also accessed on line 122
129:     if (txnToThresholdSet[txnHash].numberOfApprovalsNeeded == 0) {

/// `chainToThresholds[srcChain]` is also accessed on line 248
251:         chainToThresholds[srcChain].push(

/// `chainToThresholds[srcChain]` is also accessed on line 248
255:         if (chainToThresholds[srcChain][i - 1].amount > amounts[i]) {

/// `chainToThresholds[srcChain]` is also accessed on line 248
258:         chainToThresholds[srcChain].push(

/// `txnHashToTransaction[txnHash]` is also accessed on line 324
335:       delete txnHashToTransaction[txnHash];

```

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

```solidity
File: contracts/usdy/rUSDY.sol

/// `shares[_sender]` is also accessed on line 509
515:     shares[_sender] = currentSenderShares - _sharesAmount;

/// `shares[_account]` is also accessed on line 568
575:     shares[_account] = accountShares - _sharesAmount;

```

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

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDY.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

1: pragma solidity 0.8.16;

```

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

119:     for (uint256 i = 0; i < thresholds.length; ++i) {

144:     if (t.approvers.length > 0) {

145:       for (uint256 i = 0; i < t.approvers.length; ++i) {

249:     for (uint256 i = 0; i < amounts.length; ++i) {

255:         if (chainToThresholds[srcChain][i - 1].amount > amounts[i]) {

```

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

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

```solidity
File: contracts/usdy/rUSDY.sol

420:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

435:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

437:     if (usdyAmount < BPS_DENOMINATOR) revert UnwrapTooSmall();

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

115:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

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

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDY.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

1: pragma solidity 0.8.16;

```

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

357:   function getTotalShares() public view returns (uint256) {
         return totalShares;

```

</details>

---

<a name="GAS-10"></a> 
### [GAS-10] Remove or replace unused state variables
Saves a storage slot. If the variable is assigned a non-zero value, saves Gsset (20000 gas). If it's assigned a zero value, saves Gsreset (2900 gas). If the variable remains unassigned, there is no gas savings unless the variable is `public`, in which case the compiler-generated non-payable getter deployment cost is saved. If the state variable is overriding an interface's public function, mark the variable as `constant` or `immutable` so that it does not use a storage slot.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

```

</details>

---

<a name="GAS-11"></a> 
### [GAS-11] `require()`/`revert()` strings longer than 32 bytes cost extra gas
Each extra memory word of bytes past the original 32 [incurs an MSTORE](https://gist.github.com/hrkrshnn/ee8fabd532058307229d65dcd5836ddc#consider-having-short-revert-strings) which costs 3 gas

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

292:     require(currentAllowance >= _amount, "TRANSFER_AMOUNT_EXCEEDS_ALLOWANCE");

420:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

435:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

```

</details>

---

<a name="GAS-12"></a> 
### [GAS-12] The result of a function call should be cached rather than re-calling the function
The function calls in solidity are expensive. If the same result of the same function calls are to be used several times, the result should be cached to reduce the gas consumption of repeated calls.

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

/// `keccak256` is called 2 times
70:   function _execute(
        string calldata srcChain,
        string calldata srcAddr,
        bytes calldata payload
      ) internal override whenNotPaused {

/// `Threshold` is called 2 times
240:   function setThresholds(
         string calldata srcChain,
         uint256[] calldata amounts,
         uint256[] calldata numOfApprovers
       ) external onlyOwner {

/// `IRWALike` is called 2 times
307:   function rescueTokens(address _token) external onlyOwner {

```

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

```solidity
File: contracts/usdy/rUSDY.sol

/// `_grantRole` is called 6 times
119:   function __rUSDY_init_unchained(
         address _usdy,
         address guardian,
         address _oracle
       ) internal onlyInitializing {

/// `getRUSDYByShares` is called 2 times
560:   function _burnShares(
         address _account,
         uint256 _sharesAmount
       ) internal whenNotPaused returns (uint256) {

/// `_isBlocked` is called 3 times
611:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

/// `_isSanctioned` is called 3 times
611:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

/// `_isAllowed` is called 3 times
611:   function _beforeTokenTransfer(
         address from,
         address to,
         uint256
       ) internal view {

```

</details>

---

<a name="GAS-13"></a> 
### [GAS-13] Unused named return variables without optimizer waste gas
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

</details>

---

<a name="GAS-14"></a> 
### [GAS-14] Use assembly to compute hashes to save gas
If the arguments to the encode call can fit into the scratch space (two words or fewer), then it's more efficient to use assembly to generate the hash (80 gas):

`keccak256(abi.encodePacked(x, y)) -> assembly {mstore(0x00, a); mstore(0x20, b); let hash := keccak256(0x00, 0x40); }`

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

84:     if (chainToApprovedSender[srcChain] != keccak256(abi.encode(srcAddr))) {

93:     bytes32 txnHash = keccak256(payload);

223:     chainToApprovedSender[srcChain] = keccak256(abi.encode(srcContractAddress));

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```

```solidity
File: contracts/usdy/rUSDY.sol

82:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

83:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

84:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

85:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

87:     keccak256("LIST_CONFIGURER_ROLE");

```

</details>

---

<a name="GAS-15"></a> 
### [GAS-15] Use assembly to emit events
To efficiently emit events, it's possible to utilize assembly by making use of scratch space and the free memory pointer. This approach has the advantage of potentially avoiding the costs associated with memory expansion.

However, it's important to note that in order to safely optimize this process, it is preferable to cache and restore the free memory pointer.

A good example of such practice can be seen in [Solady's](https://github.com/Vectorized/solady/blob/main/src/tokens/ERC1155.sol#L167) codebase.

<details>
<summary>
There are <b>20</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

98:     emit MessageReceived(srcChain, srcSender, amt, nonce);

197:     emit ApproverAdded(approver);

207:     emit ApproverRemoved(approver);

224:     emit ChainIdSupported(srcChain, srcContractAddress);

263:     emit ThresholdSet(srcChain, amounts, numOfApprovers);

336:       emit BridgeCompleted(txn.sender, txn.amount);

```

```solidity
File: contracts/bridge/SourceBridge.sol

128:     emit DestinationChainContractAddressSet(destinationChain, contractAddress);

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

150:     emit RangeSet(

215:     emit RangeOverriden(

```

```solidity
File: contracts/usdy/rUSDY.sol

406:     emit TransferShares(msg.sender, _recipient, _sharesAmount);

408:     emit Transfer(msg.sender, _recipient, tokensAmount);

423:     emit Transfer(address(0), msg.sender, getRUSDYByShares(_USDYAmount));

424:     emit TransferShares(address(0), msg.sender, _USDYAmount);

440:     emit TokensBurnt(msg.sender, _rUSDYAmount);

455:     emit Transfer(_sender, _recipient, _amount);

456:     emit TransferShares(_sender, _recipient, _sharesToTransfer);

479:     emit Approval(_owner, _spender, _amount);

579:     emit SharesBurnt(

667:     emit TokensBurnt(_account, _amount);

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

86:     emit rUSDYDeployed(

```

</details>

---

<a name="GAS-16"></a> 
### [GAS-16] Using a double `if` statement instead of a logical AND (`&&`)
Using a double `if` statement instead of a logical AND (`&&`) can provide similar short-circuiting behavior whereas double if is slightly [more gas efficient](https://gist.github.com/DadeKuma/931ce6794a050201ec6544dbcc31316c).

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

187:       if (rangeLength > 1 && newEnd > ranges[indexToModify + 1].start)

```

```solidity
File: contracts/usdy/rUSDY.sol

618:     if (from != msg.sender && to != msg.sender) {

```

</details>

---

<a name="GAS-17"></a> 
### [GAS-17] Use a more recent version of solidity
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

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/bridge/SourceBridge.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/IRWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

2: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDY.sol

1: pragma solidity 0.8.16;

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

1: pragma solidity 0.8.16;

```

</details>

---

<a name="GAS-18"></a> 
### [GAS-18] `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants)
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

516:     shares[_recipient] = shares[_recipient] + _sharesAmount;

538:     shares[_recipient] = shares[_recipient] + _sharesAmount;

```

</details>

---

<a name="GAS-19"></a> 
### [GAS-19] Using bools for storage incurs overhead
Use uint256(1) and uint256(2) for true/false to avoid a Gwarmaccess (100 gas), and to avoid Gsset (20000 gas) when changing from ‘false’ to ‘true’, after having been ‘true’ in the past. See [source](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/58f635312aa21f947cae5f8578638a85aa2519f5/contracts/security/ReentrancyGuard.sol#L23-L27).

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

28:   mapping(address => bool) public approvers;

30:   mapping(bytes32 => mapping(uint256 => bool)) public isSpentNonce;

```

</details>

---

<a name="GAS-20"></a> 
### [GAS-20] Cache array length outside of loop
If not cached, the solidity compiler will always read the length of the array during each iteration. That is, if it is a storage array, this is an extra sload operation (100 additional extra gas for each iteration except for the first) and if it is a memory array, this is an extra mload operation (3 additional gas for each iteration except for the first).

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

119:     for (uint256 i = 0; i < thresholds.length; ++i) {

145:       for (uint256 i = 0; i < t.approvers.length; ++i) {

249:     for (uint256 i = 0; i < amounts.length; ++i) {

```

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

115:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

</details>

---

<a name="GAS-21"></a> 
### [GAS-21] State variables should be cached in stack variables rather than re-reading them from storage
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

```solidity
File: contracts/usdy/rUSDY.sol

/// More than 1 read for `shares`, line 516 and 509
516:     shares[_recipient] = shares[_recipient] + _sharesAmount;

```

</details>

---

<a name="GAS-22"></a> 
### [GAS-22] Use `calldata` instead of `memory` for function arguments that do not get mutated
Mark data types as `calldata` instead of `memory` where possible. This makes it so that the data is not automatically loaded into memory. If the data passed into the function does not need to be changed (like updating values in an array), it can be passed in as `calldata`. The one exception to this is if the argument must later be passed into another function that takes an argument that specifies `memory` storage.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

122:     string memory destinationChain,

```

</details>

---

<a name="GAS-23"></a> 
### [GAS-23] Use Custom Errors
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

```solidity
File: contracts/usdy/rUSDY.sol

292:     require(currentAllowance >= _amount, "TRANSFER_AMOUNT_EXCEEDS_ALLOWANCE");

420:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

435:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

475:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

476:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

504:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

505:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

532:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

564:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

569:     require(_sharesAmount <= accountShares, "BURN_AMOUNT_EXCEEDS_BALANCE");

619:       require(!_isBlocked(msg.sender), "rUSDY: 'sender' address blocked");

620:       require(!_isSanctioned(msg.sender), "rUSDY: 'sender' address sanctioned");

629:       require(!_isBlocked(from), "rUSDY: 'from' address blocked");

630:       require(!_isSanctioned(from), "rUSDY: 'from' address sanctioned");

631:       require(_isAllowed(from), "rUSDY: 'from' address not on allowlist");

636:       require(!_isBlocked(to), "rUSDY: 'to' address blocked");

637:       require(!_isSanctioned(to), "rUSDY: 'to' address sanctioned");

638:       require(_isAllowed(to), "rUSDY: 'to' address not on allowlist");

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

119:       require(success, "Call Failed");

140:     require(msg.sender == guardian, "rUSDYFactory: You are not the Guardian");

```

</details>

---

<a name="GAS-24"></a> 
### [GAS-24] Don't initialize variables with default value

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

119:     for (uint256 i = 0; i < thresholds.length; ++i) {

145:       for (uint256 i = 0; i < t.approvers.length; ++i) {

249:     for (uint256 i = 0; i < amounts.length; ++i) {

```

```solidity
File: contracts/bridge/SourceBridge.sol

164:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

63:     for (uint256 i = 0; i < length; ++i) {

99:     for (uint256 i = 0; i < length; ++i) {

115:     for (uint256 i = 0; i < length + 1; ++i) {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

115:     for (uint256 i = 0; i < exCallData.length; ++i) {

```

</details>

---

<a name="GAS-25"></a> 
### [GAS-25] Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead
Using `int`s/`uint`s smaller than 32 bytes may cost more gas. This is because the EVM operates on 32 bytes at a time, so if an element is smaller than 32 bytes, the EVM must perform more operations to reduce the size of the element from 32 bytes to the desired size.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

194:   function decimals() public pure returns (uint8) {

```

</details>

---

<a name="GAS-26"></a> 
### [GAS-26] Constructors can be marked as `payable` to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. A constructor can be safely marked as payable, because only the deployer would be able to pass funds, and the project itself would not pass any funds.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/usdy/rUSDY.sol

90:   constructor() {

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

36:   constructor(address _guardian) {

```

</details>

---

<a name="GAS-27"></a> 
### [GAS-27] Functions guaranteed to revert when called by normal users can be marked `payable`
If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function. Marking the function as `payable` will lower the gas cost for legitimate callers because the compiler will not include checks for whether a payment was provided.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

195:   function addApprover(address approver) external onlyOwner {

205:   function removeApprover(address approver) external onlyOwner {

271:   function setMintLimit(uint256 mintLimit) external onlyOwner {

280:   function setMintLimitDuration(uint256 mintDuration) external onlyOwner {

289:   function pause() external onlyOwner {

298:   function unpause() external onlyOwner {

307:   function rescueTokens(address _token) external onlyOwner {

```

```solidity
File: contracts/bridge/SourceBridge.sol

136:   function pause() external onlyOwner {

145:   function unpause() external onlyOwner {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

227:   function pauseOracle() external onlyRole(PAUSER_ROLE) {

234:   function unpauseOracle() external onlyRole(DEFAULT_ADMIN_ROLE) {

```

```solidity
File: contracts/usdy/rUSDY.sol

647:   function setOracle(address _oracle) external onlyRole(USDY_MANAGER_ROLE) {

670:   function pause() external onlyRole(PAUSER_ROLE) {

674:   function unpause() external onlyRole(USDY_MANAGER_ROLE) {

```

</details>

---

<a name="GAS-28"></a> 
### [GAS-28] `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too)
*Saves 5 gas per loop*

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bridge/SourceBridge.sol

79:     bytes memory payload = abi.encode(VERSION, msg.sender, amount, nonce++);

```

</details>

---

<a name="GAS-29"></a> 
### [GAS-29] Using `private` rather than `public` for constants, saves gas
If needed, the values can be read from the verified contract source code, or if there are multiple values there can be a single getter function that [returns a tuple](https://github.com/code-423n4/2022-08-frax/blob/90f55a9ce4e25bceed3a74290b854341d8de6afa/src/contracts/FraxlendPair.sol#L156-L178) of the values of all currently-public constants. Saves **3406-3606 gas** in deployment gas due to the compiler not having to create non-payable getter functions for deployment calldata, not having to store the bytes of the value outside of where it's used, and not adding another entry to the method ID table

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

33:   bytes32 public constant VERSION = "1.0";

```

```solidity
File: contracts/bridge/SourceBridge.sol

27:   bytes32 public constant VERSION = "1.0";

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

9:   uint256 public constant DAY = 1 days;

13:   bytes32 public constant SETTER_ROLE = keccak256("SETTER_ROLE");

14:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

```

```solidity
File: contracts/usdy/rUSDY.sol

76:   uint256 public constant BPS_DENOMINATOR = 10_000;

82:   bytes32 public constant USDY_MANAGER_ROLE = keccak256("ADMIN_ROLE");

83:   bytes32 public constant MINTER_ROLE = keccak256("MINTER_ROLE");

84:   bytes32 public constant PAUSER_ROLE = keccak256("PAUSER_ROLE");

85:   bytes32 public constant BURNER_ROLE = keccak256("BURN_ROLE");

86:   bytes32 public constant LIST_CONFIGURER_ROLE =

```

```solidity
File: contracts/usdy/rUSDYFactory.sol

29:   bytes32 public constant DEFAULT_ADMIN_ROLE = bytes32(0);

```

</details>

---

<a name="GAS-30"></a> 
### [GAS-30] Use `!= 0` instead of `> 0` for unsigned integer comparison
Using `== 0`, `!= 0` instead of `> 0`, `>= 1`, `< 1`, `<= 0` can save gas.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

144:     if (t.approvers.length > 0) {

```

```solidity
File: contracts/usdy/rUSDY.sol

420:     require(_USDYAmount > 0, "rUSDY: can't wrap zero USDY tokens");

435:     require(_rUSDYAmount > 0, "rUSDY: can't unwrap zero rUSDY tokens");

```

</details>

---

<a name="GAS-31"></a> 
### [GAS-31] Using assembly to check for zero can save gas
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

<details>
<summary>
There are <b>16</b> instances (click to show):
</summary>

```solidity
File: contracts/bridge/DestinationBridge.sol

81:     if (chainToApprovedSender[srcChain] == bytes32(0)) {

129:     if (txnToThresholdSet[txnHash].numberOfApprovalsNeeded == 0) {

250:       if (i == 0) {

```

```solidity
File: contracts/bridge/SourceBridge.sol

68:     if (bytes(destContract).length == 0) {

72:     if (msg.value == 0) {

```

```solidity
File: contracts/rwaOracles/RWADynamicOracle.sol

184:     if (indexToModify == 0) {

204:     if (indexToModify == 0) {

391:     require(y == 0 || (z = x * y) / y == x);

```

```solidity
File: contracts/usdy/rUSDY.sol

475:     require(_owner != address(0), "APPROVE_FROM_ZERO_ADDRESS");

476:     require(_spender != address(0), "APPROVE_TO_ZERO_ADDRESS");

504:     require(_sender != address(0), "TRANSFER_FROM_THE_ZERO_ADDRESS");

505:     require(_recipient != address(0), "TRANSFER_TO_THE_ZERO_ADDRESS");

532:     require(_recipient != address(0), "MINT_TO_THE_ZERO_ADDRESS");

564:     require(_account != address(0), "BURN_FROM_THE_ZERO_ADDRESS");

627:     if (from != address(0)) {

634:     if (to != address(0)) {

```

</details>

---

