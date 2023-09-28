# Report


## Medium Issues


Total <b>65</b> instances over <b>6</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | The remaining ETH may be locked in the contract after call | 7 |
| [M-2](#M-2) | Return values of `approve()` not checked | 2 |
| [M-3](#M-3) | Unchecked return value of low-level `call()`/`delegatecall()` | 12 |
| [M-4](#M-4) | Unsafe use of ERC20 `transfer()`/`transferFrom()`/`approve()` | 2 |
| [M-5](#M-5) | Use of `transferFrom()` rather than `safeTransferFrom()` for NFTs in will lead to the loss of NFTs | 1 |
| [M-6](#M-6) | Centralization Risk for trusted owners | 41 |

## Low Issues


Total <b>418</b> instances over <b>27</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Array is `push()`ed but not `pop()`ed | 12 |
| [L-2](#L-2) | Check division by zero is prevented | 12 |
| [L-3](#L-3) | Consider implementing two-step procedure for updating protocol addresses | 1 |
| [L-4](#L-4) | Constructor / initialization function lacks parameter validation | 17 |
| [L-5](#L-5) | Empty `receive()`/`fallback()` function | 3 |
| [L-6](#L-6) | Enum values should be used instead of constant array indexes | 74 |
| [L-7](#L-7) | External call recipient can consume all remaining gas | 10 |
| [L-8](#L-8) | Governance functions should be controlled by time locks | 41 |
| [L-9](#L-9) | Loss of precision in divisions | 12 |
| [L-10](#L-10) | Missing contract existence checks before low-level calls | 10 |
| [L-11](#L-11) | Missing zero address check in constructor | 10 |
| [L-12](#L-12) | Missing checks for `address(0)` when setting address state variables | 40 |
| [L-13](#L-13) | Owner can renounce Ownership | 12 |
| [L-14](#L-14) | prevent re-setting a state variable with the same value | 50 |
| [L-15](#L-15) | `receive()`/`fallback()` function does not authorize requests | 3 |
| [L-16](#L-16) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 41 |
| [L-17](#L-17) | Timestamp may be manipulation | 2 |
| [L-18](#L-18) | Unsafe downcast | 17 |
| [L-19](#L-19) | Unsafe solidity low-level call can cause gas grief attack | 10 |
| [L-20](#L-20) | Use Ownable2Step instead of Ownable | 12 |
| [L-21](#L-21) | Using zero as a parameter | 3 |
| [L-22](#L-22) | Missing zero address check in initializer | 2 |
| [L-23](#L-23) | Do not use deprecated library functions | 2 |
| [L-24](#L-24) | Empty Function Body - Consider commenting why | 8 |
| [L-25](#L-25) | Initializers could be front-run | 9 |
| [L-26](#L-26) | `safeApprove()` is deprecated | 2 |
| [L-27](#L-27) | Unspecific compiler version pragma | 3 |

## Non Critical Issues


Total <b>1838</b> instances over <b>49</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Contract declarations should have NatSpec `@author` annotations | 9 |
| [NC-2](#NC-2) | Consider adding a block/deny-list | 23 |
| [NC-3](#NC-3) | Consider adding formal verification proofs | 1 |
| [NC-4](#NC-4) | Constants should be put on the left side of comparisons | 125 |
| [NC-5](#NC-5) | Contract uses both `require()`/`revert()` as well as custom errors | 1 |
| [NC-6](#NC-6) | Contracts should have full test coverage | 1 |
| [NC-7](#NC-7) | Convert simple `if` statements to ternary expressions | 2 |
| [NC-8](#NC-8) | Events that mark critical parameter changes should contain both the old and the new value | 29 |
| [NC-9](#NC-9) | Custom errors has no error details | 90 |
| [NC-10](#NC-10) | Custom errors should be used rather than `revert()`/`require()` | 44 |
| [NC-11](#NC-11) | Solidity version is different in some files | 2 |
| [NC-12](#NC-12) | Duplicated `require()`/`revert()` checks should be refactored | 15 |
| [NC-13](#NC-13) | `else` block not required | 2 |
| [NC-14](#NC-14) | Empty bytes check is missing | 110 |
| [NC-15](#NC-15) | Enable IR-based code generation | 1 |
| [NC-16](#NC-16) | Events are emitted without the sender information | 25 |
| [NC-17](#NC-17) | Functions with array parameters should have length checks in place | 18 |
| [NC-18](#NC-18) | Import declarations should import specific identifiers, rather than the whole file | 1 |
| [NC-19](#NC-19) | Large or complicated code bases should implement invariant tests | 1 |
| [NC-20](#NC-20) | Missing zero address check in functions with address parameters | 264 |
| [NC-21](#NC-21) | Consider moving `msg.sender` checks to `modifier`s | 1 |
| [NC-22](#NC-22) | NatSpec documentation for contract is missing | 21 |
| [NC-23](#NC-23) | Event declarations should have NatSpec descriptions | 28 |
| [NC-24](#NC-24) | NatSpec documentation for function is missing | 40 |
| [NC-25](#NC-25) | Missing NatSpec `@param` | 151 |
| [NC-26](#NC-26) | NatSpec `@return` is missing | 63 |
| [NC-27](#NC-27) | There is no need to initialize variables with 0 | 17 |
| [NC-28](#NC-28) | Put all system-wide constants in one file | 22 |
| [NC-29](#NC-29) | State variables should include comments | 77 |
| [NC-30](#NC-30) | Contract declarations should have NatSpec `@title` annotations | 4 |
| [NC-31](#NC-31) | Lines are too long | 2 |
| [NC-32](#NC-32) | Unused errors | 84 |
| [NC-33](#NC-33) | Unused contract variables | 2 |
| [NC-34](#NC-34) | Consider using `delete` rather than assigning zero to clear values | 22 |
| [NC-35](#NC-35) | Solidity compiler version is not fixed | 44 |
| [NC-36](#NC-36) | Expressions for constant values should use `immutable` rather than `constant` | 22 |
| [NC-37](#NC-37) | Use `@inheritdoc` for overridden functions | 55 |
| [NC-38](#NC-38) | Use the latest solidity version for deployment | 44 |
| [NC-39](#NC-39) | Use of `override` is unnecessary | 78 |
| [NC-40](#NC-40) | Visibility of state variables is not explicitly defined | 72 |
| [NC-41](#NC-41) | Missing checks for `address(0)` when assigning values to address state variables | 7 |
| [NC-42](#NC-42) | Common functions should be refactored to a common base contract | 146 |
| [NC-43](#NC-43) | Names of `private`/`internal` functions should be prefixed with an underscore | 2 |
| [NC-44](#NC-44) | Names of `private`/`internal` state variables should be prefixed with an underscore | 23 |
| [NC-45](#NC-45) |  `require()` / `revert()` statements should have descriptive reason strings | 5 |
| [NC-46](#NC-46) | Return values of `approve()` not checked | 2 |
| [NC-47](#NC-47) | Variables should be named in mixedCase style | 29 |
| [NC-48](#NC-48) | Event is missing `indexed` fields | 3 |
| [NC-49](#NC-49) | Functions not used internally could be marked external | 8 |

## Gas Optimizations


Total <b>1013</b> instances over <b>36</b> issues:

|ID|Issue|Instances|Gas|
|-|:-|:-:|:-:|
| [GAS-1](#GAS-1) | Consider activating via-ir for deploying | 1 | - |
| [GAS-2](#GAS-2) | Divisions can be `unchecked` to save gas | 12 | 240 |
| [GAS-3](#GAS-3) | Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables | 6 | 678 |
| [GAS-4](#GAS-4) | Duplicated `require()`/`revert()` checks should be refactored to a modifier or function to save gas | 15 | - |
| [GAS-5](#GAS-5) | Increments can be `unchecked` to save gas | 14 | 840 |
| [GAS-6](#GAS-6) | Initializers can be marked as payable to save deployment gas | 9 | 189 |
| [GAS-7](#GAS-7) | `internal` functions only called once can be inlined to save gas | 15 | 450 |
| [GAS-8](#GAS-8) | Low level `call` can be optimized with assembly | 16 | 3968 |
| [GAS-9](#GAS-9) | Multiple accesses of the same mapping/array key/index should be cached | 27 | 1134 |
| [GAS-10](#GAS-10) | Newer versions of solidity are more gas efficient | 44 | - |
| [GAS-11](#GAS-11) | Operator `>=`/`<=` costs less gas than operator `>`/`<` | 48 | 144 |
| [GAS-12](#GAS-12) | Reduce gas usage by moving to Solidity 0.8.19 or later | 41 | 41000 |
| [GAS-13](#GAS-13) | Redundant state variable getters | 2 | - |
| [GAS-14](#GAS-14) | Remove or replace unused state variables | 2 | - |
| [GAS-15](#GAS-15) | `require()`/`revert()` strings longer than 32 bytes cost extra gas | 22 | 66 |
| [GAS-16](#GAS-16) | The result of a function call should be cached rather than re-calling the function | 55 | 5500 |
| [GAS-17](#GAS-17) | Unlimited gas consumption risk due to external call recipients | 10 | - |
| [GAS-18](#GAS-18) | Use assembly to compute hashes to save gas | 1 | 80 |
| [GAS-19](#GAS-19) | Use assembly to emit events | 29 | 1102 |
| [GAS-20](#GAS-20) | Using a double `if` statement instead of a logical AND (`&&`) | 1 | 30 |
| [GAS-21](#GAS-21) | Use a more recent version of solidity | 44 | - |
| [GAS-22](#GAS-22) | Use `unchecked` block for safe subtractions | 4 | 340 |
| [GAS-23](#GAS-23) | Using bitmap to store bool states can save gas | 10 | - |
| [GAS-24](#GAS-24) | Use `selfbalance()` instead of `address(this).balance` | 9 | - |
| [GAS-25](#GAS-25) | Using bools for storage incurs overhead | 13 | - |
| [GAS-26](#GAS-26) | Cache array length outside of loop | 8 | - |
| [GAS-27](#GAS-27) | State variables should be cached in stack variables rather than re-reading them from storage | 8 | 776 |
| [GAS-28](#GAS-28) | Use `calldata` instead of `memory` for function arguments that do not get mutated | 70 | - |
| [GAS-29](#GAS-29) | Use Custom Errors | 44 | 2200 |
| [GAS-30](#GAS-30) | Don't initialize variables with default value | 17 | - |
| [GAS-31](#GAS-31) | Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead | 281 | 15455 |
| [GAS-32](#GAS-32) | Constructors can be marked as `payable` to save deployment gas | 14 | 294 |
| [GAS-33](#GAS-33) | Functions guaranteed to revert when called by normal users can be marked `payable` | 21 | 441 |
| [GAS-34](#GAS-34) | `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too) | 5 | 25 |
| [GAS-35](#GAS-35) | Use `!= 0` instead of `> 0` for unsigned integer comparison | 21 | 84 |
| [GAS-36](#GAS-36) | Using assembly to check for zero can save gas | 74 | 444 |

## Medium Issues

<a name="M-1"></a> 
### [M-1] The remaining ETH may be locked in the contract after call
After calling an external contract and forwards some ETH value, the contract balance should be checked. If there is excess eth left over due to a failed call, or more eth being delivered than needed, or any other reason, this eth must be refunded to the user or handled appropriately, otherwise the eth may be frozen in the contract forever.

<details>
<summary>
There are <b>7</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

103:         _rootBridgeAgentAddress.call{value: msg.value}("");

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L103) 

```solidity
File: src/BranchBridgeAgent.sol

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

```
[#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) [#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) 

```solidity
File: src/RootBridgeAgent.sol

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

835:             callee.call{value: msg.value}("");

927:             callee.call{value: _value}("");

```
[#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L835](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L835) [#L927](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L927) 

</details>

---

<a name="M-2"></a> 
### [M-2] Return values of `approve()` not checked
Not all IERC20 implementations `revert()` when there's a failure in `approve()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually approving anything

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

168:                 ERC20(_hToken).approve(_localPortAddress, _amount - _deposit);

175:             ERC20(_token).approve(_localPortAddress, _deposit);

```
[#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L168) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L175) 

</details>

---

<a name="M-3"></a> 
### [M-3] Unchecked return value of low-level `call()`/`delegatecall()`
The function being called may revert, which will be indicated by the return value to `call()`/`delegatecall()`. If the return value is not checked, the code will continue on as if there was no error, rather than reverting with the error encountered.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

103:         _rootBridgeAgentAddress.call{value: msg.value}("");

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L103) 

```solidity
File: src/MulticallRootRouter.sol

239:             IVirtualAccount(userAccount).call(calls);

248:             IVirtualAccount(userAccount).call(calls);

275:             IVirtualAccount(userAccount).call(calls);

328:             IVirtualAccount(userAccount).call(calls);

337:             IVirtualAccount(userAccount).call(calls);

364:             IVirtualAccount(userAccount).call(calls);

416:             IVirtualAccount(userAccount).call(calls);

425:             IVirtualAccount(userAccount).call(calls);

452:             IVirtualAccount(userAccount).call(calls);

```
[#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L239) [#L248](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L248) [#L275](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L275) [#L328](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L328) [#L337](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L337) [#L364](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L364) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L416) [#L425](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L425) [#L452](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L452) 

```solidity
File: src/RootBridgeAgent.sol

835:             callee.call{value: msg.value}("");

927:             callee.call{value: _value}("");

```
[#L835](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L835) [#L927](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L927) 

</details>

---

<a name="M-4"></a> 
### [M-4] Unsafe use of ERC20 `transfer()`/`transferFrom()`/`approve()`
Some tokens do not implement the ERC20 standard properly. For example Tether (USDT)'s `transfer()` and `transferFrom()` functions do not return booleans as the ERC20 specification requires, and instead have no return value. When these sorts of tokens are cast to IERC20/ERC20, their function signatures do not match and therefore the calls made will revert.It is recommended to use the [`SafeERC20`](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/f347b410cf6aeeaaf5197e1fece139c793c03b2b/contracts/token/ERC20/utils/SafeERC20.sol#L19)'s `safeTransfer()` and `safeTransferFrom()` from OpenZeppelin instead.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

168:                 ERC20(_hToken).approve(_localPortAddress, _amount - _deposit);

175:             ERC20(_token).approve(_localPortAddress, _deposit);

```
[#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L168) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L175) 

</details>

---

<a name="M-5"></a> 
### [M-5] Use of `transferFrom()` rather than `safeTransferFrom()` for NFTs in will lead to the loss of NFTs
The EIP-721 standard says the following about `transferFrom()`:

```solidity
/// @notice Transfer ownership of an NFT -- THE CALLER IS RESPONSIBLE
///  TO CONFIRM THAT `_to` IS CAPABLE OF RECEIVING NFTS OR ELSE
///  THEY MAY BE PERMANENTLY LOST
/// @dev Throws unless `msg.sender` is the current owner, an authorized
///  operator, or the approved address for this NFT. Throws if `_from` is
///  not the current owner. Throws if `_to` is the zero address. Throws if
///  `_tokenId` is not a valid NFT.
/// @param _from The current owner of the NFT
/// @param _to The new owner
/// @param _tokenId The NFT to transfer
function transferFrom(address _from, address _to, uint256 _tokenId) external payable;
```

https://github.com/ethereum/EIPs/blob/78e2c297611f5e92b6a5112819ab71f74041ff25/EIPS/eip-721.md?plain=1#L103-L113

Code must use the `safeTransferFrom()` flavor if it hasn't otherwise verified that the receiving address can handle it

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: src/VirtualAccount.sol

62:         ERC721(_token).transferFrom(address(this), msg.sender, _tokenId);

```
[#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L62) 

</details>

---

<a name="M-6"></a> 
### [M-6] Centralization Risk for trusted owners
Contracts have owners with privileged rights to perform admin tasks and need to be trusted to not perform malicious updates or drain funds.

<details>
<summary>
There are <b>41</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

25: contract BaseBranchRouter is IBranchRouter, Ownable {

60:     function initialize(address _localBridgeAgentAddress) external onlyOwner {

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L25) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L60) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

29: contract BranchBridgeAgentExecutor is Ownable, BridgeAgentConstants {

53:     function executeNoSettlement(address _router, bytes calldata _payload) external payable onlyOwner {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L29) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L53) 

```solidity
File: src/BranchPort.sol

17: contract BranchPort is Ownable, IBranchPort {

122:     function initialize(address _coreBranchRouter, address _bridgeAgentFactory) external virtual onlyOwner {

135:     function renounceOwnership() public payable override onlyOwner {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L17) [#L122](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L122) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L135) 

```solidity
File: src/CoreRootRouter.sol

38: contract CoreRootRouter is IRootRouter, Ownable {

83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

162:     ) external payable onlyOwner {

191:     ) external payable onlyOwner {

218:     ) external payable onlyOwner {

249:     ) external payable onlyOwner {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L38) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) [#L162](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L162) [#L191](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L191) [#L218](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L218) [#L249](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L249) 

```solidity
File: src/MulticallRootRouter.sol

57: contract MulticallRootRouter is IRootRouter, Ownable {

109:     function initialize(address _bridgeAgentAddress) external onlyOwner {

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L57) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L109) 

```solidity
File: src/RootBridgeAgentExecutor.sol

27: contract RootBridgeAgentExecutor is Ownable, BridgeAgentConstants {

206:     ) external payable onlyOwner {

```
[#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L27) [#L206](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L206) 

```solidity
File: src/RootPort.sol

16: contract RootPort is Ownable, IRootPort {

129:     function initialize(address _bridgeAgentFactory, address _coreRootRouter) external onlyOwner {

151:     ) external onlyOwner {

166:     function renounceOwnership() public payable override onlyOwner {

414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

421:     function addBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

431:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

446:     ) external override onlyOwner {

483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

509:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external override onlyOwner {

527:     ) external payable override onlyOwner {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L16) [#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L129) [#L151](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L151) [#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L166) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L421) [#L431](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L431) [#L446](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L446) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) [#L509](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L509) [#L527](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L527) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

```
[#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

19: contract BranchBridgeAgentFactory is Ownable, IBranchBridgeAgentFactory {

87:     function initialize(address _coreRootBridgeAgent) external virtual onlyOwner {

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L19) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L87) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

12: contract ERC20hTokenBranchFactory is Ownable, IERC20hTokenBranchFactory {

60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L12) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

12: contract ERC20hTokenRootFactory is Ownable, IERC20hTokenRootFactory {

49:     function initialize(address _coreRouter) external onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L12) [#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L49) 

```solidity
File: src/token/ERC20hTokenBranch.sol

12: contract ERC20hTokenBranch is ERC20, Ownable, IERC20hTokenBranch {

29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

35:     function burn(uint256 amount) public override onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L12) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L35) 

```solidity
File: src/token/ERC20hTokenRoot.sol

12: contract ERC20hTokenRoot is ERC20, Ownable, IERC20hTokenRoot {

57:     function mint(address to, uint256 amount, uint256 chainId) external onlyOwner returns (bool) {

69:     function burn(address from, uint256 amount, uint256 chainId) external onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L12) [#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L57) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L69) 

</details>

---


## Low Issues

<a name="L-1"></a> 
### [L-1] Array is `push()`ed but not `pop()`ed
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

131:         bridgeAgentFactories.push(_bridgeAgentFactory);

323:         bridgeAgents.push(_bridgeAgent);

342:         bridgeAgentFactories.push(_newBridgeAgentFactory);

367:         strategyTokens.push(_token);

388:         portStrategies.push(_portStrategy);

421:         bridgeAgents.push(_coreBranchBridgeAgent);

```
[#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L131) [#L323](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L323) [#L342](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L342) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L367) [#L388](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L388) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L421) 

```solidity
File: src/RootPort.sol

136:         bridgeAgentFactories.push(_bridgeAgentFactory);

385:         bridgeAgents.push(_bridgeAgent);

424:         bridgeAgentFactories.push(_bridgeAgentFactory);

```
[#L136](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L136) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L385) [#L424](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L424) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

72:         hTokens.push(newToken);

104:         hTokens.push(newToken);

```
[#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L72) [#L104](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L104) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

89:         hTokens.push(newToken);

```
[#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L89) 

</details>

---

<a name="L-2"></a> 
### [L-2] Check division by zero is prevented

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

176:                     USER / BRANCH ROUTER EXTERNAL FUNCTIONS

```
[#L176](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L176) 

```solidity
File: src/BranchPort.sol

473:         return ((_currBalance + _strategyTokenDebt) * getMinimumTokenReserveRatio[_token]) / DIVISIONER;

490:                 lastManaged[msg.sender][_token] = (block.timestamp / 1 days) * 1 days;

```
[#L473](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L473) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L490) 

```solidity
File: src/CoreRootRouter.sol

145:                 GOVERNANCE / ADMIN EXTERNAL FUNCTIONS

```
[#L145](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L145) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

25:     address token; //Input Native / underlying Token Address.

33:     address[] tokens; //Input Native / underlying Token Address.

43:     address[] tokens; //Input Native / underlying Token Address.

52:     address token; //Input Native / underlying Token Address.

63:     address[] tokens; //Input Native / underlying Token Addresses.

84:     address token; // Input Native / underlying Token Address.

94:     address[] tokens; // Input Native / underlying Token Addresses.

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L25) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L33) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L43) [#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L52) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L63) [#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L84) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L94) 

```solidity
File: src/interfaces/IBranchRouter.sol

23:                             VIEW / STATE

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L23) 

</details>

---

<a name="L-3"></a> 
### [L-3] Consider implementing two-step procedure for updating protocol addresses
A copy-paste error or a typo may end up bricking protocol functionality, or sending tokens to an address with no known private key. Consider implementing a two-step procedure for updating protocol addresses, where the recipient is set as pending, and must "accept" the assignment by making an affirmative call. A straight forward way of doing this would be to have the target contracts implement [EIP-165](https://eips.ethereum.org/EIPS/eip-165), and to have the "set" functions ensure that the recipient is of the right interface type.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: src/RootPort.sol

509:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external override onlyOwner {

```
[#L509](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L509) 

</details>

---

<a name="L-4"></a> 
### [L-4] Constructor / initialization function lacks parameter validation
Constructors and initialization functions play a critical role in contracts by setting important initial states when the contract is first deployed before the system starts. The parameters passed to the constructor and initialization functions directly affect the behavior of the contract / protocol. If incorrect parameters are provided, the system may fail to run, behave abnormally, be unstable, or lack security. Therefore, it's crucial to carefully check each parameter in the constructor and initialization functions. If an exception is found, the transaction should be rolled back.

<details>
<summary>
There are <b>17</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// Empty constructor/initializer, lack of parameter validation
43:     constructor(

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L43) 

```solidity
File: src/ArbitrumBranchPort.sol

/// `_owner` not validated
38:     constructor(uint16 _localChainId, address _rootPortAddress, address _owner) BranchPort(_owner) {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L38) 

```solidity
File: src/BaseBranchRouter.sol

/// `_localBridgeAgentAddress` not validated
60:     function initialize(address _localBridgeAgentAddress) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L60) 

```solidity
File: src/BranchPort.sol

/// `_coreBranchRouter` not validated
/// `_bridgeAgentFactory` not validated
122:     function initialize(address _coreBranchRouter, address _bridgeAgentFactory) external virtual onlyOwner {

```
[#L122](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L122) 

```solidity
File: src/CoreRootRouter.sol

/// `_bridgeAgentAddress` not validated
/// `_hTokenFactory` not validated
83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) 

```solidity
File: src/MulticallRootRouter.sol

/// `_bridgeAgentAddress` not validated
109:     function initialize(address _bridgeAgentAddress) external onlyOwner {

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L109) 

```solidity
File: src/MulticallRootRouterLibZip.sol

/// Empty constructor/initializer, lack of parameter validation
29:     constructor(uint256 _localChainId, address _localPortAddress, address _multicallAddress)

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L29) 

```solidity
File: src/RootBridgeAgentExecutor.sol

/// `_rootBridgeAgent` not validated
35:     constructor(address _rootBridgeAgent) {

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L35) 

```solidity
File: src/RootPort.sol

/// `_bridgeAgentFactory` not validated
/// `_coreRootRouter` not validated
129:     function initialize(address _bridgeAgentFactory, address _coreRootRouter) external onlyOwner {

```
[#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L129) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

/// Empty constructor/initializer, lack of parameter validation
30:     constructor(

/// `_coreRootBridgeAgent` not validated
56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

```
[#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L30) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

/// `_coreRootBridgeAgent` not validated
87:     function initialize(address _coreRootBridgeAgent) external virtual onlyOwner {

```
[#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L87) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

/// `_chainName` not validated
/// `_chainSymbol` not validated
42:     constructor(uint16 _localChainId, address _localPortAddress, string memory _chainName, string memory _chainSymbol) {

/// `_wrappedNativeTokenAddress` not validated
/// `_coreRouter` not validated
60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L42) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

/// `_coreRouter` not validated
49:     function initialize(address _coreRouter) external onlyOwner {

```
[#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L49) 

```solidity
File: src/token/ERC20hTokenBranch.sol

/// `chainName` not validated
/// `chainSymbol` not validated
/// `_name` not validated
/// `_symbol` not validated
/// `_decimals` not validated
/// `_owner` not validated
13:     constructor(
            string memory chainName,
            string memory chainSymbol,
            string memory _name,
            string memory _symbol,
            uint8 _decimals,
            address _owner
        ) ERC20(string(string.concat(chainName, _name)), string(string.concat(chainSymbol, _symbol)), _decimals) {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L13) 

```solidity
File: src/token/ERC20hTokenRoot.sol

/// `_name` not validated
/// `_symbol` not validated
/// `_decimals` not validated
31:     constructor(
            uint16 _localChainId,
            address _factoryAddress,
            address _rootPortAddress,
            string memory _name,
            string memory _symbol,
            uint8 _decimals
        ) ERC20(string(string.concat(_name)), string(string.concat(_symbol)), _decimals) {

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L31) 

</details>

---

<a name="L-5"></a> 
### [L-5] Empty `receive()`/`fallback()` function
If the intention is for Ether sent by a caller to be used for an actual purpose (i.e. the function is not just a WETH `withdraw()` handler), the function should call another function (e.g. call `weth.deposit()` and use the token on the caller's behalf) or at least emit an event to track that funds were sent directly to it.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

149:     receive() external payable {}

```
[#L149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L149) 

```solidity
File: src/RootBridgeAgent.sol

128:     receive() external payable {}

```
[#L128](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L128) 

```solidity
File: src/VirtualAccount.sol

44:     receive() external payable {}

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L44) 

</details>

---

<a name="L-6"></a> 
### [L-6] Enum values should be used instead of constant array indexes
Create a commented enum value to use instead of constant array indexes, this makes the code far easier to understand.

<details>
<summary>
There are <b>74</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

89:     function retrySettlement(uint32, bytes calldata, GasParams[2] calldata, bool) external payable override lock {}

```
[#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L89) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

127:         if (_data[0] == 0x02) {

146:         } else if (_data[0] == 0x03) {

152:         } else if (_data[0] == 0x04) {

157:         } else if (_data[0] == 0x05) {

162:         } else if (_data[0] == 0x06) {

```
[#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L127) [#L146](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L146) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L152) [#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L157) [#L162](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L162) 

```solidity
File: src/BranchBridgeAgent.sol

366:                     deposit.hTokens[0],

367:                     deposit.tokens[0],

368:                     deposit.amounts[0],

369:                     deposit.deposits[0],

376:                     deposit.hTokens[0],

377:                     deposit.tokens[0],

378:                     deposit.amounts[0],

379:                     deposit.deposits[0],

467:         GasParams[2] calldata _gParams,

471:         bytes memory params = abi.encode(_settlementNonce, msg.sender, _params, _gParams[1]);

477:         _performCall(payable(msg.sender), payload, _gParams[0]);

501:         uint8 numOfAssets = uint8(bytes1(_sParams[0]));

593:         bytes1 flag = _payload[0] & 0x7F;

629:                 _payload[0] == 0x81,

651:                 _payload[0] == 0x82,

834:         addressArray[0] = _hToken;

837:         addressArray[0] = _token;

840:         uintArray[0] = _amount;

843:         uintArray[0] = _deposit;

```
[#L366](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L366) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L367) [#L368](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L368) [#L369](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L369) [#L376](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L376) [#L377](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L377) [#L378](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L378) [#L379](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L379) [#L467](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L467) [#L471](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L471) [#L477](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L477) [#L501](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L501) [#L593](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L593) [#L629](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L629) [#L651](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L651) [#L834](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L834) [#L837](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L837) [#L840](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L840) [#L843](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L843) 

```solidity
File: src/CoreBranchRouter.sol

43:     function addGlobalToken(address _globalAddress, uint256 _dstChainId, GasParams[3] calldata _gParams)

48:         bytes memory params = abi.encode(msg.sender, _globalAddress, _dstChainId, [_gParams[1], _gParams[2]]);

48:         bytes memory params = abi.encode(msg.sender, _globalAddress, _dstChainId, [_gParams[1], _gParams[2]]);

54:         IBridgeAgent(localBridgeAgentAddress).callOut{value: msg.value}(payable(msg.sender), payload, _gParams[0]);

88:         if (_params[0] == 0x01) {

100:         } else if (_params[0] == 0x02) {

115:         } else if (_params[0] == 0x03) {

121:         } else if (_params[0] == 0x04) {

127:         } else if (_params[0] == 0x05) {

133:         } else if (_params[0] == 0x06) {

140:         } else if (_params[0] == 0x07) {

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L43) [#L48](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L48) [#L48](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L48) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L54) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L88) [#L100](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L100) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L115) [#L121](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L121) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L127) [#L133](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L133) [#L140](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L140) 

```solidity
File: src/CoreRootRouter.sol

109:         GasParams[2] calldata _gParams

132:             _gParams[1]

140:             payable(_refundee), _refundee, _dstChainId, payload, _gParams[0]

304:         bytes1 funcId = _encodedData[0];

334:         bytes1 funcId = _encodedData[0];

338:             (address refundee, address globalAddress, uint16 dstChainId, GasParams[2] memory gasParams) =

339:                 abi.decode(_encodedData[1:], (address, address, uint16, GasParams[2]));

410:         GasParams[2] memory _gParams

430:             _gParams[1]

438:             payable(_refundee), _refundee, _dstChainId, payload, _gParams[0]

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L109) [#L132](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L132) [#L140](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L140) [#L304](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L304) [#L334](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L334) [#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L338) [#L339](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L339) [#L410](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L410) [#L430](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L430) [#L438](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L438) 

```solidity
File: src/MulticallRootRouter.sol

139:         bytes1 funcId = encodedData[0];

231:         bytes1 funcId = encodedData[0];

320:         bytes1 funcId = encodedData[0];

408:         bytes1 funcId = encodedData[0];

```
[#L139](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L139) [#L231](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L231) [#L320](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L320) [#L408](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L408) 

```solidity
File: src/RootBridgeAgent.sol

444:         if (_payload[0] == 0x00) {

467:         } else if (_payload[0] == 0x01) {

490:         } else if (_payload[0] == 0x02) {

513:         } else if (_payload[0] == 0x03) {

539:         } else if (_payload[0] == 0x04) {

577:         } else if (_payload[0] & 0x7F == 0x05) {

600:                 _payload[0] == 0x85,

617:         } else if (_payload[0] & 0x7F == 0x06) {

640:                 _payload[0] == 0x86,

657:         } else if (_payload[0] & 0x7F == 0x07) {

684:                 _payload[0] == 0x87,

699:         } else if (_payload[0] == 0x08) {

718:         } else if (_payload[0] == 0x09) {

883:                 _hTokens[0],

884:                 _tokens[0],

885:                 _amounts[0],

886:                 _deposits[0],

1017:         addressArray[0] = localAddress;

1020:         addressArray[0] = underlyingAddress;

1023:         uintArray[0] = _amount;

1026:         uintArray[0] = _deposit;

```
[#L444](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L444) [#L467](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L467) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L490) [#L513](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L513) [#L539](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L539) [#L577](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L577) [#L600](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L600) [#L617](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L617) [#L640](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L640) [#L657](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L657) [#L684](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L684) [#L699](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L699) [#L718](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L718) [#L883](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L883) [#L884](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L884) [#L885](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L885) [#L886](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L886) [#L1017](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1017) [#L1020](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1020) [#L1023](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1023) [#L1026](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1026) 

```solidity
File: src/RootBridgeAgentExecutor.sol

273:         uint8 numOfAssets = uint8(bytes1(_dParams[0]));

```
[#L273](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L273) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

288:         GasParams[2] calldata gasParams,

```
[#L288](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L288) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

38:     function addGlobalToken(address _globalAddress, uint256 _dstChainId, GasParams[3] calldata _gasParams)

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L38) 

</details>

---

<a name="L-7"></a> 
### [L-7] External call recipient can consume all remaining gas
There is no limit specified on the amount of gas used, so the recipient can use up all of the remaining gas (`gasleft()`), causing it to revert. Therefore, when calling an external contract, it is necessary to specify a limited amount of gas to forward.

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

103:         _rootBridgeAgentAddress.call{value: msg.value}("");

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L103) 

```solidity
File: src/BranchBridgeAgent.sol

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

```
[#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) [#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) 

```solidity
File: src/MulticallRootRouter.sol

239:             IVirtualAccount(userAccount).call(calls);

328:             IVirtualAccount(userAccount).call(calls);

416:             IVirtualAccount(userAccount).call(calls);

```
[#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L239) [#L328](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L328) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L416) 

```solidity
File: src/RootBridgeAgent.sol

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

835:             callee.call{value: msg.value}("");

927:             callee.call{value: _value}("");

```
[#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L835](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L835) [#L927](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L927) 

</details>

---

<a name="L-8"></a> 
### [L-8] Governance functions should be controlled by time locks
Governance functions (such as upgrading contracts, setting critical parameters) should be controlled using time locks to introduce a delay between a proposal and its execution. This gives users time to exit before a potentially dangerous or malicious operation is applied.

<details>
<summary>
There are <b>41</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

25: contract BaseBranchRouter is IBranchRouter, Ownable {

60:     function initialize(address _localBridgeAgentAddress) external onlyOwner {

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L25) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L60) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

29: contract BranchBridgeAgentExecutor is Ownable, BridgeAgentConstants {

53:     function executeNoSettlement(address _router, bytes calldata _payload) external payable onlyOwner {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L29) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L53) 

```solidity
File: src/BranchPort.sol

17: contract BranchPort is Ownable, IBranchPort {

122:     function initialize(address _coreBranchRouter, address _bridgeAgentFactory) external virtual onlyOwner {

135:     function renounceOwnership() public payable override onlyOwner {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L17) [#L122](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L122) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L135) 

```solidity
File: src/CoreRootRouter.sol

38: contract CoreRootRouter is IRootRouter, Ownable {

83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

162:     ) external payable onlyOwner {

191:     ) external payable onlyOwner {

218:     ) external payable onlyOwner {

249:     ) external payable onlyOwner {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L38) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) [#L162](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L162) [#L191](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L191) [#L218](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L218) [#L249](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L249) 

```solidity
File: src/MulticallRootRouter.sol

57: contract MulticallRootRouter is IRootRouter, Ownable {

109:     function initialize(address _bridgeAgentAddress) external onlyOwner {

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L57) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L109) 

```solidity
File: src/RootBridgeAgentExecutor.sol

27: contract RootBridgeAgentExecutor is Ownable, BridgeAgentConstants {

206:     ) external payable onlyOwner {

```
[#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L27) [#L206](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L206) 

```solidity
File: src/RootPort.sol

16: contract RootPort is Ownable, IRootPort {

129:     function initialize(address _bridgeAgentFactory, address _coreRootRouter) external onlyOwner {

151:     ) external onlyOwner {

166:     function renounceOwnership() public payable override onlyOwner {

414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

421:     function addBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

431:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

446:     ) external override onlyOwner {

483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

509:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external override onlyOwner {

527:     ) external payable override onlyOwner {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L16) [#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L129) [#L151](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L151) [#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L166) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L421) [#L431](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L431) [#L446](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L446) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) [#L509](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L509) [#L527](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L527) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

```
[#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

19: contract BranchBridgeAgentFactory is Ownable, IBranchBridgeAgentFactory {

87:     function initialize(address _coreRootBridgeAgent) external virtual onlyOwner {

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L19) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L87) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

12: contract ERC20hTokenBranchFactory is Ownable, IERC20hTokenBranchFactory {

60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L12) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

12: contract ERC20hTokenRootFactory is Ownable, IERC20hTokenRootFactory {

49:     function initialize(address _coreRouter) external onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L12) [#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L49) 

```solidity
File: src/token/ERC20hTokenBranch.sol

12: contract ERC20hTokenBranch is ERC20, Ownable, IERC20hTokenBranch {

29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

35:     function burn(uint256 amount) public override onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L12) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L35) 

```solidity
File: src/token/ERC20hTokenRoot.sol

12: contract ERC20hTokenRoot is ERC20, Ownable, IERC20hTokenRoot {

57:     function mint(address to, uint256 amount, uint256 chainId) external onlyOwner returns (bool) {

69:     function burn(address from, uint256 amount, uint256 chainId) external onlyOwner {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L12) [#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L57) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L69) 

</details>

---

<a name="L-9"></a> 
### [L-9] Loss of precision in divisions
Division by large numbers may result in the result being zero, due to solidity not supporting fractions. Consider requiring a minimum amount for the numerator to ensure that it is always larger than the denominator.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

176:                     USER / BRANCH ROUTER EXTERNAL FUNCTIONS

```
[#L176](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L176) 

```solidity
File: src/BranchPort.sol

473:         return ((_currBalance + _strategyTokenDebt) * getMinimumTokenReserveRatio[_token]) / DIVISIONER;

490:                 lastManaged[msg.sender][_token] = (block.timestamp / 1 days) * 1 days;

```
[#L473](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L473) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L490) 

```solidity
File: src/CoreRootRouter.sol

145:                 GOVERNANCE / ADMIN EXTERNAL FUNCTIONS

```
[#L145](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L145) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

25:     address token; //Input Native / underlying Token Address.

33:     address[] tokens; //Input Native / underlying Token Address.

43:     address[] tokens; //Input Native / underlying Token Address.

52:     address token; //Input Native / underlying Token Address.

63:     address[] tokens; //Input Native / underlying Token Addresses.

84:     address token; // Input Native / underlying Token Address.

94:     address[] tokens; // Input Native / underlying Token Addresses.

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L25) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L33) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L43) [#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L52) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L63) [#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L84) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L94) 

```solidity
File: src/interfaces/IBranchRouter.sol

23:                             VIEW / STATE

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L23) 

</details>

---

<a name="L-10"></a> 
### [L-10] Missing contract existence checks before low-level calls
Low-level calls return success if there is no code present at the specified address. In addition to the zero-address checks, add a check to verify that `<address>.code.length > 0`

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

103:         _rootBridgeAgentAddress.call{value: msg.value}("");

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L103) 

```solidity
File: src/BranchBridgeAgent.sol

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

```
[#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) [#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) 

```solidity
File: src/MulticallRootRouter.sol

239:             IVirtualAccount(userAccount).call(calls);

328:             IVirtualAccount(userAccount).call(calls);

416:             IVirtualAccount(userAccount).call(calls);

```
[#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L239) [#L328](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L328) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L416) 

```solidity
File: src/RootBridgeAgent.sol

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

835:             callee.call{value: msg.value}("");

927:             callee.call{value: _value}("");

```
[#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L835](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L835) [#L927](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L927) 

</details>

---

<a name="L-11"></a> 
### [L-11] Missing zero address check in constructor
Constructors often take address parameters to initialize important components of a contract, such as owner or linked contracts. However, without a checking, there's a risk that an address parameter could be mistakenly set to the zero address (0x0). This could be due to an error or oversight during contract deployment. A zero address in a crucial role can cause serious issues, as it cannot perform actions like a normal address, and any funds sent to it will be irretrievable. It's therefore crucial to include a zero address check in constructors to prevent such potential problems. If a zero address is detected, the constructor should revert the transaction.

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// Missing zero check for `_rootBridgeAgentAddress`
/// Missing zero check for `_localRouterAddress`
/// Missing zero check for `_localPortAddress`
43:     constructor(
            uint16 _localChainId,
            address _rootBridgeAgentAddress,
            address _localRouterAddress,
            address _localPortAddress
        )
            BranchBridgeAgent(
                _localChainId,
                _localChainId,
                _rootBridgeAgentAddress,
                address(0),
                _localRouterAddress,
                _localPortAddress
            )
        {}

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L43) 

```solidity
File: src/ArbitrumBranchPort.sol

/// Missing zero check for `_owner`
38:     constructor(uint16 _localChainId, address _rootPortAddress, address _owner) BranchPort(_owner) {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L38) 

```solidity
File: src/CoreBranchRouter.sol

/// Missing zero check for `_hTokenFactoryAddress`
30:     constructor(address _hTokenFactoryAddress) BaseBranchRouter() {

```
[#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L30) 

```solidity
File: src/CoreRootRouter.sol

/// Missing zero check for `_rootPortAddress`
71:     constructor(uint256 _rootChainId, address _rootPortAddress) {

```
[#L71](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L71) 

```solidity
File: src/MulticallRootRouterLibZip.sol

/// Missing zero check for `_localPortAddress`
/// Missing zero check for `_multicallAddress`
29:     constructor(uint256 _localChainId, address _localPortAddress, address _multicallAddress)
            MulticallRootRouter(_localChainId, _localPortAddress, _multicallAddress)
        {}

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L29) 

```solidity
File: src/RootBridgeAgentExecutor.sol

/// Missing zero check for `_rootBridgeAgent`
35:     constructor(address _rootBridgeAgent) {

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L35) 

```solidity
File: src/VirtualAccount.sol

/// Missing zero check for `_userAddress`
/// Missing zero check for `_localPortAddress`
35:     constructor(address _userAddress, address _localPortAddress) {

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L35) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

/// Missing zero check for `_rootBridgeAgentFactoryAddress`
/// Missing zero check for `_localCoreBranchRouterAddress`
/// Missing zero check for `_localPortAddress`
/// Missing zero check for `_owner`
30:     constructor(
            uint16 _rootChainId,
            address _rootBridgeAgentFactoryAddress,
            address _localCoreBranchRouterAddress,
            address _localPortAddress,
            address _owner
        )
            BranchBridgeAgentFactory(
                _rootChainId,
                _rootChainId,
                _rootBridgeAgentFactoryAddress,
                address(0),
                _localCoreBranchRouterAddress,
                _localPortAddress,
                _owner
            )
        {}

```
[#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L30) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

/// Missing zero check for `_lzEndpointAddress`
31:     constructor(uint16 _rootChainId, address _lzEndpointAddress, address _rootPortAddress) {

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L31) 

```solidity
File: src/token/ERC20hTokenBranch.sol

/// Missing zero check for `_owner`
13:     constructor(
            string memory chainName,
            string memory chainSymbol,
            string memory _name,
            string memory _symbol,
            uint8 _decimals,
            address _owner
        ) ERC20(string(string.concat(chainName, _name)), string(string.concat(chainSymbol, _symbol)), _decimals) {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L13) 

</details>

---

<a name="L-12"></a> 
### [L-12] Missing checks for `address(0)` when setting address state variables

<details>
<summary>
There are <b>40</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

42:         rootPortAddress = _rootPortAddress;

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L42) 

```solidity
File: src/BaseBranchRouter.sol

62:         localBridgeAgentAddress = _localBridgeAgentAddress;

63:         localPortAddress = IBridgeAgent(_localBridgeAgentAddress).localPortAddress();

64:         bridgeAgentExecutorAddress = IBridgeAgent(_localBridgeAgentAddress).bridgeAgentExecutorAddress();

```
[#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L62) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L63) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L64) 

```solidity
File: src/BranchBridgeAgent.sol

135:         rootBridgeAgentAddress = _rootBridgeAgentAddress;

136:         lzEndpointAddress = _lzEndpointAddress;

137:         localRouterAddress = _localRouterAddress;

138:         localPortAddress = _localPortAddress;

139:         bridgeAgentExecutorAddress = DeployBranchBridgeAgentExecutor.deploy();

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L135) [#L136](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L136) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L137) [#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L138) [#L139](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L139) 

```solidity
File: src/BranchPort.sol

123:         require(coreBranchRouterAddress == address(0), "Contract already initialized");

```
[#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L123) 

```solidity
File: src/CoreBranchRouter.sol

31:         hTokenFactoryAddress = _hTokenFactoryAddress;

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L31) 

```solidity
File: src/CoreRootRouter.sol

73:         rootPortAddress = _rootPortAddress;

86:         bridgeAgentAddress = payable(_bridgeAgentAddress);

87:         bridgeAgentExecutorAddress = IBridgeAgent(_bridgeAgentAddress).bridgeAgentExecutorAddress();

88:         hTokenFactoryAddress = _hTokenFactory;

```
[#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L73) [#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L86) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L87) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L88) 

```solidity
File: src/MulticallRootRouter.sol

97:         localPortAddress = _localPortAddress;

98:         multicallAddress = _multicallAddress;

112:         bridgeAgentAddress = payable(_bridgeAgentAddress);

113:         bridgeAgentExecutorAddress = IBridgeAgent(_bridgeAgentAddress).bridgeAgentExecutorAddress();

```
[#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L98) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L112) [#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L113) 

```solidity
File: src/RootBridgeAgent.sol

115:         factoryAddress = msg.sender;

117:         lzEndpointAddress = _lzEndpointAddress;

118:         localPortAddress = _localPortAddress;

119:         localRouterAddress = _localRouterAddress;

120:         bridgeAgentExecutorAddress = DeployRootBridgeAgentExecutor.deploy(address(this));

```
[#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L115) [#L117](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L117) [#L118](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L118) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L119) [#L120](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L120) 

```solidity
File: src/RootPort.sol

138:         coreRootRouterAddress = _coreRootRouter;

159:         coreRootBridgeAgentAddress = _coreRootBridgeAgent;

160:         localBranchPortAddress = _localBranchPortAddress;

```
[#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L138) [#L159](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L159) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L160) 

```solidity
File: src/VirtualAccount.sol

36:         userAddress = _userAddress;

37:         localPortAddress = _localPortAddress;

```
[#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L36) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L37) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

72:         rootBridgeAgentFactoryAddress = _rootBridgeAgentFactoryAddress;

73:         lzEndpointAddress = _lzEndpointAddress;

74:         localCoreBranchRouterAddress = _localCoreBranchRouterAddress;

75:         localPortAddress = _localPortAddress;

```
[#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L72) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L73) [#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L74) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L75) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

47:         localPortAddress = _localPortAddress;

74:         localCoreRouterAddress = _coreRouter;

```
[#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L47) [#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L74) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

37:         rootPortAddress = _rootPortAddress;

51:         coreRootRouterAddress = _coreRouter;

```
[#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L37) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L51) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

35:         lzEndpointAddress = _lzEndpointAddress;

36:         rootPortAddress = _rootPortAddress;

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L35) [#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L36) 

```solidity
File: src/token/ERC20hTokenRoot.sol

43:         factoryAddress = _factoryAddress;

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L43) 

</details>

---

<a name="L-13"></a> 
### [L-13] Owner can renounce Ownership
Each of the following contracts implements or inherits the `renounceOwnership()` function. This can represent a certain risk if the ownership is renounced for any other reason than by design. Renouncing ownership will leave the contract without an owner, thereby removing any functionality that is only available to the owner.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

25: contract BaseBranchRouter is IBranchRouter, Ownable {

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L25) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

29: contract BranchBridgeAgentExecutor is Ownable, BridgeAgentConstants {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L29) 

```solidity
File: src/BranchPort.sol

17: contract BranchPort is Ownable, IBranchPort {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L17) 

```solidity
File: src/CoreRootRouter.sol

38: contract CoreRootRouter is IRootRouter, Ownable {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L38) 

```solidity
File: src/MulticallRootRouter.sol

57: contract MulticallRootRouter is IRootRouter, Ownable {

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L57) 

```solidity
File: src/RootBridgeAgentExecutor.sol

27: contract RootBridgeAgentExecutor is Ownable, BridgeAgentConstants {

```
[#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L27) 

```solidity
File: src/RootPort.sol

16: contract RootPort is Ownable, IRootPort {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L16) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

19: contract BranchBridgeAgentFactory is Ownable, IBranchBridgeAgentFactory {

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L19) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

12: contract ERC20hTokenBranchFactory is Ownable, IERC20hTokenBranchFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L12) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

12: contract ERC20hTokenRootFactory is Ownable, IERC20hTokenRootFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L12) 

```solidity
File: src/token/ERC20hTokenBranch.sol

12: contract ERC20hTokenBranch is ERC20, Ownable, IERC20hTokenBranch {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L12) 

```solidity
File: src/token/ERC20hTokenRoot.sol

12: contract ERC20hTokenRoot is ERC20, Ownable, IERC20hTokenRoot {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L12) 

</details>

---

<a name="L-14"></a> 
### [L-14] prevent re-setting a state variable with the same value
Not only is wasteful in terms of gas, but this is especially problematic when an event is emitted and the old and new values set are the same, as listeners might not expect this kind of scenario.

<details>
<summary>
There are <b>50</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

41:         localChainId = _localChainId;

42:         rootPortAddress = _rootPortAddress;

```
[#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L41) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L42) 

```solidity
File: src/BaseBranchRouter.sol

62:         localBridgeAgentAddress = _localBridgeAgentAddress;

63:         localPortAddress = IBridgeAgent(_localBridgeAgentAddress).localPortAddress();

64:         bridgeAgentExecutorAddress = IBridgeAgent(_localBridgeAgentAddress).bridgeAgentExecutorAddress();

```
[#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L62) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L63) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L64) 

```solidity
File: src/BranchBridgeAgent.sol

133:         localChainId = _localChainId;

134:         rootChainId = _rootChainId;

135:         rootBridgeAgentAddress = _rootBridgeAgentAddress;

136:         lzEndpointAddress = _lzEndpointAddress;

137:         localRouterAddress = _localRouterAddress;

138:         localPortAddress = _localPortAddress;

821:         depositNonce = _depositNonce + 1;

875:         depositNonce = _depositNonce + 1;

```
[#L133](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L133) [#L134](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L134) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L135) [#L136](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L136) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L137) [#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L138) [#L821](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L821) [#L875](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L875) 

```solidity
File: src/CoreBranchRouter.sol

31:         hTokenFactoryAddress = _hTokenFactoryAddress;

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L31) 

```solidity
File: src/CoreRootRouter.sol

72:         rootChainId = _rootChainId;

73:         rootPortAddress = _rootPortAddress;

86:         bridgeAgentAddress = payable(_bridgeAgentAddress);

87:         bridgeAgentExecutorAddress = IBridgeAgent(_bridgeAgentAddress).bridgeAgentExecutorAddress();

```
[#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L72) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L73) [#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L86) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L87) 

```solidity
File: src/MulticallRootRouter.sol

96:         localChainId = _localChainId;

97:         localPortAddress = _localPortAddress;

98:         multicallAddress = _multicallAddress;

112:         bridgeAgentAddress = payable(_bridgeAgentAddress);

113:         bridgeAgentExecutorAddress = IBridgeAgent(_bridgeAgentAddress).bridgeAgentExecutorAddress();

```
[#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L96) [#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L98) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L112) [#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L113) 

```solidity
File: src/RootBridgeAgent.sol

116:         localChainId = _localChainId;

117:         lzEndpointAddress = _lzEndpointAddress;

118:         localPortAddress = _localPortAddress;

119:         localRouterAddress = _localRouterAddress;

978:         settlementNonce = _settlementNonce + 1;

1064:         settlementNonce = _settlementNonce + 1;

```
[#L116](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L116) [#L117](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L117) [#L118](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L118) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L119) [#L978](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L978) [#L1064](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1064) 

```solidity
File: src/RootPort.sol

112:         localChainId = _localChainId;

160:         localBranchPortAddress = _localBranchPortAddress;

```
[#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L112) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L160) 

```solidity
File: src/VirtualAccount.sol

36:         userAddress = _userAddress;

37:         localPortAddress = _localPortAddress;

```
[#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L36) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L37) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

70:         localChainId = _localChainId;

71:         rootChainId = _rootChainId;

72:         rootBridgeAgentFactoryAddress = _rootBridgeAgentFactoryAddress;

73:         lzEndpointAddress = _lzEndpointAddress;

74:         localCoreBranchRouterAddress = _localCoreBranchRouterAddress;

75:         localPortAddress = _localPortAddress;

```
[#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L70) [#L71](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L71) [#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L72) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L73) [#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L74) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L75) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

44:         chainName = string.concat(_chainName, " Ulysses");

45:         chainSymbol = string.concat(_chainSymbol, "-u");

46:         localChainId = _localChainId;

47:         localPortAddress = _localPortAddress;

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L44) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L45) [#L46](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L46) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L47) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

36:         localChainId = _localChainId;

37:         rootPortAddress = _rootPortAddress;

```
[#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L36) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L37) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

34:         rootChainId = _rootChainId;

35:         lzEndpointAddress = _lzEndpointAddress;

36:         rootPortAddress = _rootPortAddress;

```
[#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L34) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L35) [#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L36) 

```solidity
File: src/token/ERC20hTokenRoot.sol

42:         localChainId = _localChainId;

43:         factoryAddress = _factoryAddress;

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L42) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L43) 

</details>

---

<a name="L-15"></a> 
### [L-15] `receive()`/`fallback()` function does not authorize requests
Having no access control on the function (e.g. `require(msg.sender == address(weth))`) means that someone may send Ether to the contract, and have no way to get anything back out, which is a loss of funds. If the concern is having to spend a small amount of gas to check the sender against an immutable address, the code should at least have a function to rescue mistakenly-sent Ether.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

149:     receive() external payable {}

```
[#L149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L149) 

```solidity
File: src/RootBridgeAgent.sol

128:     receive() external payable {}

```
[#L128](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L128) 

```solidity
File: src/VirtualAccount.sol

44:     receive() external payable {}

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L44) 

</details>

---

<a name="L-16"></a> 
### [L-16] Solidity version 0.8.20 or above may not work on other chains due to PUSH0
Solidity version 0.8.20 or above uses the new [Shanghai EVM](https://blog.soliditylang.org/2023/05/10/solidity-0.8.20-release-announcement/#important-note) which introduces the PUSH0 opcode. This op code may not yet be implemented on all evm-chains or Layer2s, so deployment on these chains will fail. Consider using an earlier solidity version.

<details>
<summary>
There are <b>41</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L2) 

```solidity
File: src/ArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L3) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L2) 

```solidity
File: src/BaseBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L2) 

```solidity
File: src/BranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L2) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L2) 

```solidity
File: src/BranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L3) 

```solidity
File: src/CoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L2) 

```solidity
File: src/CoreRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouterLibZip.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L2) 

```solidity
File: src/RootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L2) 

```solidity
File: src/RootBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L2) 

```solidity
File: src/RootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L3) 

```solidity
File: src/VirtualAccount.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L3) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L2) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L2) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/interfaces/IMulticall2.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L2) 

```solidity
File: src/interfaces/IPortStrategy.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L3) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IRootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L3) 

```solidity
File: src/interfaces/IRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L2) 

```solidity
File: src/interfaces/IVirtualAccount.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L2) 

```solidity
File: src/token/ERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L2) 

```solidity
File: src/token/ERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L2) 

</details>

---

<a name="L-17"></a> 
### [L-17] Timestamp may be manipulation
The `block.timestamp` can be manipulated by miners to perform MEV profiting or other time-based attacks.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

487:         if (block.timestamp - lastManaged[msg.sender][_token] >= 1 days) {

490:                 lastManaged[msg.sender][_token] = (block.timestamp / 1 days) * 1 days;

```
[#L487](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L487) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L490) 

</details>

---

<a name="L-18"></a> 
### [L-18] Unsafe downcast
When a type is downcast to a smaller type, the higher order bits are truncated, effectively applying a modulo to the original value. Without any other checks, this wrapping will lead to unexpected behavior and bugs.

<details>
<summary>
There are <b>17</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

243:             uint8(_dParams.hTokens.length),

320:             uint8(_dParams.hTokens.length),

359:         if (uint8(deposit.hTokens.length) == 1) {

383:         } else if (uint8(deposit.hTokens.length) > 1) {

389:                     uint8(deposit.hTokens.length),

400:                     uint8(deposit.hTokens.length),

501:         uint8 numOfAssets = uint8(bytes1(_sParams[0]));

```
[#L243](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L243) [#L320](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L320) [#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L359) [#L383](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L383) [#L389](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L389) [#L400](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L400) [#L501](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L501) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

110:         uint256 assetsOffset = uint8(bytes1(_payload[PARAMS_START_SIGNED])) * PARAMS_TKN_SET_SIZE_MULTIPLE;

```
[#L110](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L110) 

```solidity
File: src/RootBridgeAgent.sol

896:                 uint8(_hTokens.length),

1092:             uint8(hTokens.length),

```
[#L896](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L896) [#L1092](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1092) 

```solidity
File: src/RootBridgeAgentExecutor.sol

125:                     PARAMS_END_OFFSET + uint256(uint8(bytes1(_payload[PARAMS_START]))) * PARAMS_TKN_SET_SIZE_MULTIPLE

130:         uint256 numOfAssets = uint8(bytes1(_payload[PARAMS_START]));

213:                         + uint256(uint8(bytes1(_payload[PARAMS_START_SIGNED]))) * PARAMS_TKN_SET_SIZE_MULTIPLE

222:                     + uint256(uint8(bytes1(_payload[PARAMS_START_SIGNED]))) * PARAMS_TKN_SET_SIZE_MULTIPLE

228:                         + uint256(uint8(bytes1(_payload[PARAMS_START_SIGNED]))) * PARAMS_TKN_SET_SIZE_MULTIPLE:

273:         uint8 numOfAssets = uint8(bytes1(_dParams[0]));

281:         for (uint256 i = 0; i < uint256(uint8(numOfAssets));) {

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L125) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L130) [#L213](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L213) [#L222](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L222) [#L228](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L228) [#L273](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L273) [#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L281) 

</details>

---

<a name="L-19"></a> 
### [L-19] Unsafe solidity low-level call can cause gas grief attack
Using the low-level calls of a solidity address can leave the contract open to gas grief attacks. These attacks occur when the called contract returns a large amount of data. So when calling an external contract, it is necessary to check the length of the return data before reading/copying it (using `returndatasize()`).

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

103:         _rootBridgeAgentAddress.call{value: msg.value}("");

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L103) 

```solidity
File: src/BranchBridgeAgent.sol

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

```
[#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) [#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) 

```solidity
File: src/MulticallRootRouter.sol

239:             IVirtualAccount(userAccount).call(calls);

328:             IVirtualAccount(userAccount).call(calls);

416:             IVirtualAccount(userAccount).call(calls);

```
[#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L239) [#L328](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L328) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L416) 

```solidity
File: src/RootBridgeAgent.sol

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

835:             callee.call{value: msg.value}("");

927:             callee.call{value: _value}("");

```
[#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L835](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L835) [#L927](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L927) 

</details>

---

<a name="L-20"></a> 
### [L-20] Use Ownable2Step instead of Ownable
`Ownable2Step` and `Ownable2StepUpgradeable` prevent the contract ownership from mistakenly being transferred to an address that cannot handle it (e.g. due to a typo in the address), by requiring that the recipient of the owner permissions actively accept via a contract call of its own.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

25: contract BaseBranchRouter is IBranchRouter, Ownable {

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L25) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

29: contract BranchBridgeAgentExecutor is Ownable, BridgeAgentConstants {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L29) 

```solidity
File: src/BranchPort.sol

17: contract BranchPort is Ownable, IBranchPort {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L17) 

```solidity
File: src/CoreRootRouter.sol

38: contract CoreRootRouter is IRootRouter, Ownable {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L38) 

```solidity
File: src/MulticallRootRouter.sol

57: contract MulticallRootRouter is IRootRouter, Ownable {

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L57) 

```solidity
File: src/RootBridgeAgentExecutor.sol

27: contract RootBridgeAgentExecutor is Ownable, BridgeAgentConstants {

```
[#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L27) 

```solidity
File: src/RootPort.sol

16: contract RootPort is Ownable, IRootPort {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L16) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

19: contract BranchBridgeAgentFactory is Ownable, IBranchBridgeAgentFactory {

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L19) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

12: contract ERC20hTokenBranchFactory is Ownable, IERC20hTokenBranchFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L12) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

12: contract ERC20hTokenRootFactory is Ownable, IERC20hTokenRootFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L12) 

```solidity
File: src/token/ERC20hTokenBranch.sol

12: contract ERC20hTokenBranch is ERC20, Ownable, IERC20hTokenBranch {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L12) 

```solidity
File: src/token/ERC20hTokenRoot.sol

12: contract ERC20hTokenRoot is ERC20, Ownable, IERC20hTokenRoot {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L12) 

</details>

---

<a name="L-21"></a> 
### [L-21] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumCoreBranchRouter.sol

65:         IBridgeAgent(localBridgeAgentAddress).callOutSystem(payable(msg.sender), payload, GasParams(0, 0));

142:                 GasParams(0, 0)

```
[#L65](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L65) [#L142](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L142) 

```solidity
File: src/RootBridgeAgent.sol

402:                 DepositParams({

```
[#L402](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L402) 

</details>

---

<a name="L-22"></a> 
### [L-22] Missing zero address check in initializer

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/CoreRootRouter.sol

/// Missing zero check for `_bridgeAgentAddress`
/// Missing zero check for `_hTokenFactory`
83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

/// Missing zero check for `_wrappedNativeTokenAddress`
60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

</details>

---

<a name="L-23"></a> 
### [L-23] Do not use deprecated library functions

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/MulticallRootRouter.sol

521:         outputToken.safeApprove(_bridgeAgentAddress, amountOut);

559:             outputTokens[i].safeApprove(_bridgeAgentAddress, amountsOut[i]);

```
[#L521](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L521) [#L559](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L559) 

</details>

---

<a name="L-24"></a> 
### [L-24] Empty Function Body - Consider commenting why

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

57:     {}

89:     function retrySettlement(uint32, bytes calldata, GasParams[2] calldata, bool) external payable override lock {}

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L57) [#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L89) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

44:     constructor() CoreBranchRouter(address(0)) {}

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L44) 

```solidity
File: src/BranchBridgeAgent.sol

149:     receive() external payable {}

```
[#L149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L149) 

```solidity
File: src/MulticallRootRouterLibZip.sol

31:     {}

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L31) 

```solidity
File: src/RootBridgeAgent.sol

128:     receive() external payable {}

```
[#L128](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L128) 

```solidity
File: src/VirtualAccount.sol

44:     receive() external payable {}

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L44) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

46:     {}

```
[#L46](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L46) 

</details>

---

<a name="L-25"></a> 
### [L-25] Initializers could be front-run
Initializers could be front-run, allowing an attacker to either set their own values, take ownership of the contract, and in the best case forcing a re-deployment

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

60:     function initialize(address _localBridgeAgentAddress) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L60) 

```solidity
File: src/BranchPort.sol

122:     function initialize(address _coreBranchRouter, address _bridgeAgentFactory) external virtual onlyOwner {

```
[#L122](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L122) 

```solidity
File: src/CoreRootRouter.sol

83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) 

```solidity
File: src/MulticallRootRouter.sol

109:     function initialize(address _bridgeAgentAddress) external onlyOwner {

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L109) 

```solidity
File: src/RootPort.sol

129:     function initialize(address _bridgeAgentFactory, address _coreRootRouter) external onlyOwner {

```
[#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L129) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

```
[#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

87:     function initialize(address _coreRootBridgeAgent) external virtual onlyOwner {

```
[#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L87) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

49:     function initialize(address _coreRouter) external onlyOwner {

```
[#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L49) 

</details>

---

<a name="L-26"></a> 
### [L-26] `safeApprove()` is deprecated
[Deprecated](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/bfff03c0d2a59bcd8e2ead1da9aed9edf0080d05/contracts/token/ERC20/utils/SafeERC20.sol#L38-L45) in favor of `safeIncreaseAllowance()` and `safeDecreaseAllowance()`. If only setting the initial allowance to the value that means infinite, `safeIncreaseAllowance()` can be used instead. The function may currently work, but if a bug is found in this version of OpenZeppelin, and the version that you're forced to upgrade to no longer has this function, you'll encounter unnecessary delays in porting and testing replacement contracts.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/MulticallRootRouter.sol

521:         outputToken.safeApprove(_bridgeAgentAddress, amountOut);

559:             outputTokens[i].safeApprove(_bridgeAgentAddress, amountsOut[i]);

```
[#L521](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L521) [#L559](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L559) 

</details>

---

<a name="L-27"></a> 
### [L-27] Unspecific compiler version pragma

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L3) 

</details>

---


## Non Critical Issues

<a name="NC-1"></a> 
### [NC-1] Contract declarations should have NatSpec `@author` annotations

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

10: library DeployArbitrumBranchBridgeAgent {

```
[#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L10) 

```solidity
File: src/BranchBridgeAgent.sol

23: library DeployBranchBridgeAgent {

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L23) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

15: library DeployBranchBridgeAgentExecutor {

```
[#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L15) 

```solidity
File: src/RootBridgeAgentExecutor.sol

13: library DeployRootBridgeAgentExecutor {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L13) 

```solidity
File: src/VirtualAccount.sol

17: contract VirtualAccount is IVirtualAccount, ERC1155Receiver {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L17) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

7: interface ILayerZeroEndpoint is ILayerZeroUserApplicationConfig {

```
[#L7](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L7) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

5: interface ILayerZeroReceiver {

```
[#L5](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L5) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

5: interface ILayerZeroUserApplicationConfig {

```
[#L5](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L5) 

```solidity
File: src/interfaces/IRootPort.sol

10: interface ICoreRootRouter {

```
[#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L10) 

</details>

---

<a name="NC-2"></a> 
### [NC-2] Consider adding a block/deny-list
Doing so will significantly increase centralization, but will help to prevent hackers from using stolen tokens.

<details>
<summary>
There are <b>23</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

31: contract ArbitrumBranchBridgeAgent is BranchBridgeAgent {

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L31) 

```solidity
File: src/ArbitrumBranchPort.sol

14: contract ArbitrumBranchPort is BranchPort, IArbitrumBranchPort {

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L14) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

37: contract ArbitrumCoreBranchRouter is CoreBranchRouter {

```
[#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L37) 

```solidity
File: src/BaseBranchRouter.sol

25: contract BaseBranchRouter is IBranchRouter, Ownable {

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L25) 

```solidity
File: src/BranchBridgeAgent.sol

45: contract BranchBridgeAgent is IBranchBridgeAgent, BridgeAgentConstants {

```
[#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L45) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

29: contract BranchBridgeAgentExecutor is Ownable, BridgeAgentConstants {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L29) 

```solidity
File: src/BranchPort.sol

17: contract BranchPort is Ownable, IBranchPort {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L17) 

```solidity
File: src/CoreBranchRouter.sol

18: contract CoreBranchRouter is ICoreBranchRouter, BaseBranchRouter {

```
[#L18](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L18) 

```solidity
File: src/CoreRootRouter.sol

38: contract CoreRootRouter is IRootRouter, Ownable {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L38) 

```solidity
File: src/MulticallRootRouter.sol

57: contract MulticallRootRouter is IRootRouter, Ownable {

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L57) 

```solidity
File: src/MulticallRootRouterLibZip.sol

26: contract MulticallRootRouterLibZip is MulticallRootRouter {

```
[#L26](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L26) 

```solidity
File: src/RootBridgeAgent.sol

32: contract RootBridgeAgent is IRootBridgeAgent, BridgeAgentConstants {

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L32) 

```solidity
File: src/RootBridgeAgentExecutor.sol

27: contract RootBridgeAgentExecutor is Ownable, BridgeAgentConstants {

```
[#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L27) 

```solidity
File: src/RootPort.sol

16: contract RootPort is Ownable, IRootPort {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L16) 

```solidity
File: src/VirtualAccount.sol

17: contract VirtualAccount is IVirtualAccount, ERC1155Receiver {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L17) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

17: contract ArbitrumBranchBridgeAgentFactory is BranchBridgeAgentFactory {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L17) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

19: contract BranchBridgeAgentFactory is Ownable, IBranchBridgeAgentFactory {

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L19) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

12: contract ERC20hTokenBranchFactory is Ownable, IERC20hTokenBranchFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L12) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

12: contract ERC20hTokenRootFactory is Ownable, IERC20hTokenRootFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L12) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

11: contract RootBridgeAgentFactory is IRootBridgeAgentFactory {

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L11) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

10: contract BridgeAgentConstants {

```
[#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L10) 

```solidity
File: src/token/ERC20hTokenBranch.sol

12: contract ERC20hTokenBranch is ERC20, Ownable, IERC20hTokenBranch {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L12) 

```solidity
File: src/token/ERC20hTokenRoot.sol

12: contract ERC20hTokenRoot is ERC20, Ownable, IERC20hTokenRoot {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L12) 

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
There are <b>125</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

63:         if (_globalToken == address(0)) revert UnknownGlobalToken();

90:         if (_underlyingAddress == address(0)) revert UnknownUnderlyingToken();

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L39) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L63) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L90) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

127:         if (_data[0] == 0x02) {

146:         } else if (_data[0] == 0x03) {

152:         } else if (_data[0] == 0x04) {

157:         } else if (_data[0] == 0x05) {

162:         } else if (_data[0] == 0x06) {

```
[#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L127) [#L146](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L146) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L152) [#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L157) [#L162](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L162) 

```solidity
File: src/BaseBranchRouter.sol

61:         require(_localBridgeAgentAddress != address(0), "Bridge Agent address cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L61) 

```solidity
File: src/BranchBridgeAgent.sol

125:         require(_rootBridgeAgentAddress != address(0), "Root Bridge Agent Address cannot be the zero address.");

127:             _lzEndpointAddress != address(0) || _rootChainId == _localChainId,

130:         require(_localRouterAddress != address(0), "Local Router Address cannot be the zero address.");

131:         require(_localPortAddress != address(0), "Local Port Address cannot be the zero address.");

412:         if (payload.length == 0) revert DepositRetryUnavailableUseCallout();

440:         if (deposit.owner == address(0)) revert DepositRedeemUnavailable();

599:         if (flag == 0x00) {

616:         } else if (flag == 0x01) {

629:                 _payload[0] == 0x81,

638:         } else if (flag == 0x02) {

651:                 _payload[0] == 0x82,

663:         } else if (flag == 0x03) {

681:         } else if (flag == 0x04) {

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L125) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L127) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L131) [#L412](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L412) [#L440](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L440) [#L599](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L599) [#L616](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L616) [#L629](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L629) [#L638](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L638) [#L651](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L651) [#L663](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L663) [#L681](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L681) 

```solidity
File: src/BranchPort.sol

109:         require(_owner != address(0), "Owner is zero address");

123:         require(coreBranchRouterAddress == address(0), "Contract already initialized");

126:         require(_coreBranchRouter != address(0), "CoreBranchRouter is zero address");

127:         require(_bridgeAgentFactory != address(0), "BridgeAgentFactory is zero address");

332:         require(coreBranchRouterAddress != address(0), "CoreRouter address is zero");

333:         require(_newCoreRouter != address(0), "New CoreRouter address is zero");

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L109) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L123) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L126) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L127) [#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L332) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L333) 

```solidity
File: src/CoreBranchRouter.sol

88:         if (_params[0] == 0x01) {

100:         } else if (_params[0] == 0x02) {

115:         } else if (_params[0] == 0x03) {

121:         } else if (_params[0] == 0x04) {

127:         } else if (_params[0] == 0x05) {

133:         } else if (_params[0] == 0x06) {

140:         } else if (_params[0] == 0x07) {

```
[#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L88) [#L100](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L100) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L115) [#L121](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L121) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L127) [#L133](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L133) [#L140](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L140) 

```solidity
File: src/CoreRootRouter.sol

120:         if (IBridgeAgent(_rootBridgeAgent).getBranchBridgeAgent(_dstChainId) != address(0)) revert InvalidChainId();

307:         if (funcId == 0x02) {

314:         } else if (funcId == 0x03) {

320:         } else if (funcId == 0x04) {

337:         if (funcId == 0x01) {

```
[#L120](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L120) [#L307](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L307) [#L314](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L314) [#L320](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L320) [#L337](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L337) 

```solidity
File: src/MulticallRootRouter.sol

93:         require(_localPortAddress != address(0), "Local Port Address cannot be 0");

94:         require(_multicallAddress != address(0), "Multicall Address cannot be 0");

110:         require(_bridgeAgentAddress != address(0), "Bridge Agent Address cannot be 0");

142:         if (funcId == 0x01) {

150:         } else if (funcId == 0x02) {

174:         } else if (funcId == 0x03) {

234:         if (funcId == 0x01) {

242:         } else if (funcId == 0x02) {

265:         } else if (funcId == 0x03) {

323:         if (funcId == 0x01) {

331:         } else if (funcId == 0x02) {

354:         } else if (funcId == 0x03) {

411:         if (funcId == 0x01) {

419:         } else if (funcId == 0x02) {

442:         } else if (funcId == 0x03) {

```
[#L93](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L93) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L94) [#L110](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L110) [#L142](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L142) [#L150](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L150) [#L174](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L174) [#L234](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L234) [#L242](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L242) [#L265](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L265) [#L323](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L323) [#L331](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L331) [#L354](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L354) [#L411](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L411) [#L419](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L419) [#L442](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L442) 

```solidity
File: src/RootBridgeAgent.sol

111:         require(_lzEndpointAddress != address(0), "Layerzero Enpoint Address cannot be zero address");

112:         require(_localPortAddress != address(0), "Port Address cannot be zero address");

113:         require(_localRouterAddress != address(0), "Router Address cannot be zero address");

244:         if (settlementReference.owner == address(0)) revert SettlementRetryUnavailable();

282:         if (settlementOwner == address(0)) revert SettlementRetrieveUnavailable();

308:         if (settlementOwner == address(0)) revert SettlementRedeemUnavailable();

323:             if (_hToken != address(0)) {

444:         if (_payload[0] == 0x00) {

467:         } else if (_payload[0] == 0x01) {

490:         } else if (_payload[0] == 0x02) {

513:         } else if (_payload[0] == 0x03) {

539:         } else if (_payload[0] == 0x04) {

577:         } else if (_payload[0] & 0x7F == 0x05) {

600:                 _payload[0] == 0x85,

617:         } else if (_payload[0] & 0x7F == 0x06) {

640:                 _payload[0] == 0x86,

657:         } else if (_payload[0] & 0x7F == 0x07) {

670:             if (settlementReference.owner == address(0)) revert SettlementRetryUnavailable();

684:                 _payload[0] == 0x87,

699:         } else if (_payload[0] == 0x08) {

718:         } else if (_payload[0] == 0x09) {

818:         if (callee == address(0)) revert UnrecognizedBridgeAgent();

871:         if (_hTokens.length == 0) revert SettlementRetryUnavailableUseCallout();

910:         if (callee == address(0)) revert UnrecognizedBridgeAgent();

1141:         if (_amount == 0 && _deposit == 0) revert InvalidInputParams();

1141:         if (_amount == 0 && _deposit == 0) revert InvalidInputParams();

1145:         if (_localAddress == address(0)) revert UnrecognizedLocalAddress();

1146:         if (_underlyingAddress == address(0)) if (_deposit > 0) revert UnrecognizedUnderlyingAddress();

1171:         if (getBranchBridgeAgent[_branchChainId] != address(0)) revert AlreadyAddedBridgeAgent();

```
[#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L111) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L112) [#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L113) [#L244](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L244) [#L282](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L282) [#L308](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L308) [#L323](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L323) [#L444](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L444) [#L467](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L467) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L490) [#L513](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L513) [#L539](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L539) [#L577](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L577) [#L600](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L600) [#L617](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L617) [#L640](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L640) [#L657](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L657) [#L670](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L670) [#L684](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L684) [#L699](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L699) [#L718](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L718) [#L818](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L818) [#L871](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L871) [#L910](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L910) [#L1141](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1141) [#L1141](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1141) [#L1145](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1145) [#L1146](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1146) [#L1171](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1171) 

```solidity
File: src/RootPort.sol

130:         require(_bridgeAgentFactory != address(0), "Bridge Agent Factory cannot be 0 address.");

131:         require(_coreRootRouter != address(0), "Core Root Router cannot be 0 address.");

152:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0 address.");

153:         require(_coreLocalBranchBridgeAgent != address(0), "Core Local Branch Bridge Agent cannot be 0 address.");

154:         require(_localBranchPortAddress != address(0), "Local Branch Port Address cannot be 0 address.");

212:         return getLocalTokenFromGlobal[_globalAddress][_srcChainId] != address(0);

217:         return getGlobalTokenFromLocal[_localAddress][_srcChainId] != address(0);

226:         return _getLocalToken(_localAddress, _srcChainId, _dstChainId) != address(0);

231:         return getLocalTokenFromUnderlying[_underlyingToken][_srcChainId] != address(0);

245:         if (_globalAddress == address(0)) revert InvalidGlobalAddress();

246:         if (_localAddress == address(0)) revert InvalidLocalAddress();

247:         if (_underlyingAddress == address(0)) revert InvalidUnderlyingAddress();

264:         if (_localAddress == address(0)) revert InvalidLocalAddress();

352:         if (address(account) == address(0)) account = addVirtualAccount(_user);

360:         if (_user == address(0)) revert InvalidUserAddress();

398:         if (IBridgeAgent(_rootBridgeAgent).getBranchBridgeAgent(_branchChainId) != address(0)) {

488:         if (getUnderlyingTokenFromLocal[_ecoTokenGlobalAddress][localChainId] != address(0)) {

493:         if (getLocalTokenFromUnderlying[_ecoTokenGlobalAddress][localChainId] != address(0)) {

510:         if (_coreRootRouter == address(0)) revert InvalidCoreRootRouter();

511:         if (_coreRootBridgeAgent == address(0)) revert InvalidCoreRootBridgeAgent();

528:         if (_coreBranchRouter == address(0)) revert InvalidCoreBranchRouter();

529:         if (_coreBranchBridgeAgent == address(0)) revert InvalidCoreBrancBridgeAgent();

544:         if (_coreBranchRouter == address(0)) revert InvalidCoreBranchRouter();

545:         if (_coreBranchBridgeAgent == address(0)) revert InvalidCoreBrancBridgeAgent();

```
[#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L131) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L152) [#L153](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L153) [#L154](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L154) [#L212](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L212) [#L217](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L217) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L226) [#L231](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L231) [#L245](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L245) [#L246](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L246) [#L247](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L247) [#L264](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L264) [#L352](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L352) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L360) [#L398](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L398) [#L488](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L488) [#L493](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L493) [#L510](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L510) [#L511](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L511) [#L528](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L528) [#L529](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L529) [#L544](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L544) [#L545](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L545) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

57:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent Address cannot be 0");

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L57) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

61:         require(_rootBridgeAgentFactoryAddress != address(0), "Root Bridge Agent Factory Address cannot be 0");

63:             _lzEndpointAddress != address(0) || _rootChainId == _localChainId,

66:         require(_localCoreBranchRouterAddress != address(0), "Core Branch Router Address cannot be 0");

67:         require(_localPortAddress != address(0), "Port Address cannot be 0");

68:         require(_owner != address(0), "Owner cannot be 0");

88:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L61) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L63) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L66) [#L67](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L67) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L68) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L88) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

43:         require(_localPortAddress != address(0), "Port address cannot be 0");

61:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L43) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L61) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

35:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

50:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L35) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L50) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

32:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L32) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L3) 

```solidity
File: src/token/ERC20hTokenRoot.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

40:         require(_factoryAddress != address(0), "Factory Address cannot be 0");

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L39) [#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L40) 

</details>

---

<a name="NC-5"></a> 
### [NC-5] Contract uses both `require()`/`revert()` as well as custom errors
Consider using just one method in a single file.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: src/CoreRootRouter.sol

23:  *         This contract is responsible for permissionlessly adding new

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L23) 

</details>

---

<a name="NC-6"></a> 
### [NC-6] Contracts should have full test coverage
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

<a name="NC-7"></a> 
### [NC-7] Convert simple `if` statements to ternary expressions
Converting some if statements to ternaries (such as `z = (a < b) ? x : y`) can make the code more concise and easier to read.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

360:             if (_isSigned) {
                     //Pack new Data
                     payload = abi.encodePacked(
                         _hasFallbackToggled ? bytes1(0x85) : bytes1(0x05),
                         msg.sender,
                         _depositNonce,
                         deposit.hTokens[0],
                         deposit.tokens[0],
                         deposit.amounts[0],
                         deposit.deposits[0],
                         _params
                     );
                 } else {
                     payload = abi.encodePacked(

384:             if (_isSigned) {
                     //Pack new Data
                     payload = abi.encodePacked(
                         _hasFallbackToggled ? bytes1(0x86) : bytes1(0x06),
                         msg.sender,
                         uint8(deposit.hTokens.length),
                         _depositNonce,
                         deposit.hTokens,
                         deposit.tokens,
                         deposit.amounts,
                         deposit.deposits,
                         _params
                     );
                 } else {
                     payload = abi.encodePacked(

```
[#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L360) [#L384](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L384) 

</details>

---

<a name="NC-8"></a> 
### [NC-8] Events that mark critical parameter changes should contain both the old and the new value
This should especially be done if the new value is not required to be different from the old value.

<details>
<summary>
There are <b>29</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

689:             emit LogFallback(nonce);

700:         emit LogExecute(nonce);

```
[#L689](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L689) [#L700](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L700) 

```solidity
File: src/BranchPort.sol

163:         emit DebtCreated(msg.sender, _token, _amount);

184:         emit DebtRepaid(msg.sender, _token, _amount);

218:         emit DebtRepaid(_strategy, _token, amountToWithdraw);

344:         emit BridgeAgentFactoryAdded(_newBridgeAgentFactory);

351:         emit BridgeAgentFactoryToggled(_newBridgeAgentFactory);

358:         emit BridgeAgentToggled(_bridgeAgent);

371:         emit StrategyTokenAdded(_token, _minimumReservesRatio);

378:         emit StrategyTokenToggled(_token);

392:         emit PortStrategyAdded(_portStrategy, _token, _dailyManagementLimit);

399:         emit PortStrategyToggled(_portStrategy, _token);

410:         emit PortStrategyUpdated(_portStrategy, _token, _dailyManagementLimit);

423:         emit CoreBranchSet(_coreBranchRouter, _coreBranchBridgeAgent);

```
[#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L163) [#L184](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L184) [#L218](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L218) [#L344](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L344) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L351) [#L358](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L358) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L371) [#L378](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L378) [#L392](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L392) [#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L399) [#L410](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L410) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L423) 

```solidity
File: src/RootBridgeAgent.sol

726:             emit LogFallback(nonce, _srcChainId);

736:         emit LogExecute(nonce, _srcChainId);

```
[#L726](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L726) [#L736](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L736) 

```solidity
File: src/RootPort.sol

255:         emit LocalTokenAdded(_underlyingAddress, _localAddress, _globalAddress, _srcChainId);

269:         emit GlobalTokenAdded(_localAddress, _globalAddress, _srcChainId);

365:         emit VirtualAccountCreated(_user, address(newAccount));

389:         emit BridgeAgentAdded(_bridgeAgent, _manager);

406:         emit BridgeAgentSynced(_newBranchBridgeAgent, _rootBridgeAgent, _branchChainId);

417:         emit BridgeAgentToggled(_bridgeAgent);

427:         emit BridgeAgentFactoryAdded(_bridgeAgentFactory);

434:         emit BridgeAgentFactoryToggled(_bridgeAgentFactory);

479:         emit NewChainAdded(_chainId);

505:         emit EcosystemTokenAdded(_ecoTokenGlobalAddress);

517:         emit CoreRootSet(_coreRootRouter, _coreRootBridgeAgent);

535:         emit CoreBranchSet(_coreBranchRouter, _coreBranchBridgeAgent, _dstChainId);

549:         emit CoreBranchSynced(_coreBranchRouter, _coreBranchBridgeAgent, _dstChainId);

```
[#L255](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L255) [#L269](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L269) [#L365](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L365) [#L389](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L389) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L406) [#L417](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L417) [#L427](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L427) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L434) [#L479](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L479) [#L505](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L505) [#L517](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L517) [#L535](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L535) [#L549](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L549) 

</details>

---

<a name="NC-9"></a> 
### [NC-9] Custom errors has no error details
Consider adding parameters to the error to indicate which user or values caused the failure.

<details>
<summary>
There are <b>90</b> instances (click to show):
</summary>

```solidity
File: src/CoreRootRouter.sol

520:     error InvalidChainId();

522:     error UnauthorizedChainId();

524:     error UnauthorizedCallerNotManager();

526:     error TokenAlreadyAdded();

528:     error UnrecognizedGlobalToken();

530:     error UnrecognizedBridgeAgentFactory();

```
[#L520](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L520) [#L522](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L522) [#L524](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L524) [#L526](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L526) [#L528](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L528) [#L530](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L530) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

45:     error UnknownGlobalToken();

46:     error UnknownUnderlyingToken();

```
[#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L45) [#L46](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L46) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

339:     error UnknownFlag();

340:     error ExecutionFailure();

342:     error LayerZeroUnauthorizedCaller();

343:     error LayerZeroUnauthorizedEndpoint();

345:     error AlreadyExecutedTransaction();

347:     error InvalidInput();

348:     error InsufficientGas();

350:     error NotDepositOwner();

351:     error DepositRetryUnavailableUseCallout();

352:     error DepositRedeemUnavailable();

354:     error UnrecognizedRouter();

355:     error UnrecognizedBridgeAgentExecutor();

```
[#L339](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L339) [#L340](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L340) [#L342](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L342) [#L343](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L343) [#L345](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L345) [#L347](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L347) [#L348](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L348) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L350) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L351) [#L352](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L352) [#L354](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L354) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L355) 

```solidity
File: src/interfaces/IBranchPort.sol

245:     error AlreadyAddedBridgeAgent();

246:     error AlreadyAddedBridgeAgentFactory();

247:     error InvalidMinimumReservesRatio();

248:     error InvalidInputArrays();

249:     error InsufficientReserves();

250:     error UnrecognizedCore();

251:     error UnrecognizedBridgeAgent();

252:     error UnrecognizedBridgeAgentFactory();

253:     error UnrecognizedPortStrategy();

254:     error UnrecognizedStrategyToken();

255:     error NotEnoughDebtToRepay();

```
[#L245](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L245) [#L246](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L246) [#L247](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L247) [#L248](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L248) [#L249](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L249) [#L250](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L250) [#L251](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L251) [#L252](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L252) [#L253](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L253) [#L254](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L254) [#L255](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L255) 

```solidity
File: src/interfaces/IBranchRouter.sol

113:     error UnrecognizedFunctionId();

115:     error UnrecognizedBridgeAgentExecutor();

```
[#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L113) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L115) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

53:     error UnrecognizedBridgeAgent();

54:     error UnrecognizedBridgeAgentFactory();

```
[#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L53) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L54) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

32:     error UnrecognizedCoreRouter();

34:     error UnrecognizedPort();

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L32) [#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L34) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

57:     error UnrecognizedPort();

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L57) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

32:     error UnrecognizedCoreRouterOrPort();

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L32) 

```solidity
File: src/interfaces/IPortStrategy.sol

29:     error UnrecognizedPort();

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L29) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

344:     error ExecutionFailure();

345:     error GasErrorOrRepeatedTx();

346:     error AlreadyExecutedTransaction();

347:     error UnknownFlag();

349:     error NotDao();

351:     error LayerZeroUnauthorizedEndpoint();

352:     error LayerZeroUnauthorizedCaller();

354:     error AlreadyAddedBridgeAgent();

355:     error UnrecognizedExecutor();

356:     error UnrecognizedPort();

357:     error UnrecognizedBridgeAgent();

358:     error UnrecognizedLocalBridgeAgent();

359:     error UnrecognizedBridgeAgentManager();

360:     error UnrecognizedRouter();

362:     error UnrecognizedUnderlyingAddress();

363:     error UnrecognizedLocalAddress();

365:     error SettlementRetryUnavailable();

366:     error SettlementRetryUnavailableUseCallout();

367:     error SettlementRedeemUnavailable();

368:     error SettlementRetrieveUnavailable();

369:     error NotSettlementOwner();

371:     error InsufficientBalanceForSettlement();

372:     error InsufficientGasForFees();

373:     error InvalidInputParams();

374:     error InvalidInputParamsLength();

376:     error CallerIsNotPool();

377:     error AmountsAreZero();

```
[#L344](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L344) [#L345](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L345) [#L346](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L346) [#L347](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L347) [#L349](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L349) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L351) [#L352](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L352) [#L354](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L354) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L355) [#L356](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L356) [#L357](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L357) [#L358](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L358) [#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L359) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L360) [#L362](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L362) [#L363](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L363) [#L365](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L365) [#L366](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L366) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L367) [#L368](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L368) [#L369](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L369) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L371) [#L372](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L372) [#L373](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L373) [#L374](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L374) [#L376](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L376) [#L377](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L377) 

```solidity
File: src/interfaces/IRootPort.sol

399:     error InvalidGlobalAddress();

400:     error InvalidLocalAddress();

401:     error InvalidUnderlyingAddress();

403:     error InvalidUserAddress();

405:     error InvalidCoreRootRouter();

406:     error InvalidCoreRootBridgeAgent();

407:     error InvalidCoreBranchRouter();

408:     error InvalidCoreBrancBridgeAgent();

410:     error UnrecognizedBridgeAgentFactory();

411:     error UnrecognizedBridgeAgent();

413:     error UnrecognizedToken();

414:     error UnableToMint();

416:     error AlreadyAddedChain();

417:     error AlreadyAddedEcosystemToken();

419:     error AlreadyAddedBridgeAgent();

420:     error AlreadyAddedBridgeAgentFactory();

421:     error BridgeAgentNotAllowed();

422:     error UnrecognizedCoreRootRouter();

423:     error UnrecognizedLocalBranchPort();

```
[#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L399) [#L400](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L400) [#L401](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L401) [#L403](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L403) [#L405](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L405) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L406) [#L407](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L407) [#L408](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L408) [#L410](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L410) [#L411](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L411) [#L413](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L413) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L414) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L416) [#L417](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L417) [#L419](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L419) [#L420](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L420) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L421) [#L422](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L422) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L423) 

```solidity
File: src/interfaces/IRootRouter.sol

97:     error UnrecognizedFunctionId();

98:     error UnrecognizedBridgeAgentExecutor();

```
[#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L98) 

```solidity
File: src/interfaces/IVirtualAccount.sol

79:     error CallFailed();

81:     error UnauthorizedCaller();

```
[#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L79) [#L81](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L81) 

</details>

---

<a name="NC-10"></a> 
### [NC-10] Custom errors should be used rather than `revert()`/`require()`
Custom errors are available from solidity version 0.8.4. Custom errors are more easily processed in try-catch blocks, and are easier to re-use and maintain.

<details>
<summary>
There are <b>44</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L39) 

```solidity
File: src/BaseBranchRouter.sol

61:         require(_localBridgeAgentAddress != address(0), "Bridge Agent address cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L61) 

```solidity
File: src/BranchBridgeAgent.sol

125:         require(_rootBridgeAgentAddress != address(0), "Root Bridge Agent Address cannot be the zero address.");

130:         require(_localRouterAddress != address(0), "Local Router Address cannot be the zero address.");

131:         require(_localPortAddress != address(0), "Local Port Address cannot be the zero address.");

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L125) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L131) 

```solidity
File: src/BranchPort.sol

109:         require(_owner != address(0), "Owner is zero address");

123:         require(coreBranchRouterAddress == address(0), "Contract already initialized");

124:         require(!isBridgeAgentFactory[_bridgeAgentFactory], "Contract already initialized");

126:         require(_coreBranchRouter != address(0), "CoreBranchRouter is zero address");

127:         require(_bridgeAgentFactory != address(0), "BridgeAgentFactory is zero address");

136:         revert("Cannot renounce ownership");

181:         require(ERC20(_token).balanceOf(address(this)) - currBalance == _amount, "Port Strategy Withdraw Failed");

332:         require(coreBranchRouterAddress != address(0), "CoreRouter address is zero");

333:         require(_newCoreRouter != address(0), "New CoreRouter address is zero");

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L109) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L123) [#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L124) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L126) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L127) [#L136](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L136) [#L181](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L181) [#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L332) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L333) 

```solidity
File: src/CoreRootRouter.sol

84:         require(_setup, "Contract is already initialized");

278:         require(msg.sender == rootPortAddress, "Only root port can call");

```
[#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L84) [#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L278) 

```solidity
File: src/MulticallRootRouter.sol

93:         require(_localPortAddress != address(0), "Local Port Address cannot be 0");

94:         require(_multicallAddress != address(0), "Multicall Address cannot be 0");

110:         require(_bridgeAgentAddress != address(0), "Bridge Agent Address cannot be 0");

```
[#L93](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L93) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L94) [#L110](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L110) 

```solidity
File: src/RootBridgeAgent.sol

111:         require(_lzEndpointAddress != address(0), "Layerzero Enpoint Address cannot be zero address");

112:         require(_localPortAddress != address(0), "Port Address cannot be zero address");

113:         require(_localRouterAddress != address(0), "Router Address cannot be zero address");

```
[#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L111) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L112) [#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L113) 

```solidity
File: src/RootPort.sol

130:         require(_bridgeAgentFactory != address(0), "Bridge Agent Factory cannot be 0 address.");

131:         require(_coreRootRouter != address(0), "Core Root Router cannot be 0 address.");

132:         require(_setup, "Setup ended.");

152:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0 address.");

153:         require(_coreLocalBranchBridgeAgent != address(0), "Core Local Branch Bridge Agent cannot be 0 address.");

154:         require(_localBranchPortAddress != address(0), "Local Branch Port Address cannot be 0 address.");

155:         require(isBridgeAgent[_coreRootBridgeAgent], "Core Bridge Agent doesn't exist.");

156:         require(_setupCore, "Core Setup ended.");

167:         revert("Cannot renounce ownership");

```
[#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L131) [#L132](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L132) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L152) [#L153](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L153) [#L154](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L154) [#L155](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L155) [#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L156) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L167) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

57:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent Address cannot be 0");

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L57) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

61:         require(_rootBridgeAgentFactoryAddress != address(0), "Root Bridge Agent Factory Address cannot be 0");

66:         require(_localCoreBranchRouterAddress != address(0), "Core Branch Router Address cannot be 0");

67:         require(_localPortAddress != address(0), "Port Address cannot be 0");

68:         require(_owner != address(0), "Owner cannot be 0");

88:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L61) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L66) [#L67](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L67) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L68) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L88) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

43:         require(_localPortAddress != address(0), "Port address cannot be 0");

61:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L43) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L61) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

35:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

50:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L35) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L50) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

32:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L32) 

```solidity
File: src/token/ERC20hTokenRoot.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

40:         require(_factoryAddress != address(0), "Factory Address cannot be 0");

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L39) [#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L40) 

</details>

---

<a name="NC-11"></a> 
### [NC-11] Solidity version is different in some files

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

</details>

---

<a name="NC-12"></a> 
### [NC-12] Duplicated `require()`/`revert()` checks should be refactored
Refactoring duplicate `require()`/`revert()` checks into a modifier or function can make the code more concise, readable and maintainable, and less likely to make errors or omissions when modifying the `require()` or `revert()`.

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

/// Duplicated on line 135
124:         revert UnrecognizedFunctionId();

```
[#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L124) 

```solidity
File: src/CoreRootRouter.sol

/// Duplicated on line 345
327:             revert UnrecognizedFunctionId();

/// Duplicated on line 366
356:         revert();

/// Duplicated on line 381
371:         revert();

```
[#L327](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L327) [#L356](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L356) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L371) 

```solidity
File: src/MulticallRootRouter.sol

/// Duplicated on line 204
124:         revert();

/// Duplicated on line 298
198:             revert UnrecognizedFunctionId();

/// Duplicated on line 475
387:             revert UnrecognizedFunctionId();

```
[#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L124) [#L198](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L198) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L387) 

```solidity
File: src/RootBridgeAgent.sol

/// Duplicated on line 287
249:                 revert NotSettlementOwner();

/// Duplicated on line 675
313:                 revert NotSettlementOwner();

/// Duplicated on line 372
365:                 revert InvalidInputParams();

/// Duplicated on line 473
450:                 revert AlreadyExecutedTransaction();

/// Duplicated on line 519
496:                 revert AlreadyExecutedTransaction();

/// Duplicated on line 583
545:                 revert AlreadyExecutedTransaction();

/// Duplicated on line 705
623:                 revert AlreadyExecutedTransaction();

```
[#L249](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L249) [#L313](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L313) [#L365](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L365) [#L450](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L450) [#L496](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L496) [#L545](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L545) [#L623](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L623) 

```solidity
File: src/RootPort.sol

/// Duplicated on line 494
489:             revert AlreadyAddedEcosystemToken();

```
[#L489](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L489) 

</details>

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

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

681:         } else if (flag == 0x04) {
                 //Get nonce
                 nonce = uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START]));
     
                 // Reopen Deposit for redemption
                 getDeposit[nonce].status = STATUS_FAILED;
     
                 // Emit Fallback Event
                 emit LogFallback(nonce);
     
                 // Return to prevent unnecessary logic/emits
                 return;
     
                 //Unrecognized Function Selector
             } else {

```
[#L681](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L681) 

```solidity
File: src/RootBridgeAgent.sol

718:         } else if (_payload[0] == 0x09) {
                 // Parse nonce
                 nonce = uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START]));
     
                 // Reopen Settlement for redemption
                 getSettlement[nonce].status = STATUS_FAILED;
     
                 // Emit LogFallback
                 emit LogFallback(nonce, _srcChainId);
     
                 // return to prevent unnecessary emits/logic
                 return;
     
                 // Unrecognized Function Selector
             } else {

```
[#L718](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L718) 

</details>

---

<a name="NC-14"></a> 
### [NC-14] Empty bytes check is missing
Passing empty bytes to a function can cause unexpected behavior, such as certain operations failing, producing incorrect results, or wasting gas. It is recommended to check that all byte parameters are not empty.

<details>
<summary>
There are <b>110</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// Missing empty check for ``
89:     function retrySettlement(uint32, bytes calldata, GasParams[2] calldata, bool) external payable override lock {}

/// Missing empty check for `_calldata`
99:     function _performCall(address payable, bytes memory _calldata, GasParams calldata) internal override {

/// Missing empty check for ``
125:     function _requiresEndpoint(address _endpoint, bytes calldata) internal view override {

```
[#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L89) [#L99](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L99) [#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L125) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

/// Missing empty check for `_data`
126:     function executeNoSettlement(bytes calldata _data) external payable override requiresAgentExecutor {

```
[#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L126) 

```solidity
File: src/BaseBranchRouter.sol

/// Missing empty check for `_params`
83:     function callOut(bytes calldata _params, GasParams calldata _gParams) external payable override lock {

/// Missing empty check for `_params`
88:     function callOutAndBridge(bytes calldata _params, DepositInput calldata _dParams, GasParams calldata _gParams)
            external
            payable
            override
            lock
        {

/// Missing empty check for `_params`
104:     function callOutAndBridgeMultiple(
             bytes calldata _params,
             DepositMultipleInput calldata _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

/// Missing empty check for ``
123:     function executeNoSettlement(bytes calldata) external payable virtual override requiresAgentExecutor {

/// Missing empty check for ``
128:     function executeSettlement(bytes calldata, SettlementParams memory)
             external
             payable
             virtual
             override
             requiresAgentExecutor
         {

/// Missing empty check for ``
139:     function executeSettlementMultiple(bytes calldata, SettlementMultipleParams memory)
             external
             payable
             virtual
             override
             requiresAgentExecutor
         {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L83) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L88) [#L104](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L104) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L123) [#L128](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L128) [#L139](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L139) 

```solidity
File: src/BranchBridgeAgent.sol

/// Missing empty check for `_payload`
161:     function getFeeEstimate(uint256 _gasLimit, uint256 _remoteBranchExecutionGas, bytes calldata _payload)
             external
             view
             returns (uint256 _fee)
         {

/// Missing empty check for `_params`
180:     function callOutSystem(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
             requiresRouter
         {

/// Missing empty check for `_params`
195:     function callOut(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
         {

/// Missing empty check for `_params`
209:     function callOutAndBridge(
             address payable _refundee,
             bytes calldata _params,
             DepositInput memory _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

/// Missing empty check for `_params`
231:     function callOutAndBridgeMultiple(
             address payable _refundee,
             bytes calldata _params,
             DepositMultipleInput memory _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

/// Missing empty check for `_params`
262:     function callOutSigned(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
         {

/// Missing empty check for `_params`
276:     function callOutSignedAndBridge(
             address payable _refundee,
             bytes calldata _params,
             DepositInput memory _dParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing empty check for `_params`
306:     function callOutSignedAndBridgeMultiple(
             address payable _refundee,
             bytes calldata _params,
             DepositMultipleInput memory _dParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing empty check for `_params`
343:     function retryDeposit(
             bool _isSigned,
             uint32 _depositNonce,
             bytes calldata _params,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing empty check for `_params`
464:     function retrySettlement(
             uint32 _settlementNonce,
             bytes calldata _params,
             GasParams[2] calldata _gParams,
             bool _hasFallbackToggled
         ) external payable virtual override lock {

/// Missing empty check for `_sParams`
494:     function clearTokens(bytes calldata _sParams, address _recipient)
             external
             override
             requiresAgentExecutor
             returns (SettlementMultipleParams memory)
         {

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
578:     function lzReceive(uint16, bytes calldata _srcAddress, uint64, bytes calldata _payload) public override {

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
587:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload)
             public
             override
             requiresEndpoint(_endpoint, _srcAddress)
         {

/// Missing empty check for `_calldata`
712:     function _execute(uint256 _settlementNonce, bytes memory _calldata) private {

/// Missing empty check for `_calldata`
730:     function _execute(bool _hasFallbackToggled, uint32 _settlementNonce, address _refundee, bytes memory _calldata)
             private
         {

/// Missing empty check for `_payload`
765:     function _performCall(address payable _refundee, bytes memory _payload, GasParams calldata _gParams)
             internal
             virtual
         {

```
[#L161](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L161) [#L180](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L180) [#L195](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L195) [#L209](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L209) [#L231](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L231) [#L262](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L262) [#L276](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L276) [#L306](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L306) [#L343](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L343) [#L464](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L464) [#L494](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L494) [#L578](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L578) [#L587](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L587) [#L712](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L712) [#L730](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L730) [#L765](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L765) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

/// Missing empty check for `_payload`
53:     function executeNoSettlement(address _router, bytes calldata _payload) external payable onlyOwner {

/// Missing empty check for `_payload`
66:     function executeWithSettlement(address _recipient, address _router, bytes calldata _payload)
            external
            payable
            onlyOwner
        {

/// Missing empty check for `_payload`
104:     function executeWithSettlementMultiple(address _recipient, address _router, bytes calldata _payload)
             external
             payable
             onlyOwner
         {

```
[#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L53) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L66) [#L104](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L104) 

```solidity
File: src/CoreBranchRouter.sol

/// Missing empty check for `_params`
86:     function executeNoSettlement(bytes calldata _params) external payable virtual override requiresAgentExecutor {

```
[#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L86) 

```solidity
File: src/CoreRootRouter.sol

/// Missing empty check for `_encodedData`
297:     function executeResponse(bytes calldata _encodedData, uint16 _srcChainId)
             external
             payable
             override
             requiresExecutor
         {

/// Missing empty check for `_encodedData`
332:     function execute(bytes calldata _encodedData, uint16) external payable override requiresExecutor {

/// Missing empty check for ``
350:     function executeDepositSingle(bytes memory, DepositParams memory, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Missing empty check for ``
360:     function executeDepositMultiple(bytes calldata, DepositMultipleParams memory, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Missing empty check for ``
370:     function executeSigned(bytes memory, address, uint16) external payable override requiresExecutor {

/// Missing empty check for ``
375:     function executeSignedDepositSingle(bytes memory, DepositParams memory, address, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Missing empty check for ``
385:     function executeSignedDepositMultiple(bytes memory, DepositMultipleParams memory, address, uint16)
             external
             payable
             override
             requiresExecutor
         {

```
[#L297](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L297) [#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L332) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L350) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L360) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L370) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L375) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L385) 

```solidity
File: src/MulticallRootRouter.sol

/// Missing empty check for ``
123:     function executeResponse(bytes memory, uint16) external payable override {

/// Missing empty check for `encodedData`
137:     function execute(bytes calldata encodedData, uint16) external payable override lock requiresExecutor {

/// Missing empty check for ``
203:     function executeDepositSingle(bytes calldata, DepositParams calldata, uint16) external payable override {

/// Missing empty check for ``
209:     function executeDepositMultiple(bytes calldata, DepositMultipleParams calldata, uint16) external payable {

/// Missing empty check for `encodedData`
223:     function executeSigned(bytes calldata encodedData, address userAccount, uint16)
             external
             payable
             override
             lock
             requiresExecutor
         {

/// Missing empty check for `encodedData`
312:     function executeSignedDepositSingle(bytes calldata encodedData, DepositParams calldata, address userAccount, uint16)
             external
             payable
             override
             requiresExecutor
             lock
         {

/// Missing empty check for `encodedData`
401:     function executeSignedDepositMultiple(
             bytes calldata encodedData,
             DepositMultipleParams calldata,
             address userAccount,
             uint16
         ) external payable override requiresExecutor lock {

/// Missing empty check for `data`
581:     function _decode(bytes calldata data) internal pure virtual returns (bytes memory) {

```
[#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L123) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L137) [#L203](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L203) [#L209](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L209) [#L223](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L223) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L312) [#L401](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L401) [#L581](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L581) 

```solidity
File: src/MulticallRootRouterLibZip.sol

/// Missing empty check for `data`
37:     function _decode(bytes calldata data) internal pure override returns (bytes memory) {

```
[#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L37) 

```solidity
File: src/RootBridgeAgent.sol

/// Missing empty check for `_payload`
140:     function getFeeEstimate(
             uint256 _gasLimit,
             uint256 _remoteBranchExecutionGas,
             bytes calldata _payload,
             uint16 _dstChainId
         ) external view returns (uint256 _fee) {

/// Missing empty check for `_params`
160:     function callOut(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             GasParams calldata _gParams
         ) external payable override lock requiresRouter {

/// Missing empty check for `_params`
175:     function callOutAndBridge(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             SettlementInput calldata _sParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock requiresRouter {

/// Missing empty check for `_params`
202:     function callOutAndBridgeMultiple(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             SettlementMultipleInput calldata _sParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock requiresRouter {

/// Missing empty check for `_params`
233:     function retrySettlement(
             uint32 _settlementNonce,
             address _recipient,
             bytes calldata _params,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
423:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64, bytes calldata _payload) public {

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
434:     function lzReceiveNonBlocking(
             address _endpoint,
             uint16 _srcChainId,
             bytes calldata _srcAddress,
             bytes calldata _payload
         ) public override requiresEndpoint(_endpoint, _srcChainId, _srcAddress) {

/// Missing empty check for `_calldata`
749:     function _execute(uint256 _depositNonce, bytes memory _calldata, uint16 _srcChainId) private {

/// Missing empty check for `_calldata`
768:     function _execute(
             bool _hasFallbackToggled,
             uint32 _depositNonce,
             address _refundee,
             bytes memory _calldata,
             uint16 _srcChainId
         ) private {

/// Missing empty check for `_payload`
808:     function _performCall(
             uint16 _dstChainId,
             address payable _refundee,
             bytes memory _payload,
             GasParams calldata _gParams
         ) internal {

/// Missing empty check for `_params`
856:     function _performRetrySettlementCall(
             bool _hasFallbackToggled,
             address[] memory _hTokens,
             address[] memory _tokens,
             uint256[] memory _amounts,
             uint256[] memory _deposits,
             bytes memory _params,
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             GasParams memory _gParams,
             uint256 _value
         ) internal {

/// Missing empty check for `_params`
966:     function _createSettlement(
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes memory _params,
             address _globalAddress,
             uint256 _amount,
             uint256 _deposit,
             bool _hasFallbackToggled
         ) internal returns (bytes memory _payload) {

/// Missing empty check for `_params`
1045:     function _createSettlementMultiple(
              uint32 _settlementNonce,
              address payable _refundee,
              address _recipient,
              uint16 _dstChainId,
              address[] memory _globalAddresses,
              uint256[] memory _amounts,
              uint256[] memory _deposits,
              bytes memory _params,
              bool _hasFallbackToggled
          ) internal returns (bytes memory _payload) {

```
[#L140](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L140) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L160) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L175) [#L202](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L202) [#L233](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L233) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L423) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L434) [#L749](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L749) [#L768](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L768) [#L808](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L808) [#L856](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L856) [#L966](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L966) [#L1045](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1045) 

```solidity
File: src/RootBridgeAgentExecutor.sol

/// Missing empty check for `_payload`
50:     function executeSystemRequest(address _router, bytes calldata _payload, uint16 _srcChainId)
            external
            payable
            onlyOwner
        {

/// Missing empty check for `_payload`
66:     function executeNoDeposit(address _router, bytes calldata _payload, uint16 _srcChainId)
            external
            payable
            onlyOwner
        {

/// Missing empty check for `_payload`
82:     function executeWithDeposit(address _router, bytes calldata _payload, uint16 _srcChainId)
            external
            payable
            onlyOwner
        {

/// Missing empty check for `_payload`
115:     function executeWithDepositMultiple(address _router, bytes calldata _payload, uint16 _srcChainId)
             external
             payable
             onlyOwner
         {

/// Missing empty check for `_payload`
150:     function executeSignedNoDeposit(address _account, address _router, bytes calldata _payload, uint16 _srcChainId)
             external
             payable
             onlyOwner
         {

/// Missing empty check for `_payload`
167:     function executeSignedWithDeposit(address _account, address _router, bytes calldata _payload, uint16 _srcChainId)
             external
             payable
             onlyOwner
         {

/// Missing empty check for `_payload`
201:     function executeSignedWithDepositMultiple(
             address _account,
             address _router,
             bytes calldata _payload,
             uint16 _srcChainId
         ) external payable onlyOwner {

/// Missing empty check for `_dParams`
268:     function _bridgeInMultiple(address _recipient, bytes calldata _dParams, uint16 _srcChainId)
             internal
             returns (DepositMultipleParams memory dParams)
         {

```
[#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L50) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L66) [#L82](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L82) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L115) [#L150](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L150) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L167) [#L201](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L201) [#L268](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L268) 

```solidity
File: src/VirtualAccount.sol

/// Missing empty check for ``
119:     function onERC721Received(address, address, uint256, bytes calldata) external pure override returns (bytes4) {

/// Missing empty check for ``
124:     function onERC1155Received(address, address, uint256, uint256, bytes calldata)
             external
             pure
             override
             returns (bytes4)
         {

/// Missing empty check for ``
134:     function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata)
             external
             pure
             override
             returns (bytes4)
         {

```
[#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L119) [#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L124) [#L134](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L134) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

/// Missing empty check for `_payload`
120:     function getFeeEstimate(uint256 _gasLimit, uint256 _remoteBranchExecutionGas, bytes calldata _payload)

/// Missing empty check for `params`
138:     function callOutSystem(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Missing empty check for `params`
150:     function callOut(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Missing empty check for `params`
163:     function callOutAndBridge(

/// Missing empty check for `params`
179:     function callOutAndBridgeMultiple(

/// Missing empty check for `params`
194:     function callOutSigned(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Missing empty check for `params`
208:     function callOutSignedAndBridge(

/// Missing empty check for `params`
227:     function callOutSignedAndBridgeMultiple(

/// Missing empty check for `params`
248:     function retryDeposit(

/// Missing empty check for `params`
285:     function retrySettlement(

/// Missing empty check for `sParams`
312:     function clearTokens(bytes calldata sParams, address recipient)

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
326:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload) external;

```
[#L120](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L120) [#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L138) [#L150](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L150) [#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L163) [#L179](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L179) [#L194](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L194) [#L208](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L208) [#L227](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L227) [#L248](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L248) [#L285](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L285) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L312) [#L326](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L326) 

```solidity
File: src/interfaces/IBranchRouter.sol

/// Missing empty check for `params`
46:     function callOut(bytes calldata params, GasParams calldata gParams) external payable;

/// Missing empty check for `params`
56:     function callOutAndBridge(bytes calldata params, DepositInput calldata dParams, GasParams calldata gParams)

/// Missing empty check for `params`
68:     function callOutAndBridgeMultiple(

/// Missing empty check for `params`
89:     function executeNoSettlement(bytes calldata params) external payable;

/// Missing empty check for `params`
96:     function executeSettlement(bytes calldata params, SettlementParams calldata sParams) external payable;

/// Missing empty check for `params`
105:     function executeSettlementMultiple(bytes calldata params, SettlementMultipleParams calldata sParams)

```
[#L46](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L46) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L56) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L68) [#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L89) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L96) [#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L105) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

/// Missing empty check for `_destination`
/// Missing empty check for `_payload`
/// Missing empty check for `_adapterParams`
15:     function send(

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
31:     function receivePayload(

/// Missing empty check for `_srcAddress`
43:     function getInboundNonce(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (uint64);

/// Missing empty check for `_payload`
/// Missing empty check for `_adapterParam`
55:     function estimateFees(

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
70:     function retryPayload(uint16 _srcChainId, bytes calldata _srcAddress, bytes calldata _payload) external;

/// Missing empty check for `_srcAddress`
75:     function hasStoredPayload(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (bool);

```
[#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L15) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L31) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L43) [#L55](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L55) [#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L70) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L75) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
11:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64 _nonce, bytes calldata _payload) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L11) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

/// Missing empty check for `_config`
11:     function setConfig(uint16 _version, uint16 _chainId, uint256 _configType, bytes calldata _config) external;

/// Missing empty check for `_srcAddress`
24:     function forceResumeReceive(uint16 _srcChainId, bytes calldata _srcAddress) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L11) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L24) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

/// Missing empty check for `_payload`
149:     function getFeeEstimate(

/// Missing empty check for `_params`
168:     function callOut(

/// Missing empty check for `_params`
189:     function callOutAndBridge(

/// Missing empty check for `_params`
213:     function callOutAndBridgeMultiple(

/// Missing empty check for `_params`
236:     function retrySettlement(

/// Missing empty check for `_srcAddress`
/// Missing empty check for `_payload`
309:     function lzReceiveNonBlocking(

```
[#L149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L149) [#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L168) [#L189](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L189) [#L213](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L213) [#L236](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L236) [#L309](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L309) 

```solidity
File: src/interfaces/IRootRouter.sol

/// Missing empty check for `params`
25:     function executeResponse(bytes memory params, uint16 srcChainId) external payable;

/// Missing empty check for `params`
33:     function execute(bytes memory params, uint16 srcChainId) external payable;

/// Missing empty check for `params`
42:     function executeDepositSingle(bytes memory params, DepositParams memory dParams, uint16 srcChainId)

/// Missing empty check for `params`
53:     function executeDepositMultiple(bytes memory params, DepositMultipleParams memory dParams, uint16 srcChainId)

/// Missing empty check for `params`
63:     function executeSigned(bytes memory params, address userAccount, uint16 srcChainId) external payable;

/// Missing empty check for `params`
72:     function executeSignedDepositSingle(

/// Missing empty check for `params`
86:     function executeSignedDepositMultiple(

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L25) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L33) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L42) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L53) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L63) [#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L72) [#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L86) 

</details>

---

<a name="NC-15"></a> 
### [NC-15] Enable IR-based code generation
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

<a name="NC-16"></a> 
### [NC-16] Events are emitted without the sender information
When an action is triggered based on a user's action, not being able to filter based on who triggered the action makes event processing a lot more cumbersome. Including the `msg.sender` the events of these types of action will make events much more useful to end users, especially when `msg.sender` is not `tx.origin`.

<details>
<summary>
There are <b>25</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

700:         emit LogExecute(nonce);

```
[#L700](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L700) 

```solidity
File: src/BranchPort.sol

218:         emit DebtRepaid(_strategy, _token, amountToWithdraw);

344:         emit BridgeAgentFactoryAdded(_newBridgeAgentFactory);

351:         emit BridgeAgentFactoryToggled(_newBridgeAgentFactory);

358:         emit BridgeAgentToggled(_bridgeAgent);

371:         emit StrategyTokenAdded(_token, _minimumReservesRatio);

378:         emit StrategyTokenToggled(_token);

392:         emit PortStrategyAdded(_portStrategy, _token, _dailyManagementLimit);

399:         emit PortStrategyToggled(_portStrategy, _token);

410:         emit PortStrategyUpdated(_portStrategy, _token, _dailyManagementLimit);

423:         emit CoreBranchSet(_coreBranchRouter, _coreBranchBridgeAgent);

```
[#L218](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L218) [#L344](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L344) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L351) [#L358](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L358) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L371) [#L378](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L378) [#L392](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L392) [#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L399) [#L410](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L410) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L423) 

```solidity
File: src/RootBridgeAgent.sol

736:         emit LogExecute(nonce, _srcChainId);

```
[#L736](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L736) 

```solidity
File: src/RootPort.sol

255:         emit LocalTokenAdded(_underlyingAddress, _localAddress, _globalAddress, _srcChainId);

269:         emit GlobalTokenAdded(_localAddress, _globalAddress, _srcChainId);

365:         emit VirtualAccountCreated(_user, address(newAccount));

389:         emit BridgeAgentAdded(_bridgeAgent, _manager);

406:         emit BridgeAgentSynced(_newBranchBridgeAgent, _rootBridgeAgent, _branchChainId);

417:         emit BridgeAgentToggled(_bridgeAgent);

427:         emit BridgeAgentFactoryAdded(_bridgeAgentFactory);

434:         emit BridgeAgentFactoryToggled(_bridgeAgentFactory);

479:         emit NewChainAdded(_chainId);

505:         emit EcosystemTokenAdded(_ecoTokenGlobalAddress);

517:         emit CoreRootSet(_coreRootRouter, _coreRootBridgeAgent);

535:         emit CoreBranchSet(_coreBranchRouter, _coreBranchBridgeAgent, _dstChainId);

549:         emit CoreBranchSynced(_coreBranchRouter, _coreBranchBridgeAgent, _dstChainId);

```
[#L255](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L255) [#L269](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L269) [#L365](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L365) [#L389](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L389) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L406) [#L417](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L417) [#L427](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L427) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L434) [#L479](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L479) [#L505](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L505) [#L517](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L517) [#L535](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L535) [#L549](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L549) 

</details>

---

<a name="NC-17"></a> 
### [NC-17] Functions with array parameters should have length checks in place

<details>
<summary>
There are <b>18</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// @audit ``
89:     function retrySettlement(uint32, bytes calldata, GasParams[2] calldata, bool) external payable override lock {}

```
[#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L89) 

```solidity
File: src/BaseBranchRouter.sol

/// @audit `_tokens`
/// @audit `_amounts`
/// @audit `_deposits`
186:     function _transferAndApproveMultipleTokens(
             address[] memory _hTokens,
             address[] memory _tokens,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) internal {

```
[#L186](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L186) 

```solidity
File: src/BranchBridgeAgent.sol

/// @audit `_gParams`
464:     function retrySettlement(
             uint32 _settlementNonce,
             bytes calldata _params,
             GasParams[2] calldata _gParams,
             bool _hasFallbackToggled
         ) external payable virtual override lock {

```
[#L464](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L464) 

```solidity
File: src/BranchPort.sol

/// @audit `_underlyingAddresses`
/// @audit `_amounts`
/// @audit `_deposits`
246:     function bridgeInMultiple(
             address _recipient,
             address[] memory _localAddresses,
             address[] memory _underlyingAddresses,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) external override requiresBridgeAgent {

```
[#L246](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L246) 

```solidity
File: src/CoreBranchRouter.sol

/// @audit `_gParams`
43:     function addGlobalToken(address _globalAddress, uint256 _dstChainId, GasParams[3] calldata _gParams)
            external
            payable
        {

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L43) 

```solidity
File: src/CoreRootRouter.sol

/// @audit `_gParams`
103:     function addBranchToBridgeAgent(
             address _rootBridgeAgent,
             address _branchBridgeAgentFactory,
             address _newBranchRouter,
             address _refundee,
             uint16 _dstChainId,
             GasParams[2] calldata _gParams
         ) external payable {

/// @audit `_gParams`
406:     function _addGlobalToken(
             address _refundee,
             address _globalAddress,
             uint16 _dstChainId,
             GasParams[2] memory _gParams
         ) internal {

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L103) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L406) 

```solidity
File: src/MulticallRootRouter.sol

/// @audit `calls`
488:     function _multicall(IMulticall.Call[] memory calls)
             internal
             returns (uint256 blockNumber, bytes[] memory returnData)
         {

/// @audit `amountsOut`
/// @audit `depositsOut`
544:     function _approveMultipleAndCallOut(
             address refundee,
             address recipient,
             address[] memory outputTokens,
             uint256[] memory amountsOut,
             uint256[] memory depositsOut,
             uint16 dstChainId,
             GasParams memory gasParams
         ) internal virtual {

```
[#L488](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L488) [#L544](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L544) 

```solidity
File: src/RootBridgeAgent.sol

/// @audit `_tokens`
/// @audit `_amounts`
/// @audit `_deposits`
856:     function _performRetrySettlementCall(
             bool _hasFallbackToggled,
             address[] memory _hTokens,
             address[] memory _tokens,
             uint256[] memory _amounts,
             uint256[] memory _deposits,
             bytes memory _params,
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             GasParams memory _gParams,
             uint256 _value
         ) internal {

```
[#L856](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L856) 

```solidity
File: src/VirtualAccount.sol

/// @audit ``
/// @audit ``
134:     function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata)
             external
             pure
             override
             returns (bytes4)
         {

```
[#L134](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L134) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

/// @audit `gasParams`
285:     function retrySettlement(

```
[#L285](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L285) 

```solidity
File: src/interfaces/IBranchPort.sol

/// @audit `_localAddresses`
/// @audit `_underlyingAddresses`
/// @audit `_amounts`
/// @audit `_deposits`
103:     function bridgeInMultiple(

/// @audit `_localAddresses`
/// @audit `_underlyingAddresses`
/// @audit `_amounts`
/// @audit `_deposits`
135:     function bridgeOutMultiple(

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L103) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L135) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

/// @audit `_gasParams`
38:     function addGlobalToken(address _globalAddress, uint256 _dstChainId, GasParams[3] calldata _gasParams)

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L38) 

```solidity
File: src/interfaces/IMulticall2.sol

/// @audit `calls`
20:     function aggregate(Call[] memory calls) external returns (uint256 blockNumber, bytes[] memory returnData);

```
[#L20](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L20) 

```solidity
File: src/interfaces/IVirtualAccount.sol

/// @audit `callInput`
65:     function call(Call[] calldata callInput) external returns (bytes[] memory);

/// @audit `calls`
73:     function payableCall(PayableCall[] calldata calls) external payable returns (bytes[] memory);

```
[#L65](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L65) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L73) 

</details>

---

<a name="NC-18"></a> 
### [NC-18] Import declarations should import specific identifiers, rather than the whole file
Using import declarations of the form `import {<identifier_name>} from "some/file.sol"` avoids polluting the symbol namespace making flattened files smaller, and speeds up compilation (but does not save any gas).

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

5: import "./ILayerZeroUserApplicationConfig.sol";

```
[#L5](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L5) 

</details>

---

<a name="NC-19"></a> 
### [NC-19] Large or complicated code bases should implement invariant tests
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

<a name="NC-20"></a> 
### [NC-20] Missing zero address check in functions with address parameters
Adding a zero address check for each address type parameter can prevent errors.

<details>
<summary>
There are <b>264</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// Missing zero check for `_daoAddress`
/// Missing zero check for `_localRouterAddress`
/// Missing zero check for `_localPortAddress`
11:     function deploy(uint16 _localChainId, address _daoAddress, address _localRouterAddress, address _localPortAddress)
            external
            returns (ArbitrumBranchBridgeAgent)
        {

/// Missing zero check for `_rootBridgeAgentAddress`
/// Missing zero check for `_localRouterAddress`
/// Missing zero check for `_localPortAddress`
43:     constructor(
            uint16 _localChainId,
            address _rootBridgeAgentAddress,
            address _localRouterAddress,
            address _localPortAddress
        )
            BranchBridgeAgent(
                _localChainId,
                _localChainId,
                _rootBridgeAgentAddress,
                address(0),
                _localRouterAddress,
                _localPortAddress
            )
        {}

/// Missing zero check for `underlyingAddress`
69:     function depositToPort(address underlyingAddress, uint256 amount) external payable lock {

/// Missing zero check for `localAddress`
79:     function withdrawFromPort(address localAddress, uint256 amount) external payable lock {

/// Missing zero check for ``
99:     function _performCall(address payable, bytes memory _calldata, GasParams calldata) internal override {

/// Missing zero check for ``
112:     function _performFallbackCall(address payable, uint32 _settlementNonce) internal override {

/// Missing zero check for `_endpoint`
125:     function _requiresEndpoint(address _endpoint, bytes calldata) internal view override {

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L11) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L43) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L69) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L79) [#L99](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L99) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L112) [#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L125) 

```solidity
File: src/ArbitrumBranchPort.sol

/// Missing zero check for `_rootPortAddress`
/// Missing zero check for `_owner`
38:     constructor(uint16 _localChainId, address _rootPortAddress, address _owner) BranchPort(_owner) {

/// Missing zero check for `_depositor`
/// Missing zero check for `_recipient`
/// Missing zero check for `_underlyingAddress`
50:     function depositToPort(address _depositor, address _recipient, address _underlyingAddress, uint256 _deposit)
            external
            override
            lock
            requiresBridgeAgent
        {

/// Missing zero check for `_depositor`
/// Missing zero check for `_recipient`
/// Missing zero check for `_globalAddress`
73:     function withdrawFromPort(address _depositor, address _recipient, address _globalAddress, uint256 _amount)
            external
            override
            lock
            requiresBridgeAgent
        {

/// Missing zero check for `_recipient`
/// Missing zero check for `_localAddress`
107:     function _bridgeIn(address _recipient, address _localAddress, uint256 _amount) internal override {

/// Missing zero check for `_depositor`
/// Missing zero check for `_localAddress`
/// Missing zero check for `_underlyingAddress`
119:     function _bridgeOut(
             address _depositor,
             address _localAddress,
             address _underlyingAddress,
             uint256 _amount,
             uint256 _deposit
         ) internal override {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L38) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L50) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L73) [#L107](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L107) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L119) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

/// Missing zero check for `_underlyingAddress`
51:     function addLocalToken(address _underlyingAddress, GasParams calldata) external payable override {

/// Missing zero check for `_newBranchRouter`
/// Missing zero check for `_branchBridgeAgentFactory`
/// Missing zero check for `_rootBridgeAgent`
/// Missing zero check for `_rootBridgeAgentFactory`
/// Missing zero check for `_refundee`
85:     function _receiveAddBridgeAgent(
            address _newBranchRouter,
            address _branchBridgeAgentFactory,
            address _rootBridgeAgent,
            address _rootBridgeAgentFactory,
            address _refundee,
            GasParams memory _gParams
        ) internal override {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L51) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L85) 

```solidity
File: src/BaseBranchRouter.sol

/// Missing zero check for `_hToken`
/// Missing zero check for `_token`
160:     function _transferAndApproveToken(address _hToken, address _token, uint256 _amount, uint256 _deposit) internal {

```
[#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L160) 

```solidity
File: src/BranchBridgeAgent.sol

/// Missing zero check for `_refundee`
180:     function callOutSystem(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
             requiresRouter
         {

/// Missing zero check for `_refundee`
195:     function callOut(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
         {

/// Missing zero check for `_refundee`
209:     function callOutAndBridge(
             address payable _refundee,
             bytes calldata _params,
             DepositInput memory _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

/// Missing zero check for `_refundee`
231:     function callOutAndBridgeMultiple(
             address payable _refundee,
             bytes calldata _params,
             DepositMultipleInput memory _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

/// Missing zero check for `_refundee`
262:     function callOutSigned(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
         {

/// Missing zero check for `_refundee`
276:     function callOutSignedAndBridge(
             address payable _refundee,
             bytes calldata _params,
             DepositInput memory _dParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing zero check for `_refundee`
306:     function callOutSignedAndBridgeMultiple(
             address payable _refundee,
             bytes calldata _params,
             DepositMultipleInput memory _dParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing zero check for `_recipient`
/// Missing zero check for `_hToken`
/// Missing zero check for `_token`
485:     function clearToken(address _recipient, address _hToken, address _token, uint256 _amount, uint256 _deposit)
             external
             override
             requiresAgentExecutor
         {

/// Missing zero check for `_recipient`
494:     function clearTokens(bytes calldata _sParams, address _recipient)
             external
             override
             requiresAgentExecutor
             returns (SettlementMultipleParams memory)
         {

/// Missing zero check for `_endpoint`
587:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload)
             public
             override
             requiresEndpoint(_endpoint, _srcAddress)
         {

/// Missing zero check for `_refundee`
730:     function _execute(bool _hasFallbackToggled, uint32 _settlementNonce, address _refundee, bytes memory _calldata)
             private
         {

/// Missing zero check for `_refundee`
765:     function _performCall(address payable _refundee, bytes memory _payload, GasParams calldata _gParams)
             internal
             virtual
         {

/// Missing zero check for `_refundee`
785:     function _performFallbackCall(address payable _refundee, uint32 _settlementNonce) internal virtual {

/// Missing zero check for `_refundee`
/// Missing zero check for `_hToken`
/// Missing zero check for `_token`
812:     function _createDeposit(
             uint32 _depositNonce,
             address payable _refundee,
             address _hToken,
             address _token,
             uint256 _amount,
             uint256 _deposit
         ) internal {

/// Missing zero check for `_refundee`
860:     function _createDepositMultiple(
             uint32 _depositNonce,
             address payable _refundee,
             address[] memory _hTokens,
             address[] memory _tokens,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) internal {

/// Missing zero check for `_recipient`
/// Missing zero check for `_hToken`
/// Missing zero check for `_token`
903:     function _clearToken(address _recipient, address _hToken, address _token, uint256 _amount, uint256 _deposit)
             internal
         {

/// Missing zero check for `_endpoint`
936:     function _requiresEndpoint(address _endpoint, bytes calldata _srcAddress) internal view virtual {

```
[#L180](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L180) [#L195](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L195) [#L209](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L209) [#L231](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L231) [#L262](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L262) [#L276](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L276) [#L306](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L306) [#L485](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L485) [#L494](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L494) [#L587](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L587) [#L730](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L730) [#L765](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L765) [#L785](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L785) [#L812](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L812) [#L860](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L860) [#L903](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L903) [#L936](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L936) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

/// Missing zero check for `_router`
53:     function executeNoSettlement(address _router, bytes calldata _payload) external payable onlyOwner {

/// Missing zero check for `_recipient`
/// Missing zero check for `_router`
66:     function executeWithSettlement(address _recipient, address _router, bytes calldata _payload)
            external
            payable
            onlyOwner
        {

/// Missing zero check for `_recipient`
/// Missing zero check for `_router`
104:     function executeWithSettlementMultiple(address _recipient, address _router, bytes calldata _payload)
             external
             payable
             onlyOwner
         {

```
[#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L53) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L66) [#L104](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L104) 

```solidity
File: src/BranchPort.sol

/// Missing zero check for `_owner`
108:     constructor(address _owner) {

/// Missing zero check for `_token`
144:     function manage(address _token, uint256 _amount) external override requiresPortStrategy(_token) {

/// Missing zero check for `_token`
167:     function replenishReserves(address _token, uint256 _amount) external override lock {

/// Missing zero check for `_strategy`
/// Missing zero check for `_token`
188:     function replenishReserves(address _strategy, address _token) external override lock {

/// Missing zero check for `_recipient`
/// Missing zero check for `_underlyingAddress`
226:     function withdraw(address _recipient, address _underlyingAddress, uint256 _deposit)
             public
             virtual
             override
             lock
             requiresBridgeAgent
         {

/// Missing zero check for `_recipient`
/// Missing zero check for `_localAddress`
237:     function bridgeIn(address _recipient, address _localAddress, uint256 _amount)
             external
             override
             requiresBridgeAgent
         {

/// Missing zero check for `_recipient`
246:     function bridgeInMultiple(
             address _recipient,
             address[] memory _localAddresses,
             address[] memory _underlyingAddresses,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) external override requiresBridgeAgent {

/// Missing zero check for `_depositor`
/// Missing zero check for `_localAddress`
/// Missing zero check for `_underlyingAddress`
277:     function bridgeOut(
             address _depositor,
             address _localAddress,
             address _underlyingAddress,
             uint256 _amount,
             uint256 _deposit
         ) external override lock requiresBridgeAgent {

/// Missing zero check for `_depositor`
288:     function bridgeOutMultiple(
             address _depositor,
             address[] memory _localAddresses,
             address[] memory _underlyingAddresses,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) external override lock requiresBridgeAgent {

/// Missing zero check for `_bridgeAgent`
319:     function addBridgeAgent(address _bridgeAgent) external override requiresBridgeAgentFactory {

/// Missing zero check for `_newBridgeAgentFactory`
338:     function addBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

/// Missing zero check for `_newBridgeAgentFactory`
348:     function toggleBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

/// Missing zero check for `_bridgeAgent`
355:     function toggleBridgeAgent(address _bridgeAgent) external override requiresCoreRouter {

/// Missing zero check for `_token`
362:     function addStrategyToken(address _token, uint256 _minimumReservesRatio) external override requiresCoreRouter {

/// Missing zero check for `_token`
375:     function toggleStrategyToken(address _token) external override requiresCoreRouter {

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_token`
382:     function addPortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit)
             external
             override
             requiresCoreRouter
         {

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_token`
396:     function togglePortStrategy(address _portStrategy, address _token) external override requiresCoreRouter {

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_token`
403:     function updatePortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit)
             external
             override
             requiresCoreRouter
         {

/// Missing zero check for `_coreBranchRouter`
/// Missing zero check for `_coreBranchBridgeAgent`
414:     function setCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent)
             external
             override
             requiresCoreRouter
         {

/// Missing zero check for `_token`
435:     function _excessReserves(uint256 _strategyTokenDebt, address _token) internal view returns (uint256) {

/// Missing zero check for `_token`
449:     function _reservesLacking(uint256 _strategyTokenDebt, address _token, uint256 currBalance)
             internal
             view
             returns (uint256)
         {

/// Missing zero check for `_token`
468:     function _minimumReserves(uint256 _strategyTokenDebt, uint256 _currBalance, address _token)
             internal
             view
             returns (uint256)
         {

/// Missing zero check for `_token`
485:     function _checkTimeLimit(address _token, uint256 _amount) internal {

/// Missing zero check for `_recipient`
/// Missing zero check for `_localAddress`
502:     function _bridgeIn(address _recipient, address _localAddress, uint256 _amount) internal virtual {

/// Missing zero check for `_depositor`
/// Missing zero check for `_localAddress`
/// Missing zero check for `_underlyingAddress`
514:     function _bridgeOut(
             address _depositor,
             address _localAddress,
             address _underlyingAddress,
             uint256 _amount,
             uint256 _deposit
         ) internal virtual {

```
[#L108](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L108) [#L144](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L144) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L167) [#L188](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L188) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L226) [#L237](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L237) [#L246](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L246) [#L277](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L277) [#L288](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L288) [#L319](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L319) [#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L338) [#L348](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L348) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L355) [#L362](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L362) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L375) [#L382](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L382) [#L396](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L396) [#L403](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L403) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L414) [#L435](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L435) [#L449](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L449) [#L468](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L468) [#L485](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L485) [#L502](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L502) [#L514](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L514) 

```solidity
File: src/CoreBranchRouter.sol

/// Missing zero check for `_hTokenFactoryAddress`
30:     constructor(address _hTokenFactoryAddress) BaseBranchRouter() {

/// Missing zero check for `_globalAddress`
43:     function addGlobalToken(address _globalAddress, uint256 _dstChainId, GasParams[3] calldata _gParams)
            external
            payable
        {

/// Missing zero check for `_underlyingAddress`
62:     function addLocalToken(address _underlyingAddress, GasParams calldata _gParams) external payable virtual {

/// Missing zero check for `_globalAddress`
/// Missing zero check for `_refundee`
166:     function _receiveAddGlobalToken(
             address _globalAddress,
             string memory _name,
             string memory _symbol,
             uint8 _decimals,
             address _refundee,
             GasParams memory _gParams
         ) internal {

/// Missing zero check for `_newBranchRouter`
/// Missing zero check for `_branchBridgeAgentFactory`
/// Missing zero check for `_rootBridgeAgent`
/// Missing zero check for `_rootBridgeAgentFactory`
/// Missing zero check for `_refundee`
199:     function _receiveAddBridgeAgent(
             address _newBranchRouter,
             address _branchBridgeAgentFactory,
             address _rootBridgeAgent,
             address _rootBridgeAgentFactory,
             address _refundee,
             GasParams memory _gParams
         ) internal virtual {

/// Missing zero check for `_newBridgeAgentFactoryAddress`
244:     function _toggleBranchBridgeAgentFactory(address _newBridgeAgentFactoryAddress) internal {

/// Missing zero check for `_branchBridgeAgent`
263:     function _removeBranchBridgeAgent(address _branchBridgeAgent) internal {

/// Missing zero check for `_underlyingToken`
284:     function _manageStrategyToken(address _underlyingToken, uint256 _minimumReservesRatio) internal {

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_underlyingToken`
307:     function _managePortStrategy(
             address _portStrategy,
             address _underlyingToken,
             uint256 _dailyManagementLimit,
             bool _isUpdateDailyLimit
         ) internal {

```
[#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L30) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L43) [#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L62) [#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L166) [#L199](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L199) [#L244](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L244) [#L263](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L263) [#L284](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L284) [#L307](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L307) 

```solidity
File: src/CoreRootRouter.sol

/// Missing zero check for `_rootPortAddress`
71:     constructor(uint256 _rootChainId, address _rootPortAddress) {

/// Missing zero check for `_bridgeAgentAddress`
/// Missing zero check for `_hTokenFactory`
83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

/// Missing zero check for `_rootBridgeAgent`
/// Missing zero check for `_branchBridgeAgentFactory`
/// Missing zero check for `_newBranchRouter`
/// Missing zero check for `_refundee`
103:     function addBranchToBridgeAgent(
             address _rootBridgeAgent,
             address _branchBridgeAgentFactory,
             address _newBranchRouter,
             address _refundee,
             uint16 _dstChainId,
             GasParams[2] calldata _gParams
         ) external payable {

/// Missing zero check for `_rootBridgeAgentFactory`
/// Missing zero check for `_branchBridgeAgentFactory`
/// Missing zero check for `_refundee`
156:     function toggleBranchBridgeAgentFactory(
             address _rootBridgeAgentFactory,
             address _branchBridgeAgentFactory,
             address _refundee,
             uint16 _dstChainId,
             GasParams calldata _gParams
         ) external payable onlyOwner {

/// Missing zero check for `_branchBridgeAgent`
/// Missing zero check for `_refundee`
186:     function removeBranchBridgeAgent(
             address _branchBridgeAgent,
             address _refundee,
             uint16 _dstChainId,
             GasParams calldata _gParams
         ) external payable onlyOwner {

/// Missing zero check for `_underlyingToken`
/// Missing zero check for `_refundee`
212:     function manageStrategyToken(
             address _underlyingToken,
             uint256 _minimumReservesRatio,
             address _refundee,
             uint16 _dstChainId,
             GasParams calldata _gParams
         ) external payable onlyOwner {

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_underlyingToken`
/// Missing zero check for `_refundee`
241:     function managePortStrategy(
             address _portStrategy,
             address _underlyingToken,
             uint256 _dailyManagementLimit,
             bool _isUpdateDailyLimit,
             address _refundee,
             uint16 _dstChainId,
             GasParams calldata _gParams
         ) external payable onlyOwner {

/// Missing zero check for `_refundee`
/// Missing zero check for `_coreBranchRouter`
/// Missing zero check for `_coreBranchBridgeAgent`
270:     function setCoreBranch(
             address _refundee,
             address _coreBranchRouter,
             address _coreBranchBridgeAgent,
             uint16 _dstChainId,
             GasParams calldata _gParams
         ) external payable {

/// Missing zero check for ``
370:     function executeSigned(bytes memory, address, uint16) external payable override requiresExecutor {

/// Missing zero check for ``
375:     function executeSignedDepositSingle(bytes memory, DepositParams memory, address, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Missing zero check for ``
385:     function executeSignedDepositMultiple(bytes memory, DepositMultipleParams memory, address, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Missing zero check for `_refundee`
/// Missing zero check for `_globalAddress`
406:     function _addGlobalToken(
             address _refundee,
             address _globalAddress,
             uint16 _dstChainId,
             GasParams[2] memory _gParams
         ) internal {

/// Missing zero check for `_underlyingAddress`
/// Missing zero check for `_localAddress`
452:     function _addLocalToken(
             address _underlyingAddress,
             address _localAddress,
             string memory _name,
             string memory _symbol,
             uint8 _decimals,
             uint16 _srcChainId
         ) internal {

/// Missing zero check for `_globalAddress`
/// Missing zero check for `_localAddress`
481:     function _setLocalToken(address _globalAddress, address _localAddress, uint16 _dstChainId) internal {

/// Missing zero check for `_newBranchBridgeAgent`
/// Missing zero check for `_rootBridgeAgent`
500:     function _syncBranchBridgeAgent(address _newBranchBridgeAgent, address _rootBridgeAgent, uint256 _srcChainId)
             internal
         {

```
[#L71](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L71) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) [#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L103) [#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L156) [#L186](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L186) [#L212](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L212) [#L241](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L241) [#L270](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L270) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L370) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L375) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L385) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L406) [#L452](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L452) [#L481](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L481) [#L500](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L500) 

```solidity
File: src/MulticallRootRouter.sol

/// Missing zero check for `_localPortAddress`
/// Missing zero check for `_multicallAddress`
92:     constructor(uint256 _localChainId, address _localPortAddress, address _multicallAddress) {

/// Missing zero check for `userAccount`
223:     function executeSigned(bytes calldata encodedData, address userAccount, uint16)
             external
             payable
             override
             lock
             requiresExecutor
         {

/// Missing zero check for `userAccount`
312:     function executeSignedDepositSingle(bytes calldata encodedData, DepositParams calldata, address userAccount, uint16)
             external
             payable
             override
             requiresExecutor
             lock
         {

/// Missing zero check for `userAccount`
401:     function executeSignedDepositMultiple(
             bytes calldata encodedData,
             DepositMultipleParams calldata,
             address userAccount,
             uint16
         ) external payable override requiresExecutor lock {

/// Missing zero check for `refundee`
/// Missing zero check for `recipient`
/// Missing zero check for `outputToken`
508:     function _approveAndCallOut(
             address refundee,
             address recipient,
             address outputToken,
             uint256 amountOut,
             uint256 depositOut,
             uint16 dstChainId,
             GasParams memory gasParams
         ) internal virtual {

/// Missing zero check for `refundee`
/// Missing zero check for `recipient`
544:     function _approveMultipleAndCallOut(
             address refundee,
             address recipient,
             address[] memory outputTokens,
             uint256[] memory amountsOut,
             uint256[] memory depositsOut,
             uint16 dstChainId,
             GasParams memory gasParams
         ) internal virtual {

```
[#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L92) [#L223](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L223) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L312) [#L401](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L401) [#L508](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L508) [#L544](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L544) 

```solidity
File: src/MulticallRootRouterLibZip.sol

/// Missing zero check for `_localPortAddress`
/// Missing zero check for `_multicallAddress`
29:     constructor(uint256 _localChainId, address _localPortAddress, address _multicallAddress)
            MulticallRootRouter(_localChainId, _localPortAddress, _multicallAddress)
        {}

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L29) 

```solidity
File: src/RootBridgeAgent.sol

/// Missing zero check for `_lzEndpointAddress`
/// Missing zero check for `_localPortAddress`
/// Missing zero check for `_localRouterAddress`
105:     constructor(
             uint16 _localChainId,
             address _lzEndpointAddress,
             address _localPortAddress,
             address _localRouterAddress
         ) {

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
160:     function callOut(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             GasParams calldata _gParams
         ) external payable override lock requiresRouter {

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
175:     function callOutAndBridge(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             SettlementInput calldata _sParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock requiresRouter {

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
202:     function callOutAndBridgeMultiple(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             SettlementMultipleInput calldata _sParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock requiresRouter {

/// Missing zero check for `_recipient`
233:     function retrySettlement(
             uint32 _settlementNonce,
             address _recipient,
             bytes calldata _params,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing zero check for `_recipient`
351:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId)
             public
             override
             requiresAgentExecutor
         {

/// Missing zero check for `_recipient`
387:     function bridgeInMultiple(address _recipient, DepositMultipleParams calldata _dParams, uint256 _srcChainId)
             external
             override
             requiresAgentExecutor
         {

/// Missing zero check for `_endpoint`
434:     function lzReceiveNonBlocking(
             address _endpoint,
             uint16 _srcChainId,
             bytes calldata _srcAddress,
             bytes calldata _payload
         ) public override requiresEndpoint(_endpoint, _srcChainId, _srcAddress) {

/// Missing zero check for `_refundee`
768:     function _execute(
             bool _hasFallbackToggled,
             uint32 _depositNonce,
             address _refundee,
             bytes memory _calldata,
             uint16 _srcChainId
         ) private {

/// Missing zero check for `_refundee`
808:     function _performCall(
             uint16 _dstChainId,
             address payable _refundee,
             bytes memory _payload,
             GasParams calldata _gParams
         ) internal {

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
856:     function _performRetrySettlementCall(
             bool _hasFallbackToggled,
             address[] memory _hTokens,
             address[] memory _tokens,
             uint256[] memory _amounts,
             uint256[] memory _deposits,
             bytes memory _params,
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             GasParams memory _gParams,
             uint256 _value
         ) internal {

/// Missing zero check for `_refundee`
938:     function _performFallbackCall(address payable _refundee, uint32 _depositNonce, uint16 _dstChainId) internal {

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
/// Missing zero check for `_globalAddress`
966:     function _createSettlement(
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes memory _params,
             address _globalAddress,
             uint256 _amount,
             uint256 _deposit,
             bool _hasFallbackToggled
         ) internal returns (bytes memory _payload) {

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
1045:     function _createSettlementMultiple(
              uint32 _settlementNonce,
              address payable _refundee,
              address _recipient,
              uint16 _dstChainId,
              address[] memory _globalAddresses,
              uint256[] memory _amounts,
              uint256[] memory _deposits,
              bytes memory _params,
              bool _hasFallbackToggled
          ) internal returns (bytes memory _payload) {

/// Missing zero check for `_depositor`
/// Missing zero check for `_globalAddress`
1131:     function _updateStateOnBridgeOut(
              address _depositor,
              address _globalAddress,
              address _localAddress,
              address _underlyingAddress,
              uint256 _amount,
              uint256 _deposit,
              uint16 _dstChainId
          ) internal {

/// Missing zero check for `_newBranchBridgeAgent`
1176:     function syncBranchBridgeAgent(address _newBranchBridgeAgent, uint256 _branchChainId)
              external
              override
              requiresPort
          {

```
[#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L105) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L160) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L175) [#L202](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L202) [#L233](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L233) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L351) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L387) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L434) [#L768](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L768) [#L808](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L808) [#L856](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L856) [#L938](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L938) [#L966](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L966) [#L1045](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1045) [#L1131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1131) [#L1176](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1176) 

```solidity
File: src/RootBridgeAgentExecutor.sol

/// Missing zero check for `_rootBridgeAgent`
14:     function deploy(address _rootBridgeAgent) external returns (address) {

/// Missing zero check for `_rootBridgeAgent`
35:     constructor(address _rootBridgeAgent) {

/// Missing zero check for `_router`
50:     function executeSystemRequest(address _router, bytes calldata _payload, uint16 _srcChainId)
            external
            payable
            onlyOwner
        {

/// Missing zero check for `_router`
66:     function executeNoDeposit(address _router, bytes calldata _payload, uint16 _srcChainId)
            external
            payable
            onlyOwner
        {

/// Missing zero check for `_router`
82:     function executeWithDeposit(address _router, bytes calldata _payload, uint16 _srcChainId)
            external
            payable
            onlyOwner
        {

/// Missing zero check for `_router`
115:     function executeWithDepositMultiple(address _router, bytes calldata _payload, uint16 _srcChainId)
             external
             payable
             onlyOwner
         {

/// Missing zero check for `_account`
/// Missing zero check for `_router`
150:     function executeSignedNoDeposit(address _account, address _router, bytes calldata _payload, uint16 _srcChainId)
             external
             payable
             onlyOwner
         {

/// Missing zero check for `_account`
/// Missing zero check for `_router`
167:     function executeSignedWithDeposit(address _account, address _router, bytes calldata _payload, uint16 _srcChainId)
             external
             payable
             onlyOwner
         {

/// Missing zero check for `_account`
/// Missing zero check for `_router`
201:     function executeSignedWithDepositMultiple(
             address _account,
             address _router,
             bytes calldata _payload,
             uint16 _srcChainId
         ) external payable onlyOwner {

/// Missing zero check for `_recipient`
243:     function _bridgeIn(address _recipient, DepositParams memory _dParams, uint16 _srcChainId) internal {

/// Missing zero check for `_recipient`
268:     function _bridgeInMultiple(address _recipient, bytes calldata _dParams, uint16 _srcChainId)
             internal
             returns (DepositMultipleParams memory dParams)
         {

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L14) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L35) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L50) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L66) [#L82](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L82) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L115) [#L150](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L150) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L167) [#L201](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L201) [#L243](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L243) [#L268](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L268) 

```solidity
File: src/RootPort.sol

/// Missing zero check for `_localAddress`
175:     function getLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             external
             view
             override
             returns (address)
         {

/// Missing zero check for `_localAddress`
190:     function _getLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             internal
             view
             returns (address)
         {

/// Missing zero check for `_globalAddress`
200:     function getUnderlyingTokenFromGlobal(address _globalAddress, uint256 _srcChainId)
             external
             view
             override
             returns (address)
         {

/// Missing zero check for `_globalAddress`
211:     function isGlobalToken(address _globalAddress, uint256 _srcChainId) external view override returns (bool) {

/// Missing zero check for `_localAddress`
216:     function isLocalToken(address _localAddress, uint256 _srcChainId) external view override returns (bool) {

/// Missing zero check for `_localAddress`
221:     function isLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             external
             view
             returns (bool)
         {

/// Missing zero check for `_underlyingToken`
230:     function isUnderlyingToken(address _underlyingToken, uint256 _srcChainId) external view override returns (bool) {

/// Missing zero check for `_globalAddress`
259:     function setLocalAddress(address _globalAddress, address _localAddress, uint256 _srcChainId)
             external
             override
             requiresCoreRootRouter
         {

/// Missing zero check for `_recipient`
/// Missing zero check for `_hToken`
277:     function bridgeToRoot(address _recipient, address _hToken, uint256 _amount, uint256 _deposit, uint256 _srcChainId)
             external
             override
             requiresBridgeAgent
         {

/// Missing zero check for `_from`
/// Missing zero check for `_hToken`
294:     function bridgeToRootFromLocalBranch(address _from, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing zero check for `_to`
/// Missing zero check for `_hToken`
304:     function bridgeToLocalBranchFromRoot(address _to, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing zero check for `_from`
/// Missing zero check for `_hToken`
315:     function burn(address _from, address _hToken, uint256 _amount, uint256 _srcChainId)
             external
             override
             requiresBridgeAgent
         {

/// Missing zero check for `_from`
/// Missing zero check for `_hToken`
325:     function burnFromLocalBranch(address _from, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing zero check for `_to`
/// Missing zero check for `_hToken`
336:     function mintToLocalBranch(address _to, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing zero check for `_user`
350:     function fetchVirtualAccount(address _user) external override returns (VirtualAccount account) {

/// Missing zero check for `_router`
369:     function toggleVirtualAccountApproved(VirtualAccount _userAccount, address _router)
             external
             override
             requiresBridgeAgent
         {

/// Missing zero check for `_manager`
/// Missing zero check for `_bridgeAgent`
382:     function addBridgeAgent(address _manager, address _bridgeAgent) external override requiresBridgeAgentFactory {

/// Missing zero check for `_newBranchBridgeAgent`
/// Missing zero check for `_rootBridgeAgent`
393:     function syncBranchBridgeAgentWithRoot(
             address _newBranchBridgeAgent,
             address _rootBridgeAgent,
             uint256 _branchChainId
         ) external override requiresCoreRootRouter {

/// Missing zero check for `_bridgeAgent`
414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

/// Missing zero check for `_bridgeAgentFactory`
421:     function addBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

/// Missing zero check for `_bridgeAgentFactory`
431:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

/// Missing zero check for `_coreBranchBridgeAgentAddress`
/// Missing zero check for `_newLocalBranchWrappedNativeTokenAddress`
/// Missing zero check for `_newUnderlyingBranchWrappedNativeTokenAddress`
438:     function addNewChain(
             address _coreBranchBridgeAgentAddress,
             uint256 _chainId,
             string memory _wrappedGasTokenName,
             string memory _wrappedGasTokenSymbol,
             uint8 _wrappedGasTokenDecimals,
             address _newLocalBranchWrappedNativeTokenAddress,
             address _newUnderlyingBranchWrappedNativeTokenAddress
         ) external override onlyOwner {

/// Missing zero check for `_ecoTokenGlobalAddress`
483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

/// Missing zero check for `_refundee`
521:     function setCoreBranchRouter(
             address _refundee,
             address _coreBranchRouter,
             address _coreBranchBridgeAgent,
             uint16 _dstChainId,
             GasParams calldata _gParams
         ) external payable override onlyOwner {

```
[#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L175) [#L190](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L190) [#L200](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L200) [#L211](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L211) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L216) [#L221](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L221) [#L230](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L230) [#L259](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L259) [#L277](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L277) [#L294](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L294) [#L304](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L304) [#L315](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L315) [#L325](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L325) [#L336](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L336) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L350) [#L369](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L369) [#L382](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L382) [#L393](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L393) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L421) [#L431](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L431) [#L438](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L438) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) [#L521](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L521) 

```solidity
File: src/VirtualAccount.sol

/// Missing zero check for `_userAddress`
/// Missing zero check for `_localPortAddress`
35:     constructor(address _userAddress, address _localPortAddress) {

/// Missing zero check for `_token`
56:     function withdrawERC20(address _token, uint256 _amount) external override requiresApprovedCaller {

/// Missing zero check for `_token`
61:     function withdrawERC721(address _token, uint256 _tokenId) external override requiresApprovedCaller {

/// Missing zero check for ``
/// Missing zero check for ``
119:     function onERC721Received(address, address, uint256, bytes calldata) external pure override returns (bytes4) {

/// Missing zero check for ``
/// Missing zero check for ``
124:     function onERC1155Received(address, address, uint256, uint256, bytes calldata)
             external
             pure
             override
             returns (bytes4)
         {

/// Missing zero check for ``
/// Missing zero check for ``
134:     function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata)
             external
             pure
             override
             returns (bytes4)
         {

/// Missing zero check for `addr`
147:     function isContract(address addr) internal view returns (bool) {

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L35) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L56) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L61) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L119) [#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L124) [#L134](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L134) [#L147](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L147) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

/// Missing zero check for `_rootBridgeAgentFactoryAddress`
/// Missing zero check for `_localCoreBranchRouterAddress`
/// Missing zero check for `_localPortAddress`
/// Missing zero check for `_owner`
30:     constructor(
            uint16 _rootChainId,
            address _rootBridgeAgentFactoryAddress,
            address _localCoreBranchRouterAddress,
            address _localPortAddress,
            address _owner
        )
            BranchBridgeAgentFactory(
                _rootChainId,
                _rootChainId,
                _rootBridgeAgentFactoryAddress,
                address(0),
                _localCoreBranchRouterAddress,
                _localPortAddress,
                _owner
            )
        {}

/// Missing zero check for `_newBranchRouterAddress`
/// Missing zero check for `_rootBridgeAgentAddress`
/// Missing zero check for `_rootBridgeAgentFactoryAddress`
79:     function createBridgeAgent(
            address _newBranchRouterAddress,
            address _rootBridgeAgentAddress,
            address _rootBridgeAgentFactoryAddress
        ) external virtual override returns (address newBridgeAgent) {

```
[#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L30) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L79) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

/// Missing zero check for `_rootBridgeAgentFactoryAddress`
/// Missing zero check for `_lzEndpointAddress`
/// Missing zero check for `_localCoreBranchRouterAddress`
/// Missing zero check for `_localPortAddress`
/// Missing zero check for `_owner`
52:     constructor(
            uint16 _localChainId,
            uint16 _rootChainId,
            address _rootBridgeAgentFactoryAddress,
            address _lzEndpointAddress,
            address _localCoreBranchRouterAddress,
            address _localPortAddress,
            address _owner
        ) {

/// Missing zero check for `_newBranchRouterAddress`
/// Missing zero check for `_rootBridgeAgentAddress`
/// Missing zero check for `_rootBridgeAgentFactoryAddress`
115:     function createBridgeAgent(
             address _newBranchRouterAddress,
             address _rootBridgeAgentAddress,
             address _rootBridgeAgentFactoryAddress
         ) external virtual returns (address newBridgeAgent) {

```
[#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L52) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L115) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

/// Missing zero check for `_localPortAddress`
42:     constructor(uint16 _localChainId, address _localPortAddress, string memory _chainName, string memory _chainSymbol) {

/// Missing zero check for `_wrappedNativeTokenAddress`
60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L42) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

/// Missing zero check for `_rootPortAddress`
34:     constructor(uint16 _localChainId, address _rootPortAddress) {

```
[#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L34) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

/// Missing zero check for `_lzEndpointAddress`
/// Missing zero check for `_rootPortAddress`
31:     constructor(uint16 _rootChainId, address _lzEndpointAddress, address _rootPortAddress) {

/// Missing zero check for `_newRootRouterAddress`
48:     function createBridgeAgent(address _newRootRouterAddress) external returns (address newBridgeAgent) {

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L31) [#L48](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L48) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

/// Missing zero check for `_depositor`
/// Missing zero check for `_recipient`
/// Missing zero check for `_underlyingAddress`
28:     function depositToPort(address _depositor, address _recipient, address _underlyingAddress, uint256 _amount)

/// Missing zero check for `_depositor`
/// Missing zero check for `_recipient`
/// Missing zero check for `_globalAddress`
38:     function withdrawFromPort(address _depositor, address _recipient, address _globalAddress, uint256 _amount)

```
[#L28](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L28) [#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L38) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

/// Missing zero check for `gasRefundee`
138:     function callOutSystem(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Missing zero check for `gasRefundee`
150:     function callOut(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Missing zero check for `gasRefundee`
163:     function callOutAndBridge(

/// Missing zero check for `gasRefundee`
179:     function callOutAndBridgeMultiple(

/// Missing zero check for `gasRefundee`
194:     function callOutSigned(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Missing zero check for `gasRefundee`
208:     function callOutSignedAndBridge(

/// Missing zero check for `gasRefundee`
227:     function callOutSignedAndBridgeMultiple(

/// Missing zero check for `recipient`
/// Missing zero check for `hToken`
/// Missing zero check for `token`
305:     function clearToken(address recipient, address hToken, address token, uint256 amount, uint256 deposit) external;

/// Missing zero check for `recipient`
312:     function clearTokens(bytes calldata sParams, address recipient)

/// Missing zero check for `_endpoint`
326:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload) external;

```
[#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L138) [#L150](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L150) [#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L163) [#L179](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L179) [#L194](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L194) [#L208](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L208) [#L227](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L227) [#L305](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L305) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L312) [#L326](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L326) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

/// Missing zero check for `newRootRouterAddress`
/// Missing zero check for `rootBridgeAgentAddress`
/// Missing zero check for `_rootBridgeAgentFactoryAddress`
24:     function createBridgeAgent(

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L24) 

```solidity
File: src/interfaces/IBranchPort.sol

/// Missing zero check for `_bridgeAgent`
23:     function isBridgeAgent(address _bridgeAgent) external view returns (bool);

/// Missing zero check for `_token`
30:     function isStrategyToken(address _token) external view returns (bool);

/// Missing zero check for `_strategy`
/// Missing zero check for `_token`
38:     function isPortStrategy(address _strategy, address _token) external view returns (bool);

/// Missing zero check for `_bridgeAgentFactory`
45:     function isBridgeAgentFactory(address _bridgeAgentFactory) external view returns (bool);

/// Missing zero check for `_token`
56:     function manage(address _token, uint256 _amount) external;

/// Missing zero check for `_token`
64:     function replenishReserves(address _token, uint256 _amount) external;

/// Missing zero check for `_strategy`
/// Missing zero check for `_token`
72:     function replenishReserves(address _strategy, address _token) external;

/// Missing zero check for `_recipient`
/// Missing zero check for `_underlyingAddress`
85:     function withdraw(address _recipient, address _underlyingAddress, uint256 _amount) external;

/// Missing zero check for `_recipient`
/// Missing zero check for `_localAddress`
94:     function bridgeIn(address _recipient, address _localAddress, uint256 _amount) external;

/// Missing zero check for `_recipient`
103:     function bridgeInMultiple(

/// Missing zero check for `_depositor`
/// Missing zero check for `_localAddress`
/// Missing zero check for `_underlyingAddress`
118:     function bridgeOut(

/// Missing zero check for `_depositor`
135:     function bridgeOutMultiple(

/// Missing zero check for `_bridgeAgent`
151:     function addBridgeAgent(address _bridgeAgent) external;

/// Missing zero check for `_newCoreRouter`
157:     function setCoreRouter(address _newCoreRouter) external;

/// Missing zero check for `_bridgeAgentFactory`
163:     function addBridgeAgentFactory(address _bridgeAgentFactory) external;

/// Missing zero check for `_newBridgeAgentFactory`
169:     function toggleBridgeAgentFactory(address _newBridgeAgentFactory) external;

/// Missing zero check for `_bridgeAgent`
175:     function toggleBridgeAgent(address _bridgeAgent) external;

/// Missing zero check for `_token`
181:     function addStrategyToken(address _token, uint256 _minimumReservesRatio) external;

/// Missing zero check for `_token`
187:     function toggleStrategyToken(address _token) external;

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_token`
193:     function addPortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit) external;

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_token`
199:     function togglePortStrategy(address _portStrategy, address _token) external;

/// Missing zero check for `_portStrategy`
/// Missing zero check for `_token`
207:     function updatePortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit) external;

/// Missing zero check for `_coreBranchRouter`
/// Missing zero check for `_coreBranchBridgeAgent`
214:     function setCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent) external;

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L23) [#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L30) [#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L38) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L45) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L56) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L64) [#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L72) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L85) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L94) [#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L103) [#L118](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L118) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L135) [#L151](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L151) [#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L157) [#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L163) [#L169](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L169) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L175) [#L181](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L181) [#L187](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L187) [#L193](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L193) [#L199](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L199) [#L207](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L207) [#L214](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L214) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

/// Missing zero check for `_globalAddress`
38:     function addGlobalToken(address _globalAddress, uint256 _dstChainId, GasParams[3] calldata _gasParams)

/// Missing zero check for `_underlyingAddress`
47:     function addLocalToken(address _underlyingAddress, GasParams calldata _gasParams) external payable;

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L38) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L47) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

/// Missing zero check for `account`
22:     function mint(address account, uint256 amount) external returns (bool);

```
[#L22](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L22) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

/// Missing zero check for `to`
43:     function mint(address to, uint256 amount, uint256 chainId) external returns (bool);

/// Missing zero check for `from`
51:     function burn(address from, uint256 amount, uint256 chainId) external;

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L43) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L51) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

/// Missing zero check for `_refundAddress`
/// Missing zero check for `_zroPaymentAddress`
15:     function send(

/// Missing zero check for `_dstAddress`
31:     function receivePayload(

/// Missing zero check for `_srcAddress`
47:     function getOutboundNonce(uint16 _dstChainId, address _srcAddress) external view returns (uint64);

/// Missing zero check for `_userApplication`
55:     function estimateFees(

/// Missing zero check for `_userApplication`
79:     function getSendLibraryAddress(address _userApplication) external view returns (address);

/// Missing zero check for `_userApplication`
83:     function getReceiveLibraryAddress(address _userApplication) external view returns (address);

/// Missing zero check for `_userApplication`
98:     function getConfig(uint16 _version, uint16 _chainId, address _userApplication, uint256 _configType)

/// Missing zero check for `_userApplication`
105:     function getSendVersion(address _userApplication) external view returns (uint16);

/// Missing zero check for `_userApplication`
109:     function getReceiveVersion(address _userApplication) external view returns (uint16);

```
[#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L15) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L31) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L47) [#L55](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L55) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L79) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L83) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L98) [#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L105) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L109) 

```solidity
File: src/interfaces/IPortStrategy.sol

/// Missing zero check for `_recipient`
/// Missing zero check for `_token`
23:     function withdraw(address _recipient, address _token, uint256 _amount) external;

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L23) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
168:     function callOut(

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
189:     function callOutAndBridge(

/// Missing zero check for `_refundee`
/// Missing zero check for `_recipient`
213:     function callOutAndBridgeMultiple(

/// Missing zero check for `_recipient`
236:     function retrySettlement(

/// Missing zero check for `_recipient`
271:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId) external;

/// Missing zero check for `_recipient`
295:     function bridgeInMultiple(address _recipient, DepositMultipleParams calldata _dParams, uint256 _srcChainId)

/// Missing zero check for `_endpoint`
309:     function lzReceiveNonBlocking(

/// Missing zero check for `_newBranchBridgeAgent`
331:     function syncBranchBridgeAgent(address _newBranchBridgeAgent, uint256 _branchChainId) external;

```
[#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L168) [#L189](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L189) [#L213](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L213) [#L236](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L236) [#L271](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L271) [#L295](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L295) [#L309](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L309) [#L331](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L331) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

/// Missing zero check for `newRootRouterAddress`
16:     function createBridgeAgent(address newRootRouterAddress) external returns (address newBridgeAgent);

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L16) 

```solidity
File: src/interfaces/IRootPort.sol

/// Missing zero check for `_refundee`
/// Missing zero check for `_coreBranchRouter`
/// Missing zero check for `_coreBranchBridgeAgent`
13:     function setCoreBranch(

/// Missing zero check for `_rootBridgeAgent`
47:     function getBridgeAgentManager(address _rootBridgeAgent) external view returns (address);

/// Missing zero check for `_bridgeAgentFactory`
54:     function isBridgeAgentFactory(address _bridgeAgentFactory) external view returns (bool);

/// Missing zero check for `_globalAddress`
61:     function isGlobalAddress(address _globalAddress) external view returns (bool);

/// Missing zero check for `_localAddress`
69:     function getGlobalTokenFromLocal(address _localAddress, uint256 _srcChainId) external view returns (address);

/// Missing zero check for `_globalAddress`
77:     function getLocalTokenFromGlobal(address _globalAddress, uint256 _srcChainId) external view returns (address);

/// Missing zero check for `_underlyingAddress`
85:     function getLocalTokenFromUnderlying(address _underlyingAddress, uint256 _srcChainId)

/// Missing zero check for `_localAddress`
97:     function getLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)

/// Missing zero check for `_localAddress`
108:     function getUnderlyingTokenFromLocal(address _localAddress, uint256 _srcChainId) external view returns (address);

/// Missing zero check for `_globalAddress`
116:     function getUnderlyingTokenFromGlobal(address _globalAddress, uint256 _srcChainId)

/// Missing zero check for `_globalAddress`
127:     function isGlobalToken(address _globalAddress, uint256 _srcChainId) external view returns (bool);

/// Missing zero check for `_localAddress`
135:     function isLocalToken(address _localAddress, uint256 _srcChainId) external view returns (bool);

/// Missing zero check for `_localAddress`
144:     function isLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)

/// Missing zero check for `_underlyingToken`
155:     function isUnderlyingToken(address _underlyingToken, uint256 _srcChainId) external view returns (bool);

/// Missing zero check for `_user`
162:     function getUserAccount(address _user) external view returns (VirtualAccount);

/// Missing zero check for `_router`
170:     function isRouterApproved(VirtualAccount _userAccount, address _router) external returns (bool);

/// Missing zero check for `_from`
/// Missing zero check for `_hToken`
183:     function burn(address _from, address _hToken, uint256 _amount, uint256 _srcChainId) external;

/// Missing zero check for `_recipient`
/// Missing zero check for `_hToken`
193:     function bridgeToRoot(address _recipient, address _hToken, uint256 _amount, uint256 _deposit, uint256 _srcChainId)

/// Missing zero check for `_from`
/// Missing zero check for `_hToken`
202:     function bridgeToRootFromLocalBranch(address _from, address _hToken, uint256 _amount) external;

/// Missing zero check for `_to`
/// Missing zero check for `_hToken`
210:     function bridgeToLocalBranchFromRoot(address _to, address _hToken, uint256 _amount) external;

/// Missing zero check for `_recipient`
/// Missing zero check for `_hToken`
218:     function mintToLocalBranch(address _recipient, address _hToken, uint256 _amount) external;

/// Missing zero check for `_from`
/// Missing zero check for `_hToken`
226:     function burnFromLocalBranch(address _from, address _hToken, uint256 _amount) external;

/// Missing zero check for `_globalAddress`
/// Missing zero check for `_localAddress`
/// Missing zero check for `_underlyingAddress`
238:     function setAddresses(

/// Missing zero check for `_globalAddress`
/// Missing zero check for `_localAddress`
251:     function setLocalAddress(address _globalAddress, address _localAddress, uint256 _srcChainId) external;

/// Missing zero check for `_user`
261:     function fetchVirtualAccount(address _user) external returns (VirtualAccount account);

/// Missing zero check for `_router`
269:     function toggleVirtualAccountApproved(VirtualAccount _userAccount, address _router) external;

/// Missing zero check for `_newBranchBridgeAgent`
/// Missing zero check for `_rootBridgeAgent`
281:     function syncBranchBridgeAgentWithRoot(address _newBranchBridgeAgent, address _rootBridgeAgent, uint256 _srcChainId)

/// Missing zero check for `_manager`
/// Missing zero check for `_bridgeAgent`
289:     function addBridgeAgent(address _manager, address _bridgeAgent) external;

/// Missing zero check for `_bridgeAgent`
295:     function toggleBridgeAgent(address _bridgeAgent) external;

/// Missing zero check for `_bridgeAgentFactory`
301:     function addBridgeAgentFactory(address _bridgeAgentFactory) external;

/// Missing zero check for `_bridgeAgentFactory`
307:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external;

/// Missing zero check for `_coreBranchBridgeAgentAddress`
/// Missing zero check for `_newLocalBranchWrappedNativeTokenAddress`
/// Missing zero check for `_newUnderlyingBranchWrappedNativeTokenAddress`
319:     function addNewChain(

/// Missing zero check for `ecoTokenGlobalAddress`
333:     function addEcosystemToken(address ecoTokenGlobalAddress) external;

/// Missing zero check for `_coreRootRouter`
/// Missing zero check for `_coreRootBridgeAgent`
340:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external;

/// Missing zero check for `_refundee`
/// Missing zero check for `_coreBranchRouter`
/// Missing zero check for `_coreBranchBridgeAgent`
350:     function setCoreBranchRouter(

/// Missing zero check for `_coreBranchRouter`
/// Missing zero check for `_coreBranchBridgeAgent`
364:     function syncNewCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent, uint16 _dstChainId)

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L13) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L47) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L54) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L61) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L69) [#L77](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L77) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L85) [#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L97) [#L108](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L108) [#L116](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L116) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L127) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L135) [#L144](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L144) [#L155](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L155) [#L162](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L162) [#L170](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L170) [#L183](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L183) [#L193](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L193) [#L202](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L202) [#L210](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L210) [#L218](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L218) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L226) [#L238](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L238) [#L251](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L251) [#L261](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L261) [#L269](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L269) [#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L281) [#L289](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L289) [#L295](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L295) [#L301](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L301) [#L307](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L307) [#L319](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L319) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L333) [#L340](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L340) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L350) [#L364](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L364) 

```solidity
File: src/interfaces/IRootRouter.sol

/// Missing zero check for `userAccount`
63:     function executeSigned(bytes memory params, address userAccount, uint16 srcChainId) external payable;

/// Missing zero check for `userAccount`
72:     function executeSignedDepositSingle(

/// Missing zero check for `userAccount`
86:     function executeSignedDepositMultiple(

```
[#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L63) [#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L72) [#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L86) 

```solidity
File: src/interfaces/IVirtualAccount.sol

/// Missing zero check for `_token`
51:     function withdrawERC20(address _token, uint256 _amount) external;

/// Missing zero check for `_token`
58:     function withdrawERC721(address _token, uint256 _tokenId) external;

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L51) [#L58](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L58) 

```solidity
File: src/token/ERC20hTokenBranch.sol

/// Missing zero check for `_owner`
13:     constructor(
            string memory chainName,
            string memory chainSymbol,
            string memory _name,
            string memory _symbol,
            uint8 _decimals,
            address _owner
        ) ERC20(string(string.concat(chainName, _name)), string(string.concat(chainSymbol, _symbol)), _decimals) {

/// Missing zero check for `account`
29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L13) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) 

```solidity
File: src/token/ERC20hTokenRoot.sol

/// Missing zero check for `_factoryAddress`
/// Missing zero check for `_rootPortAddress`
31:     constructor(
            uint16 _localChainId,
            address _factoryAddress,
            address _rootPortAddress,
            string memory _name,
            string memory _symbol,
            uint8 _decimals
        ) ERC20(string(string.concat(_name)), string(string.concat(_symbol)), _decimals) {

/// Missing zero check for `to`
57:     function mint(address to, uint256 amount, uint256 chainId) external onlyOwner returns (bool) {

/// Missing zero check for `from`
69:     function burn(address from, uint256 amount, uint256 chainId) external onlyOwner {

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L31) [#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L57) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L69) 

</details>

---

<a name="NC-21"></a> 
### [NC-21] Consider moving `msg.sender` checks to `modifier`s
If some functions are only allowed to be called by some specific users, consider using a modifier instead of checking with a require statement, especially if this check is done in multiple functions.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: src/CoreRootRouter.sol

278:         require(msg.sender == rootPortAddress, "Only root port can call");

```
[#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L278) 

</details>

---

<a name="NC-22"></a> 
### [NC-22] NatSpec documentation for contract is missing
e.g. `@dev` or `@notice`, and it must appear above the contract definition braces in order to be identified by the compiler as NatSpec.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

10: library DeployArbitrumBranchBridgeAgent {

```
[#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L10) 

```solidity
File: src/ArbitrumBranchPort.sol

14: contract ArbitrumBranchPort is BranchPort, IArbitrumBranchPort {

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L14) 

```solidity
File: src/BaseBranchRouter.sol

25: contract BaseBranchRouter is IBranchRouter, Ownable {

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L25) 

```solidity
File: src/BranchBridgeAgent.sol

23: library DeployBranchBridgeAgent {

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L23) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

15: library DeployBranchBridgeAgentExecutor {

```
[#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L15) 

```solidity
File: src/BranchPort.sol

17: contract BranchPort is Ownable, IBranchPort {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L17) 

```solidity
File: src/CoreBranchRouter.sol

18: contract CoreBranchRouter is ICoreBranchRouter, BaseBranchRouter {

```
[#L18](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L18) 

```solidity
File: src/RootBridgeAgent.sol

32: contract RootBridgeAgent is IRootBridgeAgent, BridgeAgentConstants {

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L32) 

```solidity
File: src/RootBridgeAgentExecutor.sol

13: library DeployRootBridgeAgentExecutor {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L13) 

```solidity
File: src/RootPort.sol

16: contract RootPort is Ownable, IRootPort {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L16) 

```solidity
File: src/VirtualAccount.sol

17: contract VirtualAccount is IVirtualAccount, ERC1155Receiver {

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L17) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

12: contract ERC20hTokenBranchFactory is Ownable, IERC20hTokenBranchFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L12) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

12: contract ERC20hTokenRootFactory is Ownable, IERC20hTokenRootFactory {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L12) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

11: contract RootBridgeAgentFactory is IRootBridgeAgentFactory {

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L11) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

7: interface ILayerZeroEndpoint is ILayerZeroUserApplicationConfig {

```
[#L7](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L7) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

5: interface ILayerZeroReceiver {

```
[#L5](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L5) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

5: interface ILayerZeroUserApplicationConfig {

```
[#L5](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L5) 

```solidity
File: src/interfaces/IMulticall2.sol

9: interface IMulticall2 {

```
[#L9](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L9) 

```solidity
File: src/interfaces/IRootPort.sol

10: interface ICoreRootRouter {

```
[#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L10) 

```solidity
File: src/token/ERC20hTokenBranch.sol

12: contract ERC20hTokenBranch is ERC20, Ownable, IERC20hTokenBranch {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L12) 

```solidity
File: src/token/ERC20hTokenRoot.sol

12: contract ERC20hTokenRoot is ERC20, Ownable, IERC20hTokenRoot {

```
[#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L12) 

</details>

---

<a name="NC-23"></a> 
### [NC-23] Event declarations should have NatSpec descriptions

<details>
<summary>
There are <b>28</b> instances (click to show):
</summary>

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

332:     event LogExecute(uint256 indexed nonce);

333:     event LogFallback(uint256 indexed nonce);

```
[#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L332) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L333) 

```solidity
File: src/interfaces/IBranchPort.sol

220:     event DebtCreated(address indexed _strategy, address indexed _token, uint256 _amount);

221:     event DebtRepaid(address indexed _strategy, address indexed _token, uint256 _amount);

223:     event StrategyTokenAdded(address indexed _token, uint256 indexed _minimumReservesRatio);

224:     event StrategyTokenToggled(address indexed _token);

226:     event PortStrategyAdded(

229:     event PortStrategyToggled(address indexed _portStrategy, address indexed _token);

230:     event PortStrategyUpdated(

234:     event BridgeAgentFactoryAdded(address indexed _bridgeAgentFactory);

235:     event BridgeAgentFactoryToggled(address indexed _bridgeAgentFactory);

237:     event BridgeAgentToggled(address indexed _bridgeAgent);

239:     event CoreBranchSet(address indexed _coreBranchRouter, address indexed _coreBranchBridgeAgent);

```
[#L220](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L220) [#L221](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L221) [#L223](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L223) [#L224](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L224) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L226) [#L229](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L229) [#L230](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L230) [#L234](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L234) [#L235](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L235) [#L237](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L237) [#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L239) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

337:     event LogExecute(uint256 indexed depositNonce, uint256 indexed srcChainId);

338:     event LogFallback(uint256 indexed settlementNonce, uint256 indexed dstChainId);

```
[#L337](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L337) [#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L338) 

```solidity
File: src/interfaces/IRootPort.sol

371:     event BridgeAgentFactoryAdded(address indexed bridgeAgentFactory);

372:     event BridgeAgentFactoryToggled(address indexed bridgeAgentFactory);

374:     event BridgeAgentAdded(address indexed bridgeAgent, address indexed manager);

375:     event BridgeAgentToggled(address indexed bridgeAgent);

376:     event BridgeAgentSynced(address indexed bridgeAgent, address indexed rootBridgeAgent, uint256 indexed srcChainId);

378:     event NewChainAdded(uint256 indexed chainId);

380:     event VirtualAccountCreated(address indexed user, address account);

382:     event LocalTokenAdded(

385:     event GlobalTokenAdded(address indexed localAddress, address indexed globalAddress, uint256 indexed chainId);

386:     event EcosystemTokenAdded(address indexed ecoTokenGlobalAddress);

387:     event CoreRootSet(address indexed coreRootRouter, address indexed coreRootBridgeAgent);

388:     event CoreBranchSet(

391:     event CoreBranchSynced(

```
[#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L371) [#L372](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L372) [#L374](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L374) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L375) [#L376](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L376) [#L378](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L378) [#L380](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L380) [#L382](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L382) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L385) [#L386](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L386) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L387) [#L388](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L388) [#L391](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L391) 

</details>

---

<a name="NC-24"></a> 
### [NC-24] NatSpec documentation for function is missing
It is recommended that Solidity contracts are fully annotated using NatSpec for all public interfaces (everything in the ABI). It is clearly stated in the Solidity official documentation. In complex projects such as DeFi, the interpretation of all functions and their arguments and returns is important for code readability and auditability.

<details>
<summary>
There are <b>40</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

11:     function deploy(uint16 _localChainId, address _daoAddress, address _localRouterAddress, address _localPortAddress)
            external
            returns (ArbitrumBranchBridgeAgent)
        {

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L11) 

```solidity
File: src/BaseBranchRouter.sol

48:     constructor() {

```
[#L48](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L48) 

```solidity
File: src/BranchBridgeAgent.sol

24:     function deploy(
            uint16 _rootChainId,
            uint16 _localChainId,
            address _rootBridgeAgentAddress,
            address _lzEndpointAddress,
            address _localRouterAddress,
            address _localPortAddress
        ) external returns (BranchBridgeAgent) {

149:     receive() external payable {}

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L24) [#L149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L149) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

16:     function deploy() external returns (address) {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L16) 

```solidity
File: src/CoreRootRouter.sol

83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) 

```solidity
File: src/MulticallRootRouter.sol

581:     function _decode(bytes calldata data) internal pure virtual returns (bytes memory) {

```
[#L581](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L581) 

```solidity
File: src/MulticallRootRouterLibZip.sol

29:     constructor(uint256 _localChainId, address _localPortAddress, address _multicallAddress)
            MulticallRootRouter(_localChainId, _localPortAddress, _multicallAddress)
        {}

37:     function _decode(bytes calldata data) internal pure override returns (bytes memory) {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L29) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L37) 

```solidity
File: src/RootBridgeAgent.sol

128:     receive() external payable {}

```
[#L128](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L128) 

```solidity
File: src/RootBridgeAgentExecutor.sol

14:     function deploy(address _rootBridgeAgent) external returns (address) {

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L14) 

```solidity
File: src/RootPort.sol

304:     function bridgeToLocalBranchFromRoot(address _to, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

```
[#L304](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L304) 

```solidity
File: src/VirtualAccount.sol

44:     receive() external payable {}

147:     function isContract(address addr) internal view returns (bool) {

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L44) [#L147](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L147) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

15:     function send(

31:     function receivePayload(

43:     function getInboundNonce(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (uint64);

47:     function getOutboundNonce(uint16 _dstChainId, address _srcAddress) external view returns (uint64);

55:     function estimateFees(

64:     function getChainId() external view returns (uint16);

70:     function retryPayload(uint16 _srcChainId, bytes calldata _srcAddress, bytes calldata _payload) external;

75:     function hasStoredPayload(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (bool);

79:     function getSendLibraryAddress(address _userApplication) external view returns (address);

83:     function getReceiveLibraryAddress(address _userApplication) external view returns (address);

87:     function isSendingPayload() external view returns (bool);

91:     function isReceivingPayload() external view returns (bool);

98:     function getConfig(uint16 _version, uint16 _chainId, address _userApplication, uint256 _configType)

105:     function getSendVersion(address _userApplication) external view returns (uint16);

109:     function getReceiveVersion(address _userApplication) external view returns (uint16);

```
[#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L15) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L31) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L43) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L47) [#L55](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L55) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L64) [#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L70) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L75) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L79) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L83) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L87) [#L91](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L91) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L98) [#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L105) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L109) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

11:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64 _nonce, bytes calldata _payload) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L11) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

11:     function setConfig(uint16 _version, uint16 _chainId, uint256 _configType, bytes calldata _config) external;

15:     function setSendVersion(uint16 _version) external;

19:     function setReceiveVersion(uint16 _version) external;

24:     function forceResumeReceive(uint16 _srcChainId, bytes calldata _srcAddress) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L11) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L15) [#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L19) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L24) 

```solidity
File: src/interfaces/IMulticall2.sol

20:     function aggregate(Call[] memory calls) external returns (uint256 blockNumber, bytes[] memory returnData);

```
[#L20](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L20) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

16:     function createBridgeAgent(address newRootRouterAddress) external returns (address newBridgeAgent);

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L16) 

```solidity
File: src/interfaces/IRootPort.sol

11:     function bridgeAgentAddress() external view returns (address);

12:     function hTokenFactoryAddress() external view returns (address);

13:     function setCoreBranch(

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L11) [#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L12) [#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L13) 

```solidity
File: src/token/ERC20hTokenBranch.sol

13:     constructor(
            string memory chainName,
            string memory chainSymbol,
            string memory _name,
            string memory _symbol,
            uint8 _decimals,
            address _owner
        ) ERC20(string(string.concat(chainName, _name)), string(string.concat(chainSymbol, _symbol)), _decimals) {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L13) 

</details>

---

<a name="NC-25"></a> 
### [NC-25] Missing NatSpec `@param`
Some functions have an incomplete NatSpec: add a `@param` notation to describe the function parameters to improve the code documentation.

<details>
<summary>
There are <b>151</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// Missing @param for _localChainId
/// Missing @param for _daoAddress
/// Missing @param for _localRouterAddress
/// Missing @param for _localPortAddress
11:     function deploy(uint16 _localChainId, address _daoAddress, address _localRouterAddress, address _localPortAddress)
            external
            returns (ArbitrumBranchBridgeAgent)
        {

/// Missing @param for _endpoint
125:     function _requiresEndpoint(address _endpoint, bytes calldata) internal view override {

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L11) [#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L125) 

```solidity
File: src/ArbitrumBranchPort.sol

/// Missing @param for _depositor
/// Missing @param for _recipient
/// Missing @param for _underlyingAddress
/// Missing @param for _deposit
50:     function depositToPort(address _depositor, address _recipient, address _underlyingAddress, uint256 _deposit)
            external
            override
            lock
            requiresBridgeAgent
        {

/// Missing @param for _depositor
/// Missing @param for _recipient
/// Missing @param for _globalAddress
/// Missing @param for _amount
73:     function withdrawFromPort(address _depositor, address _recipient, address _globalAddress, uint256 _amount)
            external
            override
            lock
            requiresBridgeAgent
        {

```
[#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L50) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L73) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

/// Missing @param for _underlyingAddress
51:     function addLocalToken(address _underlyingAddress, GasParams calldata) external payable override {

/// Missing @param for _data
126:     function executeNoSettlement(bytes calldata _data) external payable override requiresAgentExecutor {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L51) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L126) 

```solidity
File: src/BaseBranchRouter.sol

/// Missing @param for _depositNonce
74:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

/// Missing @param for _params
/// Missing @param for _gParams
83:     function callOut(bytes calldata _params, GasParams calldata _gParams) external payable override lock {

/// Missing @param for _params
/// Missing @param for _dParams
/// Missing @param for _gParams
88:     function callOutAndBridge(bytes calldata _params, DepositInput calldata _dParams, GasParams calldata _gParams)
            external
            payable
            override
            lock
        {

/// Missing @param for _params
/// Missing @param for _dParams
/// Missing @param for _gParams
104:     function callOutAndBridgeMultiple(
             bytes calldata _params,
             DepositMultipleInput calldata _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

```
[#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L74) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L83) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L88) [#L104](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L104) 

```solidity
File: src/BranchBridgeAgent.sol

/// Missing @param for _rootChainId
/// Missing @param for _localChainId
/// Missing @param for _rootBridgeAgentAddress
/// Missing @param for _lzEndpointAddress
/// Missing @param for _localRouterAddress
/// Missing @param for _localPortAddress
24:     function deploy(
            uint16 _rootChainId,
            uint16 _localChainId,
            address _rootBridgeAgentAddress,
            address _lzEndpointAddress,
            address _localRouterAddress,
            address _localPortAddress
        ) external returns (BranchBridgeAgent) {

/// Missing @param for _depositNonce
156:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

/// Missing @param for _gasLimit
/// Missing @param for _remoteBranchExecutionGas
/// Missing @param for _payload
161:     function getFeeEstimate(uint256 _gasLimit, uint256 _remoteBranchExecutionGas, bytes calldata _payload)
             external
             view
             returns (uint256 _fee)
         {

/// Missing @param for _refundee
/// Missing @param for _params
/// Missing @param for _gParams
180:     function callOutSystem(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
             requiresRouter
         {

/// Missing @param for _refundee
/// Missing @param for _params
/// Missing @param for _gParams
195:     function callOut(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
         {

/// Missing @param for _refundee
/// Missing @param for _params
/// Missing @param for _dParams
/// Missing @param for _gParams
209:     function callOutAndBridge(
             address payable _refundee,
             bytes calldata _params,
             DepositInput memory _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

/// Missing @param for _refundee
/// Missing @param for _params
/// Missing @param for _dParams
/// Missing @param for _gParams
231:     function callOutAndBridgeMultiple(
             address payable _refundee,
             bytes calldata _params,
             DepositMultipleInput memory _dParams,
             GasParams calldata _gParams
         ) external payable override lock {

/// Missing @param for _refundee
/// Missing @param for _params
/// Missing @param for _gParams
262:     function callOutSigned(address payable _refundee, bytes calldata _params, GasParams calldata _gParams)
             external
             payable
             override
             lock
         {

/// Missing @param for _refundee
/// Missing @param for _params
/// Missing @param for _dParams
/// Missing @param for _gParams
/// Missing @param for _hasFallbackToggled
276:     function callOutSignedAndBridge(
             address payable _refundee,
             bytes calldata _params,
             DepositInput memory _dParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing @param for _refundee
/// Missing @param for _params
/// Missing @param for _dParams
/// Missing @param for _gParams
/// Missing @param for _hasFallbackToggled
306:     function callOutSignedAndBridgeMultiple(
             address payable _refundee,
             bytes calldata _params,
             DepositMultipleInput memory _dParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing @param for _isSigned
/// Missing @param for _depositNonce
/// Missing @param for _params
/// Missing @param for _gParams
/// Missing @param for _hasFallbackToggled
343:     function retryDeposit(
             bool _isSigned,
             uint32 _depositNonce,
             bytes calldata _params,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing @param for _depositNonce
/// Missing @param for _gParams
422:     function retrieveDeposit(uint32 _depositNonce, GasParams calldata _gParams) external payable override lock {

/// Missing @param for _depositNonce
434:     function redeemDeposit(uint32 _depositNonce) external override lock {

/// Missing @param for _settlementNonce
/// Missing @param for _params
/// Missing @param for _gParams
/// Missing @param for _hasFallbackToggled
464:     function retrySettlement(
             uint32 _settlementNonce,
             bytes calldata _params,
             GasParams[2] calldata _gParams,
             bool _hasFallbackToggled
         ) external payable virtual override lock {

/// Missing @param for _recipient
/// Missing @param for _hToken
/// Missing @param for _token
/// Missing @param for _amount
/// Missing @param for _deposit
485:     function clearToken(address _recipient, address _hToken, address _token, uint256 _amount, uint256 _deposit)
             external
             override
             requiresAgentExecutor
         {

/// Missing @param for _sParams
/// Missing @param for _recipient
494:     function clearTokens(bytes calldata _sParams, address _recipient)
             external
             override
             requiresAgentExecutor
             returns (SettlementMultipleParams memory)
         {

/// Missing @param for _srcAddress
/// Missing @param for _payload
578:     function lzReceive(uint16, bytes calldata _srcAddress, uint64, bytes calldata _payload) public override {

/// Missing @param for _endpoint
/// Missing @param for _srcAddress
/// Missing @param for _payload
587:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload)
             public
             override
             requiresEndpoint(_endpoint, _srcAddress)
         {

/// Missing @param for _endpoint
/// Missing @param for _srcAddress
936:     function _requiresEndpoint(address _endpoint, bytes calldata _srcAddress) internal view virtual {

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L24) [#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L156) [#L161](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L161) [#L180](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L180) [#L195](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L195) [#L209](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L209) [#L231](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L231) [#L262](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L262) [#L276](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L276) [#L306](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L306) [#L343](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L343) [#L422](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L422) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L434) [#L464](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L464) [#L485](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L485) [#L494](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L494) [#L578](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L578) [#L587](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L587) [#L936](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L936) 

```solidity
File: src/BranchPort.sol

/// Missing @param for _token
/// Missing @param for _amount
144:     function manage(address _token, uint256 _amount) external override requiresPortStrategy(_token) {

/// Missing @param for _token
/// Missing @param for _amount
167:     function replenishReserves(address _token, uint256 _amount) external override lock {

/// Missing @param for _strategy
/// Missing @param for _token
188:     function replenishReserves(address _strategy, address _token) external override lock {

/// Missing @param for _recipient
/// Missing @param for _underlyingAddress
/// Missing @param for _deposit
226:     function withdraw(address _recipient, address _underlyingAddress, uint256 _deposit)
             public
             virtual
             override
             lock
             requiresBridgeAgent
         {

/// Missing @param for _recipient
/// Missing @param for _localAddress
/// Missing @param for _amount
237:     function bridgeIn(address _recipient, address _localAddress, uint256 _amount)
             external
             override
             requiresBridgeAgent
         {

/// Missing @param for _recipient
/// Missing @param for _localAddresses
/// Missing @param for _underlyingAddresses
/// Missing @param for _amounts
/// Missing @param for _deposits
246:     function bridgeInMultiple(
             address _recipient,
             address[] memory _localAddresses,
             address[] memory _underlyingAddresses,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) external override requiresBridgeAgent {

/// Missing @param for _depositor
/// Missing @param for _localAddress
/// Missing @param for _underlyingAddress
/// Missing @param for _amount
/// Missing @param for _deposit
277:     function bridgeOut(
             address _depositor,
             address _localAddress,
             address _underlyingAddress,
             uint256 _amount,
             uint256 _deposit
         ) external override lock requiresBridgeAgent {

/// Missing @param for _depositor
/// Missing @param for _localAddresses
/// Missing @param for _underlyingAddresses
/// Missing @param for _amounts
/// Missing @param for _deposits
288:     function bridgeOutMultiple(
             address _depositor,
             address[] memory _localAddresses,
             address[] memory _underlyingAddresses,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) external override lock requiresBridgeAgent {

/// Missing @param for _bridgeAgent
319:     function addBridgeAgent(address _bridgeAgent) external override requiresBridgeAgentFactory {

/// Missing @param for _newCoreRouter
331:     function setCoreRouter(address _newCoreRouter) external override requiresCoreRouter {

/// Missing @param for _newBridgeAgentFactory
338:     function addBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

/// Missing @param for _newBridgeAgentFactory
348:     function toggleBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

/// Missing @param for _bridgeAgent
355:     function toggleBridgeAgent(address _bridgeAgent) external override requiresCoreRouter {

/// Missing @param for _token
/// Missing @param for _minimumReservesRatio
362:     function addStrategyToken(address _token, uint256 _minimumReservesRatio) external override requiresCoreRouter {

/// Missing @param for _token
375:     function toggleStrategyToken(address _token) external override requiresCoreRouter {

/// Missing @param for _portStrategy
/// Missing @param for _token
/// Missing @param for _dailyManagementLimit
382:     function addPortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit)
             external
             override
             requiresCoreRouter
         {

/// Missing @param for _portStrategy
/// Missing @param for _token
396:     function togglePortStrategy(address _portStrategy, address _token) external override requiresCoreRouter {

/// Missing @param for _portStrategy
/// Missing @param for _token
/// Missing @param for _dailyManagementLimit
403:     function updatePortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit)
             external
             override
             requiresCoreRouter
         {

/// Missing @param for _coreBranchRouter
/// Missing @param for _coreBranchBridgeAgent
414:     function setCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent)
             external
             override
             requiresCoreRouter
         {

/// Missing @param for _strategyTokenDebt
435:     function _excessReserves(uint256 _strategyTokenDebt, address _token) internal view returns (uint256) {

/// Missing @param for _strategyTokenDebt
/// Missing @param for currBalance
449:     function _reservesLacking(uint256 _strategyTokenDebt, address _token, uint256 currBalance)
             internal
             view
             returns (uint256)
         {

```
[#L144](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L144) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L167) [#L188](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L188) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L226) [#L237](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L237) [#L246](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L246) [#L277](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L277) [#L288](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L288) [#L319](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L319) [#L331](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L331) [#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L338) [#L348](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L348) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L355) [#L362](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L362) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L375) [#L382](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L382) [#L396](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L396) [#L403](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L403) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L414) [#L435](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L435) [#L449](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L449) 

```solidity
File: src/CoreBranchRouter.sol

/// Missing @param for _params
86:     function executeNoSettlement(bytes calldata _params) external payable virtual override requiresAgentExecutor {

/// Missing @param for _decimals
166:     function _receiveAddGlobalToken(
             address _globalAddress,
             string memory _name,
             string memory _symbol,
             uint8 _decimals,
             address _refundee,
             GasParams memory _gParams
         ) internal {

```
[#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L86) [#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L166) 

```solidity
File: src/CoreRootRouter.sol

/// Missing @param for _bridgeAgentAddress
/// Missing @param for _hTokenFactory
83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

/// Missing @param for _rootBridgeAgent
103:     function addBranchToBridgeAgent(
             address _rootBridgeAgent,
             address _branchBridgeAgentFactory,
             address _newBranchRouter,
             address _refundee,
             uint16 _dstChainId,
             GasParams[2] calldata _gParams
         ) external payable {

/// Missing @param for _encodedData
/// Missing @param for _srcChainId
297:     function executeResponse(bytes calldata _encodedData, uint16 _srcChainId)
             external
             payable
             override
             requiresExecutor
         {

/// Missing @param for _encodedData
332:     function execute(bytes calldata _encodedData, uint16) external payable override requiresExecutor {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) [#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L103) [#L297](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L297) [#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L332) 

```solidity
File: src/MulticallRootRouter.sol

/// Missing @param for encodedData
137:     function execute(bytes calldata encodedData, uint16) external payable override lock requiresExecutor {

/// Missing @param for encodedData
/// Missing @param for userAccount
223:     function executeSigned(bytes calldata encodedData, address userAccount, uint16)
             external
             payable
             override
             lock
             requiresExecutor
         {

/// Missing @param for encodedData
/// Missing @param for userAccount
312:     function executeSignedDepositSingle(bytes calldata encodedData, DepositParams calldata, address userAccount, uint16)
             external
             payable
             override
             requiresExecutor
             lock
         {

/// Missing @param for encodedData
/// Missing @param for userAccount
401:     function executeSignedDepositMultiple(
             bytes calldata encodedData,
             DepositMultipleParams calldata,
             address userAccount,
             uint16
         ) external payable override requiresExecutor lock {

/// Missing @param for gasParams
508:     function _approveAndCallOut(
             address refundee,
             address recipient,
             address outputToken,
             uint256 amountOut,
             uint256 depositOut,
             uint16 dstChainId,
             GasParams memory gasParams
         ) internal virtual {

/// Missing @param for dstChainId
/// Missing @param for gasParams
544:     function _approveMultipleAndCallOut(
             address refundee,
             address recipient,
             address[] memory outputTokens,
             uint256[] memory amountsOut,
             uint256[] memory depositsOut,
             uint16 dstChainId,
             GasParams memory gasParams
         ) internal virtual {

/// Missing @param for data
581:     function _decode(bytes calldata data) internal pure virtual returns (bytes memory) {

```
[#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L137) [#L223](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L223) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L312) [#L401](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L401) [#L508](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L508) [#L544](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L544) [#L581](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L581) 

```solidity
File: src/MulticallRootRouterLibZip.sol

/// Missing @param for _localChainId
/// Missing @param for _localPortAddress
/// Missing @param for _multicallAddress
29:     constructor(uint256 _localChainId, address _localPortAddress, address _multicallAddress)
            MulticallRootRouter(_localChainId, _localPortAddress, _multicallAddress)
        {}

/// Missing @param for data
37:     function _decode(bytes calldata data) internal pure override returns (bytes memory) {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L29) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L37) 

```solidity
File: src/RootBridgeAgent.sol

/// Missing @param for _settlementNonce
135:     function getSettlementEntry(uint32 _settlementNonce) external view override returns (Settlement memory) {

/// Missing @param for _gasLimit
/// Missing @param for _remoteBranchExecutionGas
/// Missing @param for _payload
/// Missing @param for _dstChainId
140:     function getFeeEstimate(
             uint256 _gasLimit,
             uint256 _remoteBranchExecutionGas,
             bytes calldata _payload,
             uint16 _dstChainId
         ) external view returns (uint256 _fee) {

/// Missing @param for _refundee
/// Missing @param for _recipient
/// Missing @param for _dstChainId
/// Missing @param for _params
/// Missing @param for _gParams
160:     function callOut(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             GasParams calldata _gParams
         ) external payable override lock requiresRouter {

/// Missing @param for _refundee
/// Missing @param for _recipient
/// Missing @param for _dstChainId
/// Missing @param for _params
/// Missing @param for _sParams
/// Missing @param for _gParams
/// Missing @param for _hasFallbackToggled
175:     function callOutAndBridge(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             SettlementInput calldata _sParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock requiresRouter {

/// Missing @param for _refundee
/// Missing @param for _recipient
/// Missing @param for _dstChainId
/// Missing @param for _params
/// Missing @param for _sParams
/// Missing @param for _gParams
/// Missing @param for _hasFallbackToggled
202:     function callOutAndBridgeMultiple(
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes calldata _params,
             SettlementMultipleInput calldata _sParams,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock requiresRouter {

/// Missing @param for _settlementNonce
/// Missing @param for _recipient
/// Missing @param for _params
/// Missing @param for _gParams
/// Missing @param for _hasFallbackToggled
233:     function retrySettlement(
             uint32 _settlementNonce,
             address _recipient,
             bytes calldata _params,
             GasParams calldata _gParams,
             bool _hasFallbackToggled
         ) external payable override lock {

/// Missing @param for _settlementNonce
/// Missing @param for _gParams
274:     function retrieveSettlement(uint32 _settlementNonce, GasParams calldata _gParams) external payable lock {

/// Missing @param for _settlementNonce
299:     function redeemSettlement(uint32 _settlementNonce) external override lock {

/// Missing @param for _recipient
/// Missing @param for _dParams
/// Missing @param for _srcChainId
351:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId)
             public
             override
             requiresAgentExecutor
         {

/// Missing @param for _recipient
/// Missing @param for _dParams
/// Missing @param for _srcChainId
387:     function bridgeInMultiple(address _recipient, DepositMultipleParams calldata _dParams, uint256 _srcChainId)
             external
             override
             requiresAgentExecutor
         {

/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
/// Missing @param for _payload
423:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64, bytes calldata _payload) public {

/// Missing @param for _endpoint
/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
/// Missing @param for _payload
434:     function lzReceiveNonBlocking(
             address _endpoint,
             uint16 _srcChainId,
             bytes calldata _srcAddress,
             bytes calldata _payload
         ) public override requiresEndpoint(_endpoint, _srcChainId, _srcAddress) {

/// Missing @param for _value
856:     function _performRetrySettlementCall(
             bool _hasFallbackToggled,
             address[] memory _hTokens,
             address[] memory _tokens,
             uint256[] memory _amounts,
             uint256[] memory _deposits,
             bytes memory _params,
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             GasParams memory _gParams,
             uint256 _value
         ) internal {

/// Missing @param for _refundee
938:     function _performFallbackCall(address payable _refundee, uint32 _depositNonce, uint16 _dstChainId) internal {

/// Missing @param for _branchChainId
1170:     function approveBranchBridgeAgent(uint256 _branchChainId) external override requiresManager {

/// Missing @param for _newBranchBridgeAgent
/// Missing @param for _branchChainId
1176:     function syncBranchBridgeAgent(address _newBranchBridgeAgent, uint256 _branchChainId)
              external
              override
              requiresPort
          {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L135) [#L140](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L140) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L160) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L175) [#L202](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L202) [#L233](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L233) [#L274](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L274) [#L299](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L299) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L351) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L387) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L423) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L434) [#L856](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L856) [#L938](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L938) [#L1170](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1170) [#L1176](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1176) 

```solidity
File: src/RootBridgeAgentExecutor.sol

/// Missing @param for _rootBridgeAgent
14:     function deploy(address _rootBridgeAgent) external returns (address) {

/// Missing @param for _recipient
243:     function _bridgeIn(address _recipient, DepositParams memory _dParams, uint16 _srcChainId) internal {

/// Missing @param for _recipient
268:     function _bridgeInMultiple(address _recipient, bytes calldata _dParams, uint16 _srcChainId)
             internal
             returns (DepositMultipleParams memory dParams)
         {

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L14) [#L243](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L243) [#L268](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L268) 

```solidity
File: src/RootPort.sol

/// Missing @param for _localAddress
/// Missing @param for _srcChainId
/// Missing @param for _dstChainId
175:     function getLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             external
             view
             override
             returns (address)
         {

/// Missing @param for _globalAddress
/// Missing @param for _srcChainId
200:     function getUnderlyingTokenFromGlobal(address _globalAddress, uint256 _srcChainId)
             external
             view
             override
             returns (address)
         {

/// Missing @param for _globalAddress
/// Missing @param for _srcChainId
211:     function isGlobalToken(address _globalAddress, uint256 _srcChainId) external view override returns (bool) {

/// Missing @param for _localAddress
/// Missing @param for _srcChainId
216:     function isLocalToken(address _localAddress, uint256 _srcChainId) external view override returns (bool) {

/// Missing @param for _localAddress
/// Missing @param for _srcChainId
/// Missing @param for _dstChainId
221:     function isLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             external
             view
             returns (bool)
         {

/// Missing @param for _underlyingToken
/// Missing @param for _srcChainId
230:     function isUnderlyingToken(address _underlyingToken, uint256 _srcChainId) external view override returns (bool) {

/// Missing @param for _globalAddress
/// Missing @param for _localAddress
/// Missing @param for _underlyingAddress
/// Missing @param for _srcChainId
239:     function setAddresses(
             address _globalAddress,
             address _localAddress,
             address _underlyingAddress,
             uint256 _srcChainId
         ) external override requiresCoreRootRouter {

/// Missing @param for _globalAddress
/// Missing @param for _localAddress
/// Missing @param for _srcChainId
259:     function setLocalAddress(address _globalAddress, address _localAddress, uint256 _srcChainId)
             external
             override
             requiresCoreRootRouter
         {

/// Missing @param for _recipient
/// Missing @param for _hToken
/// Missing @param for _amount
/// Missing @param for _deposit
/// Missing @param for _srcChainId
277:     function bridgeToRoot(address _recipient, address _hToken, uint256 _amount, uint256 _deposit, uint256 _srcChainId)
             external
             override
             requiresBridgeAgent
         {

/// Missing @param for _from
/// Missing @param for _hToken
/// Missing @param for _amount
294:     function bridgeToRootFromLocalBranch(address _from, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing @param for _to
/// Missing @param for _hToken
/// Missing @param for _amount
304:     function bridgeToLocalBranchFromRoot(address _to, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing @param for _from
/// Missing @param for _hToken
/// Missing @param for _amount
/// Missing @param for _srcChainId
315:     function burn(address _from, address _hToken, uint256 _amount, uint256 _srcChainId)
             external
             override
             requiresBridgeAgent
         {

/// Missing @param for _from
/// Missing @param for _hToken
/// Missing @param for _amount
325:     function burnFromLocalBranch(address _from, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing @param for _to
/// Missing @param for _hToken
/// Missing @param for _amount
336:     function mintToLocalBranch(address _to, address _hToken, uint256 _amount)
             external
             override
             requiresLocalBranchPort
         {

/// Missing @param for _user
350:     function fetchVirtualAccount(address _user) external override returns (VirtualAccount account) {

/// Missing @param for _userAccount
/// Missing @param for _router
369:     function toggleVirtualAccountApproved(VirtualAccount _userAccount, address _router)
             external
             override
             requiresBridgeAgent
         {

/// Missing @param for _manager
/// Missing @param for _bridgeAgent
382:     function addBridgeAgent(address _manager, address _bridgeAgent) external override requiresBridgeAgentFactory {

/// Missing @param for _newBranchBridgeAgent
/// Missing @param for _rootBridgeAgent
/// Missing @param for _branchChainId
393:     function syncBranchBridgeAgentWithRoot(
             address _newBranchBridgeAgent,
             address _rootBridgeAgent,
             uint256 _branchChainId
         ) external override requiresCoreRootRouter {

/// Missing @param for _bridgeAgent
414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

/// Missing @param for _bridgeAgentFactory
421:     function addBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

/// Missing @param for _bridgeAgentFactory
431:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

/// Missing @param for _coreBranchBridgeAgentAddress
/// Missing @param for _chainId
/// Missing @param for _wrappedGasTokenName
/// Missing @param for _wrappedGasTokenSymbol
/// Missing @param for _wrappedGasTokenDecimals
/// Missing @param for _newLocalBranchWrappedNativeTokenAddress
/// Missing @param for _newUnderlyingBranchWrappedNativeTokenAddress
438:     function addNewChain(
             address _coreBranchBridgeAgentAddress,
             uint256 _chainId,
             string memory _wrappedGasTokenName,
             string memory _wrappedGasTokenSymbol,
             uint8 _wrappedGasTokenDecimals,
             address _newLocalBranchWrappedNativeTokenAddress,
             address _newUnderlyingBranchWrappedNativeTokenAddress
         ) external override onlyOwner {

/// Missing @param for _ecoTokenGlobalAddress
483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

/// Missing @param for _coreRootRouter
/// Missing @param for _coreRootBridgeAgent
509:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external override onlyOwner {

/// Missing @param for _refundee
/// Missing @param for _coreBranchRouter
/// Missing @param for _coreBranchBridgeAgent
/// Missing @param for _dstChainId
/// Missing @param for _gParams
521:     function setCoreBranchRouter(
             address _refundee,
             address _coreBranchRouter,
             address _coreBranchBridgeAgent,
             uint16 _dstChainId,
             GasParams calldata _gParams
         ) external payable override onlyOwner {

/// Missing @param for _coreBranchRouter
/// Missing @param for _coreBranchBridgeAgent
/// Missing @param for _dstChainId
539:     function syncNewCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent, uint16 _dstChainId)
             external
             override
             onlyOwner
         {

```
[#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L175) [#L200](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L200) [#L211](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L211) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L216) [#L221](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L221) [#L230](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L230) [#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L239) [#L259](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L259) [#L277](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L277) [#L294](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L294) [#L304](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L304) [#L315](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L315) [#L325](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L325) [#L336](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L336) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L350) [#L369](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L369) [#L382](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L382) [#L393](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L393) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L421) [#L431](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L431) [#L438](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L438) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) [#L509](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L509) [#L521](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L521) [#L539](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L539) 

```solidity
File: src/VirtualAccount.sol

/// Missing @param for _amount
51:     function withdrawNative(uint256 _amount) external override requiresApprovedCaller {

/// Missing @param for _token
/// Missing @param for _amount
56:     function withdrawERC20(address _token, uint256 _amount) external override requiresApprovedCaller {

/// Missing @param for _token
/// Missing @param for _tokenId
61:     function withdrawERC721(address _token, uint256 _tokenId) external override requiresApprovedCaller {

/// Missing @param for calls
66:     function call(Call[] calldata calls) external override requiresApprovedCaller returns (bytes[] memory returnData) {

/// Missing @param for calls
85:     function payableCall(PayableCall[] calldata calls) public payable returns (bytes[] memory returnData) {

/// Missing @param for addr
147:     function isContract(address addr) internal view returns (bool) {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L51) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L56) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L61) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L66) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L85) [#L147](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L147) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

/// Missing @param for _rootBridgeAgentFactoryAddress
79:     function createBridgeAgent(
            address _newBranchRouterAddress,
            address _rootBridgeAgentAddress,
            address _rootBridgeAgentFactoryAddress
        ) external virtual override returns (address newBridgeAgent) {

```
[#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L79) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

/// Missing @param for _rootBridgeAgentFactoryAddress
115:     function createBridgeAgent(
             address _newBranchRouterAddress,
             address _rootBridgeAgentAddress,
             address _rootBridgeAgentFactoryAddress
         ) external virtual returns (address newBridgeAgent) {

```
[#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L115) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

/// Missing @param for _name
/// Missing @param for _symbol
/// Missing @param for _decimals
/// Missing @param for _addPrefix
96:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)
            external
            requiresCoreRouter
            returns (ERC20hTokenBranch newToken)
        {

```
[#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L96) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

/// Missing @param for recipient
312:     function clearTokens(bytes calldata sParams, address recipient)

```
[#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L312) 

```solidity
File: src/interfaces/IBranchPort.sol

/// Missing @param for _underlyingAddresses
/// Missing @param for _deposits
103:     function bridgeInMultiple(

/// Missing @param for _depositor
/// Missing @param for _underlyingAddress
118:     function bridgeOut(

/// Missing @param for _minimumReservesRatio
181:     function addStrategyToken(address _token, uint256 _minimumReservesRatio) external;

/// Missing @param for _token
/// Missing @param for _dailyManagementLimit
193:     function addPortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit) external;

/// Missing @param for _token
199:     function togglePortStrategy(address _portStrategy, address _token) external;

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L103) [#L118](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L118) [#L181](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L181) [#L193](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L193) [#L199](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L199) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

/// Missing @param for _dstChainId
/// Missing @param for _destination
/// Missing @param for _payload
/// Missing @param for _refundAddress
/// Missing @param for _zroPaymentAddress
/// Missing @param for _adapterParams
15:     function send(

/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
/// Missing @param for _dstAddress
/// Missing @param for _nonce
/// Missing @param for _gasLimit
/// Missing @param for _payload
31:     function receivePayload(

/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
43:     function getInboundNonce(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (uint64);

/// Missing @param for _dstChainId
/// Missing @param for _srcAddress
47:     function getOutboundNonce(uint16 _dstChainId, address _srcAddress) external view returns (uint64);

/// Missing @param for _dstChainId
/// Missing @param for _userApplication
/// Missing @param for _payload
/// Missing @param for _payInZRO
/// Missing @param for _adapterParam
55:     function estimateFees(

/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
/// Missing @param for _payload
70:     function retryPayload(uint16 _srcChainId, bytes calldata _srcAddress, bytes calldata _payload) external;

/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
75:     function hasStoredPayload(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (bool);

/// Missing @param for _userApplication
79:     function getSendLibraryAddress(address _userApplication) external view returns (address);

/// Missing @param for _userApplication
83:     function getReceiveLibraryAddress(address _userApplication) external view returns (address);

/// Missing @param for _version
/// Missing @param for _chainId
/// Missing @param for _userApplication
/// Missing @param for _configType
98:     function getConfig(uint16 _version, uint16 _chainId, address _userApplication, uint256 _configType)

/// Missing @param for _userApplication
105:     function getSendVersion(address _userApplication) external view returns (uint16);

/// Missing @param for _userApplication
109:     function getReceiveVersion(address _userApplication) external view returns (uint16);

```
[#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L15) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L31) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L43) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L47) [#L55](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L55) [#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L70) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L75) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L79) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L83) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L98) [#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L105) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L109) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
/// Missing @param for _nonce
/// Missing @param for _payload
11:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64 _nonce, bytes calldata _payload) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L11) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

/// Missing @param for _version
/// Missing @param for _chainId
/// Missing @param for _configType
/// Missing @param for _config
11:     function setConfig(uint16 _version, uint16 _chainId, uint256 _configType, bytes calldata _config) external;

/// Missing @param for _version
15:     function setSendVersion(uint16 _version) external;

/// Missing @param for _version
19:     function setReceiveVersion(uint16 _version) external;

/// Missing @param for _srcChainId
/// Missing @param for _srcAddress
24:     function forceResumeReceive(uint16 _srcChainId, bytes calldata _srcAddress) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L11) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L15) [#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L19) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L24) 

```solidity
File: src/interfaces/IMulticall2.sol

/// Missing @param for calls
20:     function aggregate(Call[] memory calls) external returns (uint256 blockNumber, bytes[] memory returnData);

```
[#L20](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L20) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

/// Missing @param for _refundee
168:     function callOut(

```
[#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L168) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

/// Missing @param for newRootRouterAddress
16:     function createBridgeAgent(address newRootRouterAddress) external returns (address newBridgeAgent);

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L16) 

```solidity
File: src/interfaces/IRootPort.sol

/// Missing @param for _refundee
/// Missing @param for _coreBranchRouter
/// Missing @param for _coreBranchBridgeAgent
/// Missing @param for _dstChainId
/// Missing @param for _gParams
13:     function setCoreBranch(

/// Missing @param for _underlyingAddress
/// Missing @param for _srcChainId
238:     function setAddresses(

/// Missing @param for _srcChainId
251:     function setLocalAddress(address _globalAddress, address _localAddress, uint256 _srcChainId) external;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L13) [#L238](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L238) [#L251](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L251) 

```solidity
File: src/token/ERC20hTokenBranch.sol

/// Missing @param for chainName
/// Missing @param for chainSymbol
/// Missing @param for _name
/// Missing @param for _symbol
/// Missing @param for _decimals
/// Missing @param for _owner
13:     constructor(
            string memory chainName,
            string memory chainSymbol,
            string memory _name,
            string memory _symbol,
            uint8 _decimals,
            address _owner
        ) ERC20(string(string.concat(chainName, _name)), string(string.concat(chainSymbol, _symbol)), _decimals) {

/// Missing @param for account
/// Missing @param for amount
29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

/// Missing @param for amount
35:     function burn(uint256 amount) public override onlyOwner {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L13) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L35) 

</details>

---

<a name="NC-26"></a> 
### [NC-26] NatSpec `@return` is missing
It is recommended that Solidity contracts are fully annotated using NatSpec

<details>
<summary>
There are <b>63</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

11:     function deploy(uint16 _localChainId, address _daoAddress, address _localRouterAddress, address _localPortAddress)
            external
            returns (ArbitrumBranchBridgeAgent)
        {

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L11) 

```solidity
File: src/BaseBranchRouter.sol

74:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

```
[#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L74) 

```solidity
File: src/BranchBridgeAgent.sol

24:     function deploy(
            uint16 _rootChainId,
            uint16 _localChainId,
            address _rootBridgeAgentAddress,
            address _lzEndpointAddress,
            address _localRouterAddress,
            address _localPortAddress
        ) external returns (BranchBridgeAgent) {

156:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

161:     function getFeeEstimate(uint256 _gasLimit, uint256 _remoteBranchExecutionGas, bytes calldata _payload)
             external
             view
             returns (uint256 _fee)
         {

494:     function clearTokens(bytes calldata _sParams, address _recipient)
             external
             override
             requiresAgentExecutor
             returns (SettlementMultipleParams memory)
         {

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L24) [#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L156) [#L161](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L161) [#L494](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L494) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

16:     function deploy() external returns (address) {

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L16) 

```solidity
File: src/MulticallRootRouter.sol

488:     function _multicall(IMulticall.Call[] memory calls)
             internal
             returns (uint256 blockNumber, bytes[] memory returnData)
         {

581:     function _decode(bytes calldata data) internal pure virtual returns (bytes memory) {

```
[#L488](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L488) [#L581](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L581) 

```solidity
File: src/MulticallRootRouterLibZip.sol

37:     function _decode(bytes calldata data) internal pure override returns (bytes memory) {

```
[#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L37) 

```solidity
File: src/RootBridgeAgent.sol

135:     function getSettlementEntry(uint32 _settlementNonce) external view override returns (Settlement memory) {

140:     function getFeeEstimate(
             uint256 _gasLimit,
             uint256 _remoteBranchExecutionGas,
             bytes calldata _payload,
             uint16 _dstChainId
         ) external view returns (uint256 _fee) {

966:     function _createSettlement(
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes memory _params,
             address _globalAddress,
             uint256 _amount,
             uint256 _deposit,
             bool _hasFallbackToggled
         ) internal returns (bytes memory _payload) {

1045:     function _createSettlementMultiple(
              uint32 _settlementNonce,
              address payable _refundee,
              address _recipient,
              uint16 _dstChainId,
              address[] memory _globalAddresses,
              uint256[] memory _amounts,
              uint256[] memory _deposits,
              bytes memory _params,
              bool _hasFallbackToggled
          ) internal returns (bytes memory _payload) {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L135) [#L140](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L140) [#L966](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L966) [#L1045](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1045) 

```solidity
File: src/RootBridgeAgentExecutor.sol

14:     function deploy(address _rootBridgeAgent) external returns (address) {

268:     function _bridgeInMultiple(address _recipient, bytes calldata _dParams, uint16 _srcChainId)
             internal
             returns (DepositMultipleParams memory dParams)
         {

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L14) [#L268](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L268) 

```solidity
File: src/RootPort.sol

175:     function getLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             external
             view
             override
             returns (address)
         {

190:     function _getLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             internal
             view
             returns (address)
         {

200:     function getUnderlyingTokenFromGlobal(address _globalAddress, uint256 _srcChainId)
             external
             view
             override
             returns (address)
         {

211:     function isGlobalToken(address _globalAddress, uint256 _srcChainId) external view override returns (bool) {

216:     function isLocalToken(address _localAddress, uint256 _srcChainId) external view override returns (bool) {

221:     function isLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)
             external
             view
             returns (bool)
         {

230:     function isUnderlyingToken(address _underlyingToken, uint256 _srcChainId) external view override returns (bool) {

350:     function fetchVirtualAccount(address _user) external override returns (VirtualAccount account) {

359:     function addVirtualAccount(address _user) internal returns (VirtualAccount newAccount) {

```
[#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L175) [#L190](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L190) [#L200](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L200) [#L211](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L211) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L216) [#L221](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L221) [#L230](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L230) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L350) [#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L359) 

```solidity
File: src/VirtualAccount.sol

66:     function call(Call[] calldata calls) external override requiresApprovedCaller returns (bytes[] memory returnData) {

85:     function payableCall(PayableCall[] calldata calls) public payable returns (bytes[] memory returnData) {

119:     function onERC721Received(address, address, uint256, bytes calldata) external pure override returns (bytes4) {

124:     function onERC1155Received(address, address, uint256, uint256, bytes calldata)
             external
             pure
             override
             returns (bytes4)
         {

134:     function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata)
             external
             pure
             override
             returns (bytes4)
         {

147:     function isContract(address addr) internal view returns (bool) {

```
[#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L66) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L85) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L119) [#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L124) [#L134](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L134) [#L147](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L147) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

79:     function createBridgeAgent(
            address _newBranchRouterAddress,
            address _rootBridgeAgentAddress,
            address _rootBridgeAgentFactoryAddress
        ) external virtual override returns (address newBridgeAgent) {

```
[#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L79) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

115:     function createBridgeAgent(
             address _newBranchRouterAddress,
             address _rootBridgeAgentAddress,
             address _rootBridgeAgentFactoryAddress
         ) external virtual returns (address newBridgeAgent) {

```
[#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L115) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

96:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)
            external
            requiresCoreRouter
            returns (ERC20hTokenBranch newToken)
        {

```
[#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L96) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

76:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)
            external
            requiresCoreRouterOrPort
            returns (ERC20hTokenRoot newToken)
        {

```
[#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L76) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

109:     function getDepositEntry(uint32 depositNonce) external view returns (Deposit memory);

312:     function clearTokens(bytes calldata sParams, address recipient)

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L109) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L312) 

```solidity
File: src/interfaces/IBranchRouter.sol

27:     function localPortAddress() external view returns (address);

30:     function localBridgeAgentAddress() external view returns (address);

33:     function bridgeAgentExecutorAddress() external view returns (address);

79:     function getDepositEntry(uint32 depositNonce) external view returns (Deposit memory);

```
[#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L27) [#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L30) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L33) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L79) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L24) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L24) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

43:     function getInboundNonce(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (uint64);

47:     function getOutboundNonce(uint16 _dstChainId, address _srcAddress) external view returns (uint64);

55:     function estimateFees(

64:     function getChainId() external view returns (uint16);

75:     function hasStoredPayload(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (bool);

79:     function getSendLibraryAddress(address _userApplication) external view returns (address);

83:     function getReceiveLibraryAddress(address _userApplication) external view returns (address);

87:     function isSendingPayload() external view returns (bool);

91:     function isReceivingPayload() external view returns (bool);

98:     function getConfig(uint16 _version, uint16 _chainId, address _userApplication, uint256 _configType)

105:     function getSendVersion(address _userApplication) external view returns (uint16);

109:     function getReceiveVersion(address _userApplication) external view returns (uint16);

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L43) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L47) [#L55](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L55) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L64) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L75) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L79) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L83) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L87) [#L91](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L91) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L98) [#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L105) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L109) 

```solidity
File: src/interfaces/IMulticall2.sol

20:     function aggregate(Call[] memory calls) external returns (uint256 blockNumber, bytes[] memory returnData);

```
[#L20](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L20) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

111:     function getSettlementEntry(uint32 _settlementNonce) external view returns (Settlement memory);

```
[#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L111) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

16:     function createBridgeAgent(address newRootRouterAddress) external returns (address newBridgeAgent);

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L16) 

```solidity
File: src/interfaces/IRootPort.sol

11:     function bridgeAgentAddress() external view returns (address);

12:     function hTokenFactoryAddress() external view returns (address);

261:     function fetchVirtualAccount(address _user) external returns (VirtualAccount account);

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L11) [#L12](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L12) [#L261](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L261) 

```solidity
File: src/token/ERC20hTokenBranch.sol

29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) 

```solidity
File: src/token/ERC20hTokenRoot.sol

57:     function mint(address to, uint256 amount, uint256 chainId) external onlyOwner returns (bool) {

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L57) 

</details>

---

<a name="NC-27"></a> 
### [NC-27] There is no need to initialize variables with 0
Since the variables are automatically set to 0 when created, it is redundant to initialize it with 0 again.

<details>
<summary>
There are <b>17</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

192:         for (uint256 i = 0; i < _hTokens.length;) {

```
[#L192](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L192) 

```solidity
File: src/BranchBridgeAgent.sol

447:         for (uint256 i = 0; i < deposit.tokens.length;) {

513:         for (uint256 i = 0; i < numOfAssets;) {

```
[#L447](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L447) [#L513](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L513) 

```solidity
File: src/BranchPort.sol

257:         for (uint256 i = 0; i < length;) {

305:         for (uint256 i = 0; i < length;) {

```
[#L257](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L257) [#L305](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L305) 

```solidity
File: src/MulticallRootRouter.sol

278:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

367:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

455:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

557:         for (uint256 i = 0; i < outputTokens.length;) {

```
[#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L278) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L367) [#L455](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L455) [#L557](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L557) 

```solidity
File: src/RootBridgeAgent.sol

318:         for (uint256 i = 0; i < settlement.hTokens.length;) {

399:         for (uint256 i = 0; i < length;) {

1070:         for (uint256 i = 0; i < hTokens.length;) {

```
[#L318](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L318) [#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L399) [#L1070](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1070) 

```solidity
File: src/RootBridgeAgentExecutor.sol

281:         for (uint256 i = 0; i < uint256(uint8(numOfAssets));) {

```
[#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L281) 

```solidity
File: src/VirtualAccount.sol

70:         for (uint256 i = 0; i < length;) {

90:         for (uint256 i = 0; i < length;) {

```
[#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L70) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L90) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

23:     uint8 internal constant STATUS_SUCCESS = 0;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) 

</details>

---

<a name="NC-28"></a> 
### [NC-28] Put all system-wide constants in one file
Putting all the system-wide constants in a single file improves code readability, makes it easier to understand the basic configuration and limitations of the system, and makes maintenance easier.

<details>
<summary>
There are <b>22</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

97:     uint256 internal constant DIVISIONER = 1e4;

98:     uint256 internal constant MIN_RESERVE_RATIO = 3e3;

```
[#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L98) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

15:     uint8 internal constant STATUS_DONE = 1;

17:     uint8 internal constant STATUS_RETRIEVE = 2;

21:     uint8 internal constant STATUS_FAILED = 1;

23:     uint8 internal constant STATUS_SUCCESS = 0;

27:     uint256 internal constant PARAMS_START = 1;

29:     uint256 internal constant PARAMS_START_SIGNED = 21;

31:     uint256 internal constant PARAMS_TKN_START = 5;

33:     uint256 internal constant PARAMS_TKN_START_SIGNED = 25;

35:     uint256 internal constant PARAMS_ENTRY_SIZE = 32;

37:     uint256 internal constant PARAMS_ADDRESS_SIZE = 20;

39:     uint256 internal constant PARAMS_TKN_SET_SIZE = 109;

41:     uint256 internal constant PARAMS_TKN_SET_SIZE_MULTIPLE = 128;

43:     uint256 internal constant ADDRESS_END_OFFSET = 12;

45:     uint256 internal constant PARAMS_AMT_OFFSET = 64;

47:     uint256 internal constant PARAMS_DEPOSIT_OFFSET = 96;

49:     uint256 internal constant PARAMS_END_OFFSET = 6;

51:     uint256 internal constant PARAMS_END_SIGNED_OFFSET = 26;

53:     uint256 internal constant PARAMS_SETTLEMENT_OFFSET = 129;

57:     uint256 internal constant MAX_TOKENS_LENGTH = 255;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L15) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L17) [#L21](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L21) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) [#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L27) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L29) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L31) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L33) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L35) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L37) [#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L39) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L41) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L43) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L45) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L47) [#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L49) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L51) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L53) [#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L57) 

</details>

---

<a name="NC-29"></a> 
### [NC-29] State variables should include comments
Consider adding some comments on critical state variables to explain what they are supposed to do: this will help for future code reviews.

<details>
<summary>
There are <b>77</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

105:         bytes calldata _params,

```
[#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L105) 

```solidity
File: src/BranchPort.sol

98:     uint256 internal constant MIN_RESERVE_RATIO = 3e3;

```
[#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L98) 

```solidity
File: src/CoreRootRouter.sol

157:         address _rootBridgeAgentFactory,

158:         address _branchBridgeAgentFactory,

159:         address _refundee,

160:         uint16 _dstChainId,

```
[#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L157) [#L158](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L158) [#L159](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L159) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L160) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

15:     uint8 internal constant STATUS_DONE = 1;

17:     uint8 internal constant STATUS_RETRIEVE = 2;

23:     uint8 internal constant STATUS_SUCCESS = 0;

29:     uint256 internal constant PARAMS_START_SIGNED = 21;

31:     uint256 internal constant PARAMS_TKN_START = 5;

33:     uint256 internal constant PARAMS_TKN_START_SIGNED = 25;

35:     uint256 internal constant PARAMS_ENTRY_SIZE = 32;

37:     uint256 internal constant PARAMS_ADDRESS_SIZE = 20;

39:     uint256 internal constant PARAMS_TKN_SET_SIZE = 109;

41:     uint256 internal constant PARAMS_TKN_SET_SIZE_MULTIPLE = 128;

43:     uint256 internal constant ADDRESS_END_OFFSET = 12;

45:     uint256 internal constant PARAMS_AMT_OFFSET = 64;

47:     uint256 internal constant PARAMS_DEPOSIT_OFFSET = 96;

49:     uint256 internal constant PARAMS_END_OFFSET = 6;

51:     uint256 internal constant PARAMS_END_SIGNED_OFFSET = 26;

53:     uint256 internal constant PARAMS_SETTLEMENT_OFFSET = 129;

```
[#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L15) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L17) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L29) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L31) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L33) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L35) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L37) [#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L39) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L41) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L43) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L45) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L47) [#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L49) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L51) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L53) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

9:     uint256 gasLimit; // gas allocated for the cross-chain call.

10:     uint256 remoteBranchExecutionGas; //gas allocated for remote branch execution. Must be lower than `gasLimit`.

14:     uint8 status;

15:     address owner;

16:     address[] hTokens;

17:     address[] tokens;

18:     uint256[] amounts;

19:     uint256[] deposits;

25:     address token; //Input Native / underlying Token Address.

26:     uint256 amount; //Amount of Local hTokens deposited for interaction.

27:     uint256 deposit; //Amount of native tokens deposited for interaction.

33:     address[] tokens; //Input Native / underlying Token Address.

34:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

35:     uint256[] deposits; //Amount of native tokens deposited for interaction.

41:     uint32 depositNonce; //Deposit nonce.

42:     address[] hTokens; //Input Local hTokens Address.

43:     address[] tokens; //Input Native / underlying Token Address.

44:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

45:     uint256[] deposits; //Amount of native tokens deposited for interaction.

51:     address hToken; //Input Local hTokens Address.

52:     address token; //Input Native / underlying Token Address.

53:     uint256 amount; //Amount of Local hTokens deposited for interaction.

54:     uint256 deposit; //Amount of native tokens deposited for interaction.

58:     uint16 dstChainId; //Destination chain for interaction.

59:     uint80 status; //Status of the settlement

60:     address owner; //Owner of the settlement

61:     address recipient; //Recipient of the settlement.

62:     address[] hTokens; //Input Local hTokens Addresses.

63:     address[] tokens; //Input Native / underlying Token Addresses.

64:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

65:     uint256[] deposits; //Amount of native tokens deposited for interaction.

69:     address globalAddress; //Input Global hTokens Address.

70:     uint256 amount; //Amount of Local hTokens deposited for interaction.

71:     uint256 deposit; //Amount of native tokens deposited for interaction.

75:     address[] globalAddresses; //Input Global hTokens Addresses.

76:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

77:     uint256[] deposits; //Amount of native tokens deposited for interaction.

81:     uint32 settlementNonce; // Settlement nonce.

82:     address recipient; // Recipient of the settlement.

83:     address hToken; // Input Local hTokens Address.

84:     address token; // Input Native / underlying Token Address.

85:     uint256 amount; // Amount of Local hTokens deposited for interaction.

86:     uint256 deposit; // Amount of native tokens deposited for interaction.

90:     uint8 numberOfAssets; // Number of assets to deposit.

91:     address recipient; // Recipient of the settlement.

92:     uint32 settlementNonce; // Settlement nonce.

93:     address[] hTokens; // Input Local hTokens Addresses.

94:     address[] tokens; // Input Native / underlying Token Addresses.

95:     uint256[] amounts; // Amount of Local hTokens deposited for interaction.

96:     uint256[] deposits; // Amount of native tokens deposited for interaction.

```
[#L9](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L9) [#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L10) [#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L14) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L15) [#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L16) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L17) [#L18](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L18) [#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L19) [#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L25) [#L26](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L26) [#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L27) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L33) [#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L34) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L35) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L41) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L42) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L43) [#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L44) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L45) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L51) [#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L52) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L53) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L54) [#L58](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L58) [#L59](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L59) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L60) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L61) [#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L62) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L63) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L64) [#L65](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L65) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L69) [#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L70) [#L71](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L71) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L75) [#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L76) [#L77](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L77) [#L81](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L81) [#L82](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L82) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L83) [#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L84) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L85) [#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L86) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L90) [#L91](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L91) [#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L92) [#L93](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L93) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L94) [#L95](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L95) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L96) 

```solidity
File: src/interfaces/IVirtualAccount.sol

8:     address target;

9:     bytes callData;

14:     address target;

15:     bytes callData;

16:     uint256 value;

```
[#L8](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L8) [#L9](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L9) [#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L14) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L15) [#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L16) 

</details>

---

<a name="NC-30"></a> 
### [NC-30] Contract declarations should have NatSpec `@title` annotations
Some contract definitions have an incomplete NatSpec: add a `@title` notation to describe the contract to improve the code documentation.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

10: library DeployArbitrumBranchBridgeAgent {

```
[#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L10) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

7: interface ILayerZeroEndpoint is ILayerZeroUserApplicationConfig {

```
[#L7](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L7) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

5: interface ILayerZeroReceiver {

```
[#L5](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L5) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

5: interface ILayerZeroUserApplicationConfig {

```
[#L5](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L5) 

</details>

---

<a name="NC-31"></a> 
### [NC-31] Lines are too long
The [solidity style guide](https://docs.soliditylang.org/en/v0.8.17/style-guide.html#maximum-line-length) recommends a maximum line length of 120 characters. Lines of code that are longer than 120 should be wrapped.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

60:         address _globalToken = IRootPort(_rootPortAddress).getLocalTokenFromUnderlying(_underlyingAddress, localChainId);

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L60) 

```solidity
File: src/BranchBridgeAgent.sol

548:                             PARAMS_TKN_START + PARAMS_AMT_OFFSET * numOfAssets + PARAMS_ENTRY_SIZE * currentIterationOffset

```
[#L548](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L548) 

</details>

---

<a name="NC-32"></a> 
### [NC-32] Unused errors
The following `error`s are defined but not used. It is recommended to check the code for logical omissions that cause them not to be used. If it's determined that they are not needed anywhere, it's best to remove them from the codebase to improve code clarity and minimize confusion. Note that there may be cases where an error appears to be used because it has multiple definitions in different files. In such cases, the definitions should be moved to a separate file.

<details>
<summary>
There are <b>84</b> instances (click to show):
</summary>

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

45:     error UnknownGlobalToken();

46:     error UnknownUnderlyingToken();

```
[#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L45) [#L46](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L46) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

339:     error UnknownFlag();

340:     error ExecutionFailure();

342:     error LayerZeroUnauthorizedCaller();

343:     error LayerZeroUnauthorizedEndpoint();

345:     error AlreadyExecutedTransaction();

347:     error InvalidInput();

348:     error InsufficientGas();

350:     error NotDepositOwner();

351:     error DepositRetryUnavailableUseCallout();

352:     error DepositRedeemUnavailable();

354:     error UnrecognizedRouter();

355:     error UnrecognizedBridgeAgentExecutor();

```
[#L339](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L339) [#L340](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L340) [#L342](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L342) [#L343](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L343) [#L345](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L345) [#L347](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L347) [#L348](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L348) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L350) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L351) [#L352](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L352) [#L354](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L354) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L355) 

```solidity
File: src/interfaces/IBranchPort.sol

245:     error AlreadyAddedBridgeAgent();

246:     error AlreadyAddedBridgeAgentFactory();

247:     error InvalidMinimumReservesRatio();

248:     error InvalidInputArrays();

249:     error InsufficientReserves();

250:     error UnrecognizedCore();

251:     error UnrecognizedBridgeAgent();

252:     error UnrecognizedBridgeAgentFactory();

253:     error UnrecognizedPortStrategy();

254:     error UnrecognizedStrategyToken();

255:     error NotEnoughDebtToRepay();

```
[#L245](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L245) [#L246](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L246) [#L247](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L247) [#L248](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L248) [#L249](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L249) [#L250](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L250) [#L251](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L251) [#L252](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L252) [#L253](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L253) [#L254](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L254) [#L255](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L255) 

```solidity
File: src/interfaces/IBranchRouter.sol

113:     error UnrecognizedFunctionId();

115:     error UnrecognizedBridgeAgentExecutor();

```
[#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L113) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L115) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

53:     error UnrecognizedBridgeAgent();

54:     error UnrecognizedBridgeAgentFactory();

```
[#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L53) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L54) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

32:     error UnrecognizedCoreRouter();

34:     error UnrecognizedPort();

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L32) [#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L34) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

57:     error UnrecognizedPort();

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L57) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

32:     error UnrecognizedCoreRouterOrPort();

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L32) 

```solidity
File: src/interfaces/IPortStrategy.sol

29:     error UnrecognizedPort();

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L29) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

344:     error ExecutionFailure();

345:     error GasErrorOrRepeatedTx();

346:     error AlreadyExecutedTransaction();

347:     error UnknownFlag();

349:     error NotDao();

351:     error LayerZeroUnauthorizedEndpoint();

352:     error LayerZeroUnauthorizedCaller();

354:     error AlreadyAddedBridgeAgent();

355:     error UnrecognizedExecutor();

356:     error UnrecognizedPort();

357:     error UnrecognizedBridgeAgent();

358:     error UnrecognizedLocalBridgeAgent();

359:     error UnrecognizedBridgeAgentManager();

360:     error UnrecognizedRouter();

362:     error UnrecognizedUnderlyingAddress();

363:     error UnrecognizedLocalAddress();

365:     error SettlementRetryUnavailable();

366:     error SettlementRetryUnavailableUseCallout();

367:     error SettlementRedeemUnavailable();

368:     error SettlementRetrieveUnavailable();

369:     error NotSettlementOwner();

371:     error InsufficientBalanceForSettlement();

372:     error InsufficientGasForFees();

373:     error InvalidInputParams();

374:     error InvalidInputParamsLength();

376:     error CallerIsNotPool();

377:     error AmountsAreZero();

```
[#L344](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L344) [#L345](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L345) [#L346](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L346) [#L347](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L347) [#L349](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L349) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L351) [#L352](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L352) [#L354](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L354) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L355) [#L356](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L356) [#L357](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L357) [#L358](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L358) [#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L359) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L360) [#L362](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L362) [#L363](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L363) [#L365](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L365) [#L366](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L366) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L367) [#L368](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L368) [#L369](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L369) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L371) [#L372](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L372) [#L373](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L373) [#L374](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L374) [#L376](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L376) [#L377](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L377) 

```solidity
File: src/interfaces/IRootPort.sol

399:     error InvalidGlobalAddress();

400:     error InvalidLocalAddress();

401:     error InvalidUnderlyingAddress();

403:     error InvalidUserAddress();

405:     error InvalidCoreRootRouter();

406:     error InvalidCoreRootBridgeAgent();

407:     error InvalidCoreBranchRouter();

408:     error InvalidCoreBrancBridgeAgent();

410:     error UnrecognizedBridgeAgentFactory();

411:     error UnrecognizedBridgeAgent();

413:     error UnrecognizedToken();

414:     error UnableToMint();

416:     error AlreadyAddedChain();

417:     error AlreadyAddedEcosystemToken();

419:     error AlreadyAddedBridgeAgent();

420:     error AlreadyAddedBridgeAgentFactory();

421:     error BridgeAgentNotAllowed();

422:     error UnrecognizedCoreRootRouter();

423:     error UnrecognizedLocalBranchPort();

```
[#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L399) [#L400](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L400) [#L401](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L401) [#L403](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L403) [#L405](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L405) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L406) [#L407](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L407) [#L408](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L408) [#L410](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L410) [#L411](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L411) [#L413](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L413) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L414) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L416) [#L417](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L417) [#L419](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L419) [#L420](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L420) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L421) [#L422](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L422) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L423) 

```solidity
File: src/interfaces/IRootRouter.sol

97:     error UnrecognizedFunctionId();

98:     error UnrecognizedBridgeAgentExecutor();

```
[#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L98) 

```solidity
File: src/interfaces/IVirtualAccount.sol

79:     error CallFailed();

81:     error UnauthorizedCaller();

```
[#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L79) [#L81](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L81) 

</details>

---

<a name="NC-33"></a> 
### [NC-33] Unused contract variables
The following state variables are defined but not used. It is recommended to check the code for logical omissions that cause them not to be used. If it's determined that they are not needed anywhere, it's best to remove them from the codebase to improve code clarity and minimize confusion.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

98:     uint256 internal constant MIN_RESERVE_RATIO = 3e3;

```
[#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L98) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

49:     uint256 internal constant PARAMS_END_OFFSET = 6;

```
[#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L49) 

</details>

---

<a name="NC-34"></a> 
### [NC-34] Consider using `delete` rather than assigning zero to clear values
The `delete` keyword more closely matches the semantics of what is being done, and draws more attention to the changing of state, which may lead to a more thorough audit of its associated logic.

<details>
<summary>
There are <b>22</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

192:         for (uint256 i = 0; i < _hTokens.length;) {

```
[#L192](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L192) 

```solidity
File: src/BranchBridgeAgent.sol

444:         deposit.owner = address(0);

447:         for (uint256 i = 0; i < deposit.tokens.length;) {

513:         for (uint256 i = 0; i < numOfAssets;) {

```
[#L444](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L444) [#L447](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L447) [#L513](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L513) 

```solidity
File: src/BranchPort.sol

257:         for (uint256 i = 0; i < length;) {

305:         for (uint256 i = 0; i < length;) {

```
[#L257](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L257) [#L305](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L305) 

```solidity
File: src/MulticallRootRouter.sol

278:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

367:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

455:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

557:         for (uint256 i = 0; i < outputTokens.length;) {

```
[#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L278) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L367) [#L455](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L455) [#L557](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L557) 

```solidity
File: src/RootBridgeAgent.sol

318:         for (uint256 i = 0; i < settlement.hTokens.length;) {

399:         for (uint256 i = 0; i < length;) {

1070:         for (uint256 i = 0; i < hTokens.length;) {

```
[#L318](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L318) [#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L399) [#L1070](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1070) 

```solidity
File: src/RootBridgeAgentExecutor.sol

281:         for (uint256 i = 0; i < uint256(uint8(numOfAssets));) {

```
[#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L281) 

```solidity
File: src/RootPort.sol

212:         return getLocalTokenFromGlobal[_globalAddress][_srcChainId] != address(0);

217:         return getGlobalTokenFromLocal[_localAddress][_srcChainId] != address(0);

226:         return _getLocalToken(_localAddress, _srcChainId, _dstChainId) != address(0);

231:         return getLocalTokenFromUnderlying[_underlyingToken][_srcChainId] != address(0);

```
[#L212](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L212) [#L217](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L217) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L226) [#L231](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L231) 

```solidity
File: src/VirtualAccount.sol

70:         for (uint256 i = 0; i < length;) {

90:         for (uint256 i = 0; i < length;) {

```
[#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L70) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L90) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

23:     uint8 internal constant STATUS_SUCCESS = 0;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) 

</details>

---

<a name="NC-35"></a> 
### [NC-35] Solidity compiler version is not fixed
To prevent the actual contracts deployed from behaving differently depending on the compiler version, it is recommended to use a fixed solidity version.

<details>
<summary>
There are <b>44</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L2) 

```solidity
File: src/ArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L3) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L2) 

```solidity
File: src/BaseBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L2) 

```solidity
File: src/BranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L2) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L2) 

```solidity
File: src/BranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L3) 

```solidity
File: src/CoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L2) 

```solidity
File: src/CoreRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouterLibZip.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L2) 

```solidity
File: src/RootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L2) 

```solidity
File: src/RootBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L2) 

```solidity
File: src/RootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L3) 

```solidity
File: src/VirtualAccount.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L3) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L2) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L2) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L3) 

```solidity
File: src/interfaces/IMulticall2.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L2) 

```solidity
File: src/interfaces/IPortStrategy.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L3) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IRootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L3) 

```solidity
File: src/interfaces/IRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L2) 

```solidity
File: src/interfaces/IVirtualAccount.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L2) 

```solidity
File: src/token/ERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L2) 

```solidity
File: src/token/ERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L2) 

</details>

---

<a name="NC-36"></a> 
### [NC-36] Expressions for constant values should use `immutable` rather than `constant`
While it doesn't save any gas because the compiler knows that developers often make this mistake, it's still best to use the right tool for the task at hand. There is a difference between `constant` variables and `immutable` variables, and they should each be used in their appropriate contexts. `constants` should be used for literal values written into the code, and `immutable` variables should be used for expressions, or values calculated in, or passed into the constructor.

<details>
<summary>
There are <b>22</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

97:     uint256 internal constant DIVISIONER = 1e4;

98:     uint256 internal constant MIN_RESERVE_RATIO = 3e3;

```
[#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L98) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

15:     uint8 internal constant STATUS_DONE = 1;

17:     uint8 internal constant STATUS_RETRIEVE = 2;

21:     uint8 internal constant STATUS_FAILED = 1;

23:     uint8 internal constant STATUS_SUCCESS = 0;

27:     uint256 internal constant PARAMS_START = 1;

29:     uint256 internal constant PARAMS_START_SIGNED = 21;

31:     uint256 internal constant PARAMS_TKN_START = 5;

33:     uint256 internal constant PARAMS_TKN_START_SIGNED = 25;

35:     uint256 internal constant PARAMS_ENTRY_SIZE = 32;

37:     uint256 internal constant PARAMS_ADDRESS_SIZE = 20;

39:     uint256 internal constant PARAMS_TKN_SET_SIZE = 109;

41:     uint256 internal constant PARAMS_TKN_SET_SIZE_MULTIPLE = 128;

43:     uint256 internal constant ADDRESS_END_OFFSET = 12;

45:     uint256 internal constant PARAMS_AMT_OFFSET = 64;

47:     uint256 internal constant PARAMS_DEPOSIT_OFFSET = 96;

49:     uint256 internal constant PARAMS_END_OFFSET = 6;

51:     uint256 internal constant PARAMS_END_SIGNED_OFFSET = 26;

53:     uint256 internal constant PARAMS_SETTLEMENT_OFFSET = 129;

57:     uint256 internal constant MAX_TOKENS_LENGTH = 255;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L15) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L17) [#L21](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L21) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) [#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L27) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L29) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L31) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L33) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L35) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L37) [#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L39) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L41) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L43) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L45) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L47) [#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L49) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L51) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L53) [#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L57) 

</details>

---

<a name="NC-37"></a> 
### [NC-37] Use `@inheritdoc` for overridden functions

<details>
<summary>
There are <b>55</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

89:     function retrySettlement(uint32, bytes calldata, GasParams[2] calldata, bool) external payable override lock {}

99:     function _performCall(address payable, bytes memory _calldata, GasParams calldata) internal override {

112:     function _performFallbackCall(address payable, uint32 _settlementNonce) internal override {

125:     function _requiresEndpoint(address _endpoint, bytes calldata) internal view override {

```
[#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L89) [#L99](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L99) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L112) [#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L125) 

```solidity
File: src/ArbitrumBranchPort.sol

107:     function _bridgeIn(address _recipient, address _localAddress, uint256 _amount) internal override {

```
[#L107](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L107) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

51:     function addLocalToken(address _underlyingAddress, GasParams calldata) external payable override {

126:     function executeNoSettlement(bytes calldata _data) external payable override requiresAgentExecutor {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L51) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L126) 

```solidity
File: src/BaseBranchRouter.sol

74:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

83:     function callOut(bytes calldata _params, GasParams calldata _gParams) external payable override lock {

123:     function executeNoSettlement(bytes calldata) external payable virtual override requiresAgentExecutor {

```
[#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L74) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L83) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L123) 

```solidity
File: src/BranchBridgeAgent.sol

156:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

422:     function retrieveDeposit(uint32 _depositNonce, GasParams calldata _gParams) external payable override lock {

434:     function redeemDeposit(uint32 _depositNonce) external override lock {

578:     function lzReceive(uint16, bytes calldata _srcAddress, uint64, bytes calldata _payload) public override {

```
[#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L156) [#L422](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L422) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L434) [#L578](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L578) 

```solidity
File: src/BranchPort.sol

135:     function renounceOwnership() public payable override onlyOwner {

144:     function manage(address _token, uint256 _amount) external override requiresPortStrategy(_token) {

167:     function replenishReserves(address _token, uint256 _amount) external override lock {

188:     function replenishReserves(address _strategy, address _token) external override lock {

319:     function addBridgeAgent(address _bridgeAgent) external override requiresBridgeAgentFactory {

331:     function setCoreRouter(address _newCoreRouter) external override requiresCoreRouter {

338:     function addBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

348:     function toggleBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

355:     function toggleBridgeAgent(address _bridgeAgent) external override requiresCoreRouter {

362:     function addStrategyToken(address _token, uint256 _minimumReservesRatio) external override requiresCoreRouter {

375:     function toggleStrategyToken(address _token) external override requiresCoreRouter {

396:     function togglePortStrategy(address _portStrategy, address _token) external override requiresCoreRouter {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L135) [#L144](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L144) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L167) [#L188](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L188) [#L319](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L319) [#L331](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L331) [#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L338) [#L348](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L348) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L355) [#L362](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L362) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L375) [#L396](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L396) 

```solidity
File: src/CoreBranchRouter.sol

86:     function executeNoSettlement(bytes calldata _params) external payable virtual override requiresAgentExecutor {

```
[#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L86) 

```solidity
File: src/CoreRootRouter.sol

332:     function execute(bytes calldata _encodedData, uint16) external payable override requiresExecutor {

370:     function executeSigned(bytes memory, address, uint16) external payable override requiresExecutor {

```
[#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L332) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L370) 

```solidity
File: src/MulticallRootRouter.sol

123:     function executeResponse(bytes memory, uint16) external payable override {

137:     function execute(bytes calldata encodedData, uint16) external payable override lock requiresExecutor {

203:     function executeDepositSingle(bytes calldata, DepositParams calldata, uint16) external payable override {

```
[#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L123) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L137) [#L203](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L203) 

```solidity
File: src/MulticallRootRouterLibZip.sol

37:     function _decode(bytes calldata data) internal pure override returns (bytes memory) {

```
[#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L37) 

```solidity
File: src/RootBridgeAgent.sol

135:     function getSettlementEntry(uint32 _settlementNonce) external view override returns (Settlement memory) {

299:     function redeemSettlement(uint32 _settlementNonce) external override lock {

1170:     function approveBranchBridgeAgent(uint256 _branchChainId) external override requiresManager {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L135) [#L299](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L299) [#L1170](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1170) 

```solidity
File: src/RootPort.sol

166:     function renounceOwnership() public payable override onlyOwner {

211:     function isGlobalToken(address _globalAddress, uint256 _srcChainId) external view override returns (bool) {

216:     function isLocalToken(address _localAddress, uint256 _srcChainId) external view override returns (bool) {

230:     function isUnderlyingToken(address _underlyingToken, uint256 _srcChainId) external view override returns (bool) {

350:     function fetchVirtualAccount(address _user) external override returns (VirtualAccount account) {

382:     function addBridgeAgent(address _manager, address _bridgeAgent) external override requiresBridgeAgentFactory {

414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

421:     function addBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

431:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

509:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external override onlyOwner {

```
[#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L166) [#L211](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L211) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L216) [#L230](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L230) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L350) [#L382](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L382) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L421) [#L431](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L431) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) [#L509](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L509) 

```solidity
File: src/VirtualAccount.sol

51:     function withdrawNative(uint256 _amount) external override requiresApprovedCaller {

56:     function withdrawERC20(address _token, uint256 _amount) external override requiresApprovedCaller {

61:     function withdrawERC721(address _token, uint256 _tokenId) external override requiresApprovedCaller {

66:     function call(Call[] calldata calls) external override requiresApprovedCaller returns (bytes[] memory returnData) {

119:     function onERC721Received(address, address, uint256, bytes calldata) external pure override returns (bytes4) {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L51) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L56) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L61) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L66) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L119) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

```
[#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) 

```solidity
File: src/token/ERC20hTokenBranch.sol

29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

35:     function burn(uint256 amount) public override onlyOwner {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L35) 

</details>

---

<a name="NC-38"></a> 
### [NC-38] Use the latest solidity version for deployment
Upgrading to a newer Solidity release can optimize gas usage, take advantage of new features and improve overall contract efficiency. Where possible, based on compatibility requirements, it is recommended to use newer/latest solidity version to take advantage of the latest optimizations and features.

<details>
<summary>
There are <b>44</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L2) 

```solidity
File: src/ArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L3) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L2) 

```solidity
File: src/BaseBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L2) 

```solidity
File: src/BranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L2) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L2) 

```solidity
File: src/BranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L3) 

```solidity
File: src/CoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L2) 

```solidity
File: src/CoreRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouterLibZip.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L2) 

```solidity
File: src/RootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L2) 

```solidity
File: src/RootBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L2) 

```solidity
File: src/RootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L3) 

```solidity
File: src/VirtualAccount.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L3) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L2) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L2) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L3) 

```solidity
File: src/interfaces/IMulticall2.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L2) 

```solidity
File: src/interfaces/IPortStrategy.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L3) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IRootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L3) 

```solidity
File: src/interfaces/IRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L2) 

```solidity
File: src/interfaces/IVirtualAccount.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L2) 

```solidity
File: src/token/ERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L2) 

```solidity
File: src/token/ERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L2) 

</details>

---

<a name="NC-39"></a> 
### [NC-39] Use of `override` is unnecessary
Starting with Solidity version [0.8.8](https://docs.soliditylang.org/en/v0.8.20/contracts.html#function-overriding), using the `override` keyword when the function solely overrides an interface function, and the function doesn't exist in multiple base contracts, is unnecessary.

<details>
<summary>
There are <b>78</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

89:     function retrySettlement(uint32, bytes calldata, GasParams[2] calldata, bool) external payable override lock {}

99:     function _performCall(address payable, bytes memory _calldata, GasParams calldata) internal override {

112:     function _performFallbackCall(address payable, uint32 _settlementNonce) internal override {

125:     function _requiresEndpoint(address _endpoint, bytes calldata) internal view override {

```
[#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L89) [#L99](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L99) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L112) [#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L125) 

```solidity
File: src/ArbitrumBranchPort.sol

107:     function _bridgeIn(address _recipient, address _localAddress, uint256 _amount) internal override {

125:     ) internal override {

```
[#L107](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L107) [#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L125) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

51:     function addLocalToken(address _underlyingAddress, GasParams calldata) external payable override {

92:     ) internal override {

126:     function executeNoSettlement(bytes calldata _data) external payable override requiresAgentExecutor {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L51) [#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L92) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L126) 

```solidity
File: src/BaseBranchRouter.sol

74:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

83:     function callOut(bytes calldata _params, GasParams calldata _gParams) external payable override lock {

108:     ) external payable override lock {

123:     function executeNoSettlement(bytes calldata) external payable virtual override requiresAgentExecutor {

```
[#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L74) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L83) [#L108](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L108) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L123) 

```solidity
File: src/BranchBridgeAgent.sol

156:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

214:     ) external payable override lock {

236:     ) external payable override lock {

282:     ) external payable override lock {

312:     ) external payable override lock {

349:     ) external payable override lock {

422:     function retrieveDeposit(uint32 _depositNonce, GasParams calldata _gParams) external payable override lock {

434:     function redeemDeposit(uint32 _depositNonce) external override lock {

469:     ) external payable virtual override lock {

578:     function lzReceive(uint16, bytes calldata _srcAddress, uint64, bytes calldata _payload) public override {

```
[#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L156) [#L214](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L214) [#L236](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L236) [#L282](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L282) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L312) [#L349](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L349) [#L422](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L422) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L434) [#L469](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L469) [#L578](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L578) 

```solidity
File: src/BranchPort.sol

135:     function renounceOwnership() public payable override onlyOwner {

144:     function manage(address _token, uint256 _amount) external override requiresPortStrategy(_token) {

167:     function replenishReserves(address _token, uint256 _amount) external override lock {

188:     function replenishReserves(address _strategy, address _token) external override lock {

252:     ) external override requiresBridgeAgent {

283:     ) external override lock requiresBridgeAgent {

294:     ) external override lock requiresBridgeAgent {

319:     function addBridgeAgent(address _bridgeAgent) external override requiresBridgeAgentFactory {

331:     function setCoreRouter(address _newCoreRouter) external override requiresCoreRouter {

338:     function addBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

348:     function toggleBridgeAgentFactory(address _newBridgeAgentFactory) external override requiresCoreRouter {

355:     function toggleBridgeAgent(address _bridgeAgent) external override requiresCoreRouter {

362:     function addStrategyToken(address _token, uint256 _minimumReservesRatio) external override requiresCoreRouter {

375:     function toggleStrategyToken(address _token) external override requiresCoreRouter {

396:     function togglePortStrategy(address _portStrategy, address _token) external override requiresCoreRouter {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L135) [#L144](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L144) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L167) [#L188](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L188) [#L252](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L252) [#L283](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L283) [#L294](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L294) [#L319](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L319) [#L331](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L331) [#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L338) [#L348](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L348) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L355) [#L362](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L362) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L375) [#L396](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L396) 

```solidity
File: src/CoreBranchRouter.sol

86:     function executeNoSettlement(bytes calldata _params) external payable virtual override requiresAgentExecutor {

```
[#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L86) 

```solidity
File: src/CoreRootRouter.sol

332:     function execute(bytes calldata _encodedData, uint16) external payable override requiresExecutor {

370:     function executeSigned(bytes memory, address, uint16) external payable override requiresExecutor {

```
[#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L332) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L370) 

```solidity
File: src/MulticallRootRouter.sol

123:     function executeResponse(bytes memory, uint16) external payable override {

137:     function execute(bytes calldata encodedData, uint16) external payable override lock requiresExecutor {

203:     function executeDepositSingle(bytes calldata, DepositParams calldata, uint16) external payable override {

406:     ) external payable override requiresExecutor lock {

```
[#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L123) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L137) [#L203](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L203) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L406) 

```solidity
File: src/MulticallRootRouterLibZip.sol

37:     function _decode(bytes calldata data) internal pure override returns (bytes memory) {

```
[#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L37) 

```solidity
File: src/RootBridgeAgent.sol

135:     function getSettlementEntry(uint32 _settlementNonce) external view override returns (Settlement memory) {

166:     ) external payable override lock requiresRouter {

183:     ) external payable override lock requiresRouter {

210:     ) external payable override lock requiresRouter {

239:     ) external payable override lock {

299:     function redeemSettlement(uint32 _settlementNonce) external override lock {

439:     ) public override requiresEndpoint(_endpoint, _srcChainId, _srcAddress) {

1170:     function approveBranchBridgeAgent(uint256 _branchChainId) external override requiresManager {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L135) [#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L166) [#L183](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L183) [#L210](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L210) [#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L239) [#L299](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L299) [#L439](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L439) [#L1170](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1170) 

```solidity
File: src/RootPort.sol

166:     function renounceOwnership() public payable override onlyOwner {

211:     function isGlobalToken(address _globalAddress, uint256 _srcChainId) external view override returns (bool) {

216:     function isLocalToken(address _localAddress, uint256 _srcChainId) external view override returns (bool) {

230:     function isUnderlyingToken(address _underlyingToken, uint256 _srcChainId) external view override returns (bool) {

244:     ) external override requiresCoreRootRouter {

350:     function fetchVirtualAccount(address _user) external override returns (VirtualAccount account) {

382:     function addBridgeAgent(address _manager, address _bridgeAgent) external override requiresBridgeAgentFactory {

397:     ) external override requiresCoreRootRouter {

414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

421:     function addBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

431:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

446:     ) external override onlyOwner {

483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

509:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external override onlyOwner {

527:     ) external payable override onlyOwner {

```
[#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L166) [#L211](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L211) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L216) [#L230](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L230) [#L244](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L244) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L350) [#L382](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L382) [#L397](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L397) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L421) [#L431](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L431) [#L446](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L446) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) [#L509](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L509) [#L527](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L527) 

```solidity
File: src/VirtualAccount.sol

51:     function withdrawNative(uint256 _amount) external override requiresApprovedCaller {

56:     function withdrawERC20(address _token, uint256 _amount) external override requiresApprovedCaller {

61:     function withdrawERC721(address _token, uint256 _tokenId) external override requiresApprovedCaller {

66:     function call(Call[] calldata calls) external override requiresApprovedCaller returns (bytes[] memory returnData) {

119:     function onERC721Received(address, address, uint256, bytes calldata) external pure override returns (bytes4) {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L51) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L56) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L61) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L66) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L119) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

83:     ) external virtual override returns (address newBridgeAgent) {

```
[#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L83) 

```solidity
File: src/token/ERC20hTokenBranch.sol

29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

35:     function burn(uint256 amount) public override onlyOwner {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L35) 

</details>

---

<a name="NC-40"></a> 
### [NC-40] Visibility of state variables is not explicitly defined
To avoid misunderstandings and unexpected state accesses, it is recommended to explicitly define the visibility of each state variable.

<details>
<summary>
There are <b>72</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

105:         bytes calldata _params,

```
[#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L105) 

```solidity
File: src/CoreRootRouter.sol

157:         address _rootBridgeAgentFactory,

158:         address _branchBridgeAgentFactory,

159:         address _refundee,

160:         uint16 _dstChainId,

```
[#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L157) [#L158](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L158) [#L159](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L159) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L160) 

```solidity
File: src/MulticallRootRouter.sol

19:     address recipient;

21:     address outputToken;

23:     uint256 amountOut;

25:     uint256 depositOut;

30:     address recipient;

32:     address[] outputTokens;

34:     uint256[] amountsOut;

36:     uint256[] depositsOut;

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L19) [#L21](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L21) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L23) [#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L25) [#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L30) [#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L32) [#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L34) [#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L36) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

9:     uint256 gasLimit; // gas allocated for the cross-chain call.

10:     uint256 remoteBranchExecutionGas; //gas allocated for remote branch execution. Must be lower than `gasLimit`.

14:     uint8 status;

15:     address owner;

16:     address[] hTokens;

17:     address[] tokens;

18:     uint256[] amounts;

19:     uint256[] deposits;

24:     address hToken; //Input Local hTokens Address.

25:     address token; //Input Native / underlying Token Address.

26:     uint256 amount; //Amount of Local hTokens deposited for interaction.

27:     uint256 deposit; //Amount of native tokens deposited for interaction.

32:     address[] hTokens; //Input Local hTokens Address.

33:     address[] tokens; //Input Native / underlying Token Address.

34:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

35:     uint256[] deposits; //Amount of native tokens deposited for interaction.

40:     uint8 numberOfAssets; //Number of assets to deposit.

41:     uint32 depositNonce; //Deposit nonce.

42:     address[] hTokens; //Input Local hTokens Address.

43:     address[] tokens; //Input Native / underlying Token Address.

44:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

45:     uint256[] deposits; //Amount of native tokens deposited for interaction.

50:     uint32 depositNonce; //Deposit nonce.

51:     address hToken; //Input Local hTokens Address.

52:     address token; //Input Native / underlying Token Address.

53:     uint256 amount; //Amount of Local hTokens deposited for interaction.

54:     uint256 deposit; //Amount of native tokens deposited for interaction.

58:     uint16 dstChainId; //Destination chain for interaction.

59:     uint80 status; //Status of the settlement

60:     address owner; //Owner of the settlement

61:     address recipient; //Recipient of the settlement.

62:     address[] hTokens; //Input Local hTokens Addresses.

63:     address[] tokens; //Input Native / underlying Token Addresses.

64:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

65:     uint256[] deposits; //Amount of native tokens deposited for interaction.

69:     address globalAddress; //Input Global hTokens Address.

70:     uint256 amount; //Amount of Local hTokens deposited for interaction.

71:     uint256 deposit; //Amount of native tokens deposited for interaction.

75:     address[] globalAddresses; //Input Global hTokens Addresses.

76:     uint256[] amounts; //Amount of Local hTokens deposited for interaction.

77:     uint256[] deposits; //Amount of native tokens deposited for interaction.

81:     uint32 settlementNonce; // Settlement nonce.

82:     address recipient; // Recipient of the settlement.

83:     address hToken; // Input Local hTokens Address.

84:     address token; // Input Native / underlying Token Address.

85:     uint256 amount; // Amount of Local hTokens deposited for interaction.

86:     uint256 deposit; // Amount of native tokens deposited for interaction.

90:     uint8 numberOfAssets; // Number of assets to deposit.

91:     address recipient; // Recipient of the settlement.

92:     uint32 settlementNonce; // Settlement nonce.

93:     address[] hTokens; // Input Local hTokens Addresses.

94:     address[] tokens; // Input Native / underlying Token Addresses.

95:     uint256[] amounts; // Amount of Local hTokens deposited for interaction.

96:     uint256[] deposits; // Amount of native tokens deposited for interaction.

```
[#L9](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L9) [#L10](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L10) [#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L14) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L15) [#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L16) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L17) [#L18](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L18) [#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L19) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L24) [#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L25) [#L26](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L26) [#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L27) [#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L32) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L33) [#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L34) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L35) [#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L40) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L41) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L42) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L43) [#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L44) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L45) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L50) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L51) [#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L52) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L53) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L54) [#L58](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L58) [#L59](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L59) [#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L60) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L61) [#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L62) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L63) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L64) [#L65](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L65) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L69) [#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L70) [#L71](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L71) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L75) [#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L76) [#L77](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L77) [#L81](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L81) [#L82](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L82) [#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L83) [#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L84) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L85) [#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L86) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L90) [#L91](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L91) [#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L92) [#L93](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L93) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L94) [#L95](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L95) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L96) 

```solidity
File: src/interfaces/IVirtualAccount.sol

8:     address target;

9:     bytes callData;

14:     address target;

15:     bytes callData;

16:     uint256 value;

```
[#L8](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L8) [#L9](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L9) [#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L14) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L15) [#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L16) 

</details>

---

<a name="NC-41"></a> 
### [NC-41] Missing checks for `address(0)` when assigning values to address state variables

<details>
<summary>
There are <b>7</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

419:         coreBranchRouterAddress = _coreBranchRouter;

```
[#L419](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L419) 

```solidity
File: src/CoreBranchRouter.sol

31:         hTokenFactoryAddress = _hTokenFactoryAddress;

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L31) 

```solidity
File: src/CoreRootRouter.sol

73:         rootPortAddress = _rootPortAddress;

88:         hTokenFactoryAddress = _hTokenFactory;

```
[#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L73) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L88) 

```solidity
File: src/VirtualAccount.sol

36:         userAddress = _userAddress;

37:         localPortAddress = _localPortAddress;

```
[#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L36) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L37) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

35:         lzEndpointAddress = _lzEndpointAddress;

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L35) 

</details>

---

<a name="NC-42"></a> 
### [NC-42] Common functions should be refactored to a common base contract
The functions below have the same implementation as is seen in other files. The functions should be refactored into functions of a common base contract.

<details>
<summary>
There are <b>146</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

/// Seen in src/RootPort.sol
135:     function renounceOwnership() public payable override onlyOwner {

/// Seen in src/RootPort.sol
355:     function toggleBridgeAgent(address _bridgeAgent) external override requiresCoreRouter {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L135) [#L355](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L355) 

```solidity
File: src/CoreRootRouter.sol

/// Seen in src/MulticallRootRouter.sol
350:     function executeDepositSingle(bytes memory, DepositParams memory, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Seen in src/MulticallRootRouter.sol
360:     function executeDepositMultiple(bytes calldata, DepositMultipleParams memory, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Seen in src/MulticallRootRouter.sol
370:     function executeSigned(bytes memory, address, uint16) external payable override requiresExecutor {

/// Seen in src/MulticallRootRouter.sol
375:     function executeSignedDepositSingle(bytes memory, DepositParams memory, address, uint16)
             external
             payable
             override
             requiresExecutor
         {

/// Seen in src/MulticallRootRouter.sol
385:     function executeSignedDepositMultiple(bytes memory, DepositMultipleParams memory, address, uint16)
             external
             payable
             override
             requiresExecutor
         {

```
[#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L350) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L360) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L370) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L375) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L385) 

```solidity
File: src/MulticallRootRouter.sol

/// Seen in src/CoreRootRouter.sol
123:     function executeResponse(bytes memory, uint16) external payable override {

/// Seen in src/CoreRootRouter.sol
203:     function executeDepositSingle(bytes calldata, DepositParams calldata, uint16) external payable override {

/// Seen in src/CoreRootRouter.sol
209:     function executeDepositMultiple(bytes calldata, DepositMultipleParams calldata, uint16) external payable {

```
[#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L123) [#L203](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L203) [#L209](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L209) 

```solidity
File: src/RootPort.sol

/// Seen in src/BranchPort.sol
166:     function renounceOwnership() public payable override onlyOwner {

/// Seen in src/BranchPort.sol
414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

```
[#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L166) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
28:     function depositToPort(address _depositor, address _recipient, address _underlyingAddress, uint256 _amount)

/// Seen in src/interfaces/IRootBridgeAgent.sol
38:     function withdrawFromPort(address _depositor, address _recipient, address _globalAddress, uint256 _amount)

```
[#L28](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L28) [#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L38) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
96:     function localPortAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
102:     function bridgeAgentExecutorAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
109:     function getDepositEntry(uint32 depositNonce) external view returns (Deposit memory);

/// Seen in src/interfaces/IRootBridgeAgent.sol
120:     function getFeeEstimate(uint256 _gasLimit, uint256 _remoteBranchExecutionGas, bytes calldata _payload)

/// Seen in src/interfaces/IRootBridgeAgent.sol
138:     function callOutSystem(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Seen in src/interfaces/IRootBridgeAgent.sol
150:     function callOut(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Seen in src/interfaces/IRootBridgeAgent.sol
163:     function callOutAndBridge(

/// Seen in src/interfaces/IRootBridgeAgent.sol
179:     function callOutAndBridgeMultiple(

/// Seen in src/interfaces/IRootBridgeAgent.sol
194:     function callOutSigned(address payable gasRefundee, bytes calldata params, GasParams calldata gasParams)

/// Seen in src/interfaces/IRootBridgeAgent.sol
208:     function callOutSignedAndBridge(

/// Seen in src/interfaces/IRootBridgeAgent.sol
227:     function callOutSignedAndBridgeMultiple(

/// Seen in src/interfaces/IRootBridgeAgent.sol
248:     function retryDeposit(

/// Seen in src/interfaces/IRootBridgeAgent.sol
263:     function retrieveDeposit(uint32 depositNonce, GasParams calldata gasParams) external payable;

/// Seen in src/interfaces/IRootBridgeAgent.sol
270:     function redeemDeposit(uint32 depositNonce) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
285:     function retrySettlement(

/// Seen in src/interfaces/IRootBridgeAgent.sol
305:     function clearToken(address recipient, address hToken, address token, uint256 amount, uint256 deposit) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
312:     function clearTokens(bytes calldata sParams, address recipient)

/// Seen in src/interfaces/IRootBridgeAgent.sol
326:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload) external;

```
[#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L96) [#L102](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L102) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L109) [#L120](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L120) [#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L138) [#L150](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L150) [#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L163) [#L179](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L179) [#L194](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L194) [#L208](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L208) [#L227](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L227) [#L248](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L248) [#L263](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L263) [#L270](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L270) [#L285](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L285) [#L305](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L305) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L312) [#L326](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L326) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
24:     function createBridgeAgent(

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L24) 

```solidity
File: src/interfaces/IBranchPort.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
23:     function isBridgeAgent(address _bridgeAgent) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
30:     function isStrategyToken(address _token) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
38:     function isPortStrategy(address _strategy, address _token) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
45:     function isBridgeAgentFactory(address _bridgeAgentFactory) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
56:     function manage(address _token, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
64:     function replenishReserves(address _token, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
72:     function replenishReserves(address _strategy, address _token) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
85:     function withdraw(address _recipient, address _underlyingAddress, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
94:     function bridgeIn(address _recipient, address _localAddress, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
103:     function bridgeInMultiple(

/// Seen in src/interfaces/IRootBridgeAgent.sol
118:     function bridgeOut(

/// Seen in src/interfaces/IRootBridgeAgent.sol
135:     function bridgeOutMultiple(

/// Seen in src/interfaces/IRootBridgeAgent.sol
151:     function addBridgeAgent(address _bridgeAgent) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
157:     function setCoreRouter(address _newCoreRouter) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
163:     function addBridgeAgentFactory(address _bridgeAgentFactory) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
169:     function toggleBridgeAgentFactory(address _newBridgeAgentFactory) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
175:     function toggleBridgeAgent(address _bridgeAgent) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
181:     function addStrategyToken(address _token, uint256 _minimumReservesRatio) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
187:     function toggleStrategyToken(address _token) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
193:     function addPortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
199:     function togglePortStrategy(address _portStrategy, address _token) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
207:     function updatePortStrategy(address _portStrategy, address _token, uint256 _dailyManagementLimit) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
214:     function setCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent) external;

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L23) [#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L30) [#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L38) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L45) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L56) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L64) [#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L72) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L85) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L94) [#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L103) [#L118](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L118) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L135) [#L151](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L151) [#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L157) [#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L163) [#L169](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L169) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L175) [#L181](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L181) [#L187](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L187) [#L193](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L193) [#L199](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L199) [#L207](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L207) [#L214](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L214) 

```solidity
File: src/interfaces/IBranchRouter.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
27:     function localPortAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
30:     function localBridgeAgentAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
33:     function bridgeAgentExecutorAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
46:     function callOut(bytes calldata params, GasParams calldata gParams) external payable;

/// Seen in src/interfaces/IRootBridgeAgent.sol
56:     function callOutAndBridge(bytes calldata params, DepositInput calldata dParams, GasParams calldata gParams)

/// Seen in src/interfaces/IRootBridgeAgent.sol
68:     function callOutAndBridgeMultiple(

/// Seen in src/interfaces/IRootBridgeAgent.sol
79:     function getDepositEntry(uint32 depositNonce) external view returns (Deposit memory);

/// Seen in src/interfaces/IRootBridgeAgent.sol
89:     function executeNoSettlement(bytes calldata params) external payable;

/// Seen in src/interfaces/IRootBridgeAgent.sol
96:     function executeSettlement(bytes calldata params, SettlementParams calldata sParams) external payable;

/// Seen in src/interfaces/IRootBridgeAgent.sol
105:     function executeSettlementMultiple(bytes calldata params, SettlementMultipleParams calldata sParams)

```
[#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L27) [#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L30) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L33) [#L46](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L46) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L56) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L68) [#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L79) [#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L89) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L96) [#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L105) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
38:     function addGlobalToken(address _globalAddress, uint256 _dstChainId, GasParams[3] calldata _gasParams)

/// Seen in src/interfaces/IRootBridgeAgent.sol
47:     function addLocalToken(address _underlyingAddress, GasParams calldata _gasParams) external payable;

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L38) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L47) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
22:     function mint(address account, uint256 amount) external returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
28:     function burn(uint256 amount) external;

```
[#L22](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L22) [#L28](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L28) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L24) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
19:     function localChainId() external view returns (uint16);

/// Seen in src/interfaces/IRootBridgeAgent.sol
23:     function factoryAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
30:     function getTokenBalance(uint256 chainId) external view returns (uint256);

/// Seen in src/interfaces/IRootBridgeAgent.sol
43:     function mint(address to, uint256 amount, uint256 chainId) external returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
51:     function burn(address from, uint256 amount, uint256 chainId) external;

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L19) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L23) [#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L30) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L43) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L51) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L24) 

```solidity
File: src/interfaces/IPortStrategy.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
23:     function withdraw(address _recipient, address _token, uint256 _amount) external;

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L23) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
104:     function settlementNonce() external view returns (uint32 nonce);

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
111:     function getSettlementEntry(uint32 _settlementNonce) external view returns (Settlement memory);

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
117:     function bridgeAgentExecutorAddress() external view returns (address);

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
123:     function factoryAddress() external view returns (address);

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
130:     function getBranchBridgeAgent(uint256 _chainId) external view returns (address);

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
138:     function isBranchBridgeAgentAllowed(uint256 _chainId) external view returns (bool);

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
149:     function getFeeEstimate(

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
168:     function callOut(

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
189:     function callOutAndBridge(

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
213:     function callOutAndBridgeMultiple(

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
236:     function retrySettlement(

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
250:     function retrieveSettlement(uint32 _settlementNonce, GasParams calldata _gParams) external payable;

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
257:     function redeemSettlement(uint32 _depositNonce) external;

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
271:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId) external;

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
295:     function bridgeInMultiple(address _recipient, DepositMultipleParams calldata _dParams, uint256 _srcChainId)

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
309:     function lzReceiveNonBlocking(

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
324:     function approveBranchBridgeAgent(uint256 _branchChainId) external;

/// Seen in src/interfaces/IERC20hTokenBranchFactory.sol
331:     function syncBranchBridgeAgent(address _newBranchBridgeAgent, uint256 _branchChainId) external;

```
[#L104](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L104) [#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L111) [#L117](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L117) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L123) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L130) [#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L138) [#L149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L149) [#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L168) [#L189](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L189) [#L213](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L213) [#L236](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L236) [#L250](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L250) [#L257](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L257) [#L271](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L271) [#L295](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L295) [#L309](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L309) [#L324](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L324) [#L331](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L331) 

```solidity
File: src/interfaces/IRootPort.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
40:     function isChainId(uint256 _chainId) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
47:     function getBridgeAgentManager(address _rootBridgeAgent) external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
54:     function isBridgeAgentFactory(address _bridgeAgentFactory) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
61:     function isGlobalAddress(address _globalAddress) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
69:     function getGlobalTokenFromLocal(address _localAddress, uint256 _srcChainId) external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
77:     function getLocalTokenFromGlobal(address _globalAddress, uint256 _srcChainId) external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
85:     function getLocalTokenFromUnderlying(address _underlyingAddress, uint256 _srcChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
97:     function getLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
108:     function getUnderlyingTokenFromLocal(address _localAddress, uint256 _srcChainId) external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
116:     function getUnderlyingTokenFromGlobal(address _globalAddress, uint256 _srcChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
127:     function isGlobalToken(address _globalAddress, uint256 _srcChainId) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
135:     function isLocalToken(address _localAddress, uint256 _srcChainId) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
144:     function isLocalToken(address _localAddress, uint256 _srcChainId, uint256 _dstChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
155:     function isUnderlyingToken(address _underlyingToken, uint256 _srcChainId) external view returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
162:     function getUserAccount(address _user) external view returns (VirtualAccount);

/// Seen in src/interfaces/IRootBridgeAgent.sol
170:     function isRouterApproved(VirtualAccount _userAccount, address _router) external returns (bool);

/// Seen in src/interfaces/IRootBridgeAgent.sol
183:     function burn(address _from, address _hToken, uint256 _amount, uint256 _srcChainId) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
193:     function bridgeToRoot(address _recipient, address _hToken, uint256 _amount, uint256 _deposit, uint256 _srcChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
202:     function bridgeToRootFromLocalBranch(address _from, address _hToken, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
210:     function bridgeToLocalBranchFromRoot(address _to, address _hToken, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
218:     function mintToLocalBranch(address _recipient, address _hToken, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
226:     function burnFromLocalBranch(address _from, address _hToken, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
238:     function setAddresses(

/// Seen in src/interfaces/IRootBridgeAgent.sol
251:     function setLocalAddress(address _globalAddress, address _localAddress, uint256 _srcChainId) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
261:     function fetchVirtualAccount(address _user) external returns (VirtualAccount account);

/// Seen in src/interfaces/IRootBridgeAgent.sol
269:     function toggleVirtualAccountApproved(VirtualAccount _userAccount, address _router) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
281:     function syncBranchBridgeAgentWithRoot(address _newBranchBridgeAgent, address _rootBridgeAgent, uint256 _srcChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
289:     function addBridgeAgent(address _manager, address _bridgeAgent) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
295:     function toggleBridgeAgent(address _bridgeAgent) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
301:     function addBridgeAgentFactory(address _bridgeAgentFactory) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
307:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
319:     function addNewChain(

/// Seen in src/interfaces/IRootBridgeAgent.sol
333:     function addEcosystemToken(address ecoTokenGlobalAddress) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
340:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
350:     function setCoreBranchRouter(

/// Seen in src/interfaces/IRootBridgeAgent.sol
364:     function syncNewCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent, uint16 _dstChainId)

```
[#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L40) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L47) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L54) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L61) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L69) [#L77](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L77) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L85) [#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L97) [#L108](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L108) [#L116](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L116) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L127) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L135) [#L144](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L144) [#L155](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L155) [#L162](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L162) [#L170](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L170) [#L183](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L183) [#L193](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L193) [#L202](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L202) [#L210](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L210) [#L218](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L218) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L226) [#L238](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L238) [#L251](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L251) [#L261](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L261) [#L269](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L269) [#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L281) [#L289](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L289) [#L295](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L295) [#L301](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L301) [#L307](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L307) [#L319](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L319) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L333) [#L340](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L340) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L350) [#L364](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L364) 

```solidity
File: src/interfaces/IRootRouter.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
25:     function executeResponse(bytes memory params, uint16 srcChainId) external payable;

/// Seen in src/interfaces/IRootBridgeAgent.sol
33:     function execute(bytes memory params, uint16 srcChainId) external payable;

/// Seen in src/interfaces/IRootBridgeAgent.sol
42:     function executeDepositSingle(bytes memory params, DepositParams memory dParams, uint16 srcChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
53:     function executeDepositMultiple(bytes memory params, DepositMultipleParams memory dParams, uint16 srcChainId)

/// Seen in src/interfaces/IRootBridgeAgent.sol
63:     function executeSigned(bytes memory params, address userAccount, uint16 srcChainId) external payable;

/// Seen in src/interfaces/IRootBridgeAgent.sol
72:     function executeSignedDepositSingle(

/// Seen in src/interfaces/IRootBridgeAgent.sol
86:     function executeSignedDepositMultiple(

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L25) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L33) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L42) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L53) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L63) [#L72](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L72) [#L86](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L86) 

```solidity
File: src/interfaces/IVirtualAccount.sol

/// Seen in src/interfaces/IRootBridgeAgent.sol
32:     function userAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
38:     function localPortAddress() external view returns (address);

/// Seen in src/interfaces/IRootBridgeAgent.sol
44:     function withdrawNative(uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
51:     function withdrawERC20(address _token, uint256 _amount) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
58:     function withdrawERC721(address _token, uint256 _tokenId) external;

/// Seen in src/interfaces/IRootBridgeAgent.sol
65:     function call(Call[] calldata callInput) external returns (bytes[] memory);

/// Seen in src/interfaces/IRootBridgeAgent.sol
73:     function payableCall(PayableCall[] calldata calls) external payable returns (bytes[] memory);

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L32) [#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L38) [#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L44) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L51) [#L58](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L58) [#L65](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L65) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L73) 

</details>

---

<a name="NC-43"></a> 
### [NC-43] Names of `private`/`internal` functions should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/RootPort.sol

359:     function addVirtualAccount(address _user) internal returns (VirtualAccount newAccount) {

```
[#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L359) 

```solidity
File: src/VirtualAccount.sol

147:     function isContract(address addr) internal view returns (bool) {

```
[#L147](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L147) 

</details>

---

<a name="NC-44"></a> 
### [NC-44] Names of `private`/`internal` state variables should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>23</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

64:     bytes private rootBridgeAgentPath;

```
[#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L64) 

```solidity
File: src/BranchPort.sol

97:     uint256 internal constant DIVISIONER = 1e4;

98:     uint256 internal constant MIN_RESERVE_RATIO = 3e3;

```
[#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L98) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

15:     uint8 internal constant STATUS_DONE = 1;

17:     uint8 internal constant STATUS_RETRIEVE = 2;

21:     uint8 internal constant STATUS_FAILED = 1;

23:     uint8 internal constant STATUS_SUCCESS = 0;

27:     uint256 internal constant PARAMS_START = 1;

29:     uint256 internal constant PARAMS_START_SIGNED = 21;

31:     uint256 internal constant PARAMS_TKN_START = 5;

33:     uint256 internal constant PARAMS_TKN_START_SIGNED = 25;

35:     uint256 internal constant PARAMS_ENTRY_SIZE = 32;

37:     uint256 internal constant PARAMS_ADDRESS_SIZE = 20;

39:     uint256 internal constant PARAMS_TKN_SET_SIZE = 109;

41:     uint256 internal constant PARAMS_TKN_SET_SIZE_MULTIPLE = 128;

43:     uint256 internal constant ADDRESS_END_OFFSET = 12;

45:     uint256 internal constant PARAMS_AMT_OFFSET = 64;

47:     uint256 internal constant PARAMS_DEPOSIT_OFFSET = 96;

49:     uint256 internal constant PARAMS_END_OFFSET = 6;

51:     uint256 internal constant PARAMS_END_SIGNED_OFFSET = 26;

53:     uint256 internal constant PARAMS_SETTLEMENT_OFFSET = 129;

57:     uint256 internal constant MAX_TOKENS_LENGTH = 255;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L15) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L17) [#L21](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L21) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) [#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L27) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L29) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L31) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L33) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L35) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L37) [#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L39) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L41) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L43) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L45) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L47) [#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L49) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L51) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L53) [#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L57) 

</details>

---

<a name="NC-45"></a> 
### [NC-45]  `require()` / `revert()` statements should have descriptive reason strings

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

213:         require(_unlocked == 1);

```
[#L213](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L213) 

```solidity
File: src/BranchBridgeAgent.sol

923:         require(_unlocked == 1);

```
[#L923](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L923) 

```solidity
File: src/BranchPort.sol

567:         require(_unlocked == 1);

```
[#L567](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L567) 

```solidity
File: src/MulticallRootRouter.sol

591:         require(_unlocked == 1);

```
[#L591](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L591) 

```solidity
File: src/RootBridgeAgent.sol

1191:         require(_unlocked == 1);

```
[#L1191](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1191) 

</details>

---

<a name="NC-46"></a> 
### [NC-46] Return values of `approve()` not checked
Not all IERC20 implementations `revert()` when there's a failure in `approve()`. The function signature has a boolean return value and they indicate errors that way instead. By not checking the return value, operations that should have marked as failed, may potentially go through without actually approving anything

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

168:                 ERC20(_hToken).approve(_localPortAddress, _amount - _deposit);

175:             ERC20(_token).approve(_localPortAddress, _deposit);

```
[#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L168) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L175) 

</details>

---

<a name="NC-47"></a> 
### [NC-47] Variables should be named in mixedCase style
As the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html#naming-styles) suggests: arguments, local variables and mutable state variables should be named in mixedCase style.

<details>
<summary>
There are <b>29</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

42:     uint256 internal _unlocked = 1;

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L42) 

```solidity
File: src/BranchBridgeAgent.sol

101:     uint256 internal _unlocked = 1;

```
[#L101](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L101) 

```solidity
File: src/BranchPort.sol

91:     uint256 internal _unlocked = 1;

97:     uint256 internal constant DIVISIONER = 1e4;

98:     uint256 internal constant MIN_RESERVE_RATIO = 3e3;

```
[#L91](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L91) [#L97](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L97) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L98) 

```solidity
File: src/CoreRootRouter.sol

44:     bool internal _setup;

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L44) 

```solidity
File: src/MulticallRootRouter.sol

80:     uint256 internal _unlocked = 1;

```
[#L80](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L80) 

```solidity
File: src/RootBridgeAgent.sol

92:     uint256 internal _unlocked = 1;

```
[#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L92) 

```solidity
File: src/RootPort.sol

24:     bool internal _setup;

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L24) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

15:     uint8 internal constant STATUS_DONE = 1;

17:     uint8 internal constant STATUS_RETRIEVE = 2;

21:     uint8 internal constant STATUS_FAILED = 1;

23:     uint8 internal constant STATUS_SUCCESS = 0;

27:     uint256 internal constant PARAMS_START = 1;

29:     uint256 internal constant PARAMS_START_SIGNED = 21;

31:     uint256 internal constant PARAMS_TKN_START = 5;

33:     uint256 internal constant PARAMS_TKN_START_SIGNED = 25;

35:     uint256 internal constant PARAMS_ENTRY_SIZE = 32;

37:     uint256 internal constant PARAMS_ADDRESS_SIZE = 20;

39:     uint256 internal constant PARAMS_TKN_SET_SIZE = 109;

41:     uint256 internal constant PARAMS_TKN_SET_SIZE_MULTIPLE = 128;

43:     uint256 internal constant ADDRESS_END_OFFSET = 12;

45:     uint256 internal constant PARAMS_AMT_OFFSET = 64;

47:     uint256 internal constant PARAMS_DEPOSIT_OFFSET = 96;

49:     uint256 internal constant PARAMS_END_OFFSET = 6;

51:     uint256 internal constant PARAMS_END_SIGNED_OFFSET = 26;

53:     uint256 internal constant PARAMS_SETTLEMENT_OFFSET = 129;

57:     uint256 internal constant MAX_TOKENS_LENGTH = 255;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L15) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L17) [#L21](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L21) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) [#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L27) [#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L29) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L31) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L33) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L35) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L37) [#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L39) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L41) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L43) [#L45](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L45) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L47) [#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L49) [#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L51) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L53) [#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L57) 

</details>

---

<a name="NC-48"></a> 
### [NC-48] Event is missing `indexed` fields
Index event fields make the field more quickly accessible to off-chain tools that parse events. However, note that each index field costs extra gas during emission, so it's not necessarily best to index the maximum allowed per event (three fields). Each event should use three indexed fields if there are three or more fields, and gas usage is not particularly of concern for the events in question. If there are fewer than three fields, all of the fields should be indexed.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: src/interfaces/IBranchPort.sol

220:     event DebtCreated(address indexed _strategy, address indexed _token, uint256 _amount);

221:     event DebtRepaid(address indexed _strategy, address indexed _token, uint256 _amount);

```
[#L220](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L220) [#L221](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L221) 

```solidity
File: src/interfaces/IRootPort.sol

380:     event VirtualAccountCreated(address indexed user, address account);

```
[#L380](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L380) 

</details>

---

<a name="NC-49"></a> 
### [NC-49] Functions not used internally could be marked external

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

578:     function lzReceive(uint16, bytes calldata _srcAddress, uint64, bytes calldata _payload) public override {

587:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload)

```
[#L578](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L578) [#L587](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L587) 

```solidity
File: src/BranchPort.sol

135:     function renounceOwnership() public payable override onlyOwner {

```
[#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L135) 

```solidity
File: src/RootBridgeAgent.sol

423:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64, bytes calldata _payload) public {

434:     function lzReceiveNonBlocking(

```
[#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L423) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L434) 

```solidity
File: src/RootPort.sol

166:     function renounceOwnership() public payable override onlyOwner {

```
[#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L166) 

```solidity
File: src/VirtualAccount.sol

85:     function payableCall(PayableCall[] calldata calls) public payable returns (bytes[] memory returnData) {

```
[#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L85) 

```solidity
File: src/token/ERC20hTokenBranch.sol

35:     function burn(uint256 amount) public override onlyOwner {

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L35) 

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
File: src/BranchBridgeAgent.sol

176:                     USER / BRANCH ROUTER EXTERNAL FUNCTIONS

```
[#L176](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L176) 

```solidity
File: src/BranchPort.sol

473:         return ((_currBalance + _strategyTokenDebt) * getMinimumTokenReserveRatio[_token]) / DIVISIONER;

490:                 lastManaged[msg.sender][_token] = (block.timestamp / 1 days) * 1 days;

```
[#L473](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L473) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L490) 

```solidity
File: src/CoreRootRouter.sol

145:                 GOVERNANCE / ADMIN EXTERNAL FUNCTIONS

```
[#L145](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L145) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

25:     address token; //Input Native / underlying Token Address.

33:     address[] tokens; //Input Native / underlying Token Address.

43:     address[] tokens; //Input Native / underlying Token Address.

52:     address token; //Input Native / underlying Token Address.

63:     address[] tokens; //Input Native / underlying Token Addresses.

84:     address token; // Input Native / underlying Token Address.

94:     address[] tokens; // Input Native / underlying Token Addresses.

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L25) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L33) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L43) [#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L52) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L63) [#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L84) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L94) 

```solidity
File: src/interfaces/IBranchRouter.sol

23:                             VIEW / STATE

```
[#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L23) 

</details>

---

<a name="GAS-3"></a> 
### [GAS-3] Operator `+=` costs more gas than `<x> = <x> + <y>` for state variables

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

157:         getPortStrategyTokenDebt[msg.sender][_token] += _amount;

169:         getPortStrategyTokenDebt[msg.sender][_token] -= _amount;

172:         getStrategyTokenDebt[_token] -= _amount;

```
[#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L157) [#L169](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L169) [#L172](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L172) 

```solidity
File: src/VirtualAccount.sol

96:                 valAccumulator += val;

```
[#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L96) 

```solidity
File: src/token/ERC20hTokenRoot.sol

58:         getTokenBalance[chainId] += amount;

70:         getTokenBalance[chainId] -= amount;

```
[#L58](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L58) [#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L70) 

</details>

---

<a name="GAS-4"></a> 
### [GAS-4] Duplicated `require()`/`revert()` checks should be refactored to a modifier or function to save gas
Saves deployment costs.

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

/// Duplicated on line 135
124:         revert UnrecognizedFunctionId();

```
[#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L124) 

```solidity
File: src/CoreRootRouter.sol

/// Duplicated on line 345
327:             revert UnrecognizedFunctionId();

/// Duplicated on line 366
356:         revert();

/// Duplicated on line 381
371:         revert();

```
[#L327](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L327) [#L356](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L356) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L371) 

```solidity
File: src/MulticallRootRouter.sol

/// Duplicated on line 204
124:         revert();

/// Duplicated on line 298
198:             revert UnrecognizedFunctionId();

/// Duplicated on line 475
387:             revert UnrecognizedFunctionId();

```
[#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L124) [#L198](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L198) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L387) 

```solidity
File: src/RootBridgeAgent.sol

/// Duplicated on line 287
249:                 revert NotSettlementOwner();

/// Duplicated on line 675
313:                 revert NotSettlementOwner();

/// Duplicated on line 372
365:                 revert InvalidInputParams();

/// Duplicated on line 473
450:                 revert AlreadyExecutedTransaction();

/// Duplicated on line 519
496:                 revert AlreadyExecutedTransaction();

/// Duplicated on line 583
545:                 revert AlreadyExecutedTransaction();

/// Duplicated on line 705
623:                 revert AlreadyExecutedTransaction();

```
[#L249](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L249) [#L313](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L313) [#L365](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L365) [#L450](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L450) [#L496](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L496) [#L545](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L545) [#L623](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L623) 

```solidity
File: src/RootPort.sol

/// Duplicated on line 494
489:             revert AlreadyAddedEcosystemToken();

```
[#L489](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L489) 

</details>

---

<a name="GAS-5"></a> 
### [GAS-5] Increments can be `unchecked` to save gas
Using `unchecked` increments can save gas by bypassing the built-in overflow checks. This can save 30-40 gas per iteration. So it is recommended to use unchecked increments when overflow is not possible.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

196:                 ++i;

```
[#L196](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L196) 

```solidity
File: src/BranchBridgeAgent.sol

451:                 ++i;

564:                 ++i;

```
[#L451](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L451) [#L564](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L564) 

```solidity
File: src/BranchPort.sol

271:                 ++i;

```
[#L271](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L271) 

```solidity
File: src/MulticallRootRouter.sol

282:                     ++i;

371:                     ++i;

459:                     ++i;

561:                 ++i;

```
[#L282](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L282) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L371) [#L459](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L459) [#L561](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L561) 

```solidity
File: src/RootBridgeAgent.sol

338:                 ++i;

413:                 ++i;

1084:                 ++i;

```
[#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L338) [#L413](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L413) [#L1084](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1084) 

```solidity
File: src/RootBridgeAgentExecutor.sol

333:                 ++i;

```
[#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L333) 

```solidity
File: src/VirtualAccount.sol

79:                 ++i;

106:                 ++i;

```
[#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L79) [#L106](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L106) 

</details>

---

<a name="GAS-6"></a> 
### [GAS-6] Initializers can be marked as payable to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. Initializers can be safely marked as payable, because only the deployer or the factory contract would call the function without carrying any funds.

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

60:     function initialize(address _localBridgeAgentAddress) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L60) 

```solidity
File: src/BranchPort.sol

122:     function initialize(address _coreBranchRouter, address _bridgeAgentFactory) external virtual onlyOwner {

```
[#L122](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L122) 

```solidity
File: src/CoreRootRouter.sol

83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) 

```solidity
File: src/MulticallRootRouter.sol

109:     function initialize(address _bridgeAgentAddress) external onlyOwner {

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L109) 

```solidity
File: src/RootPort.sol

129:     function initialize(address _bridgeAgentFactory, address _coreRootRouter) external onlyOwner {

```
[#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L129) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

```
[#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

87:     function initialize(address _coreRootBridgeAgent) external virtual onlyOwner {

```
[#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L87) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

49:     function initialize(address _coreRouter) external onlyOwner {

```
[#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L49) 

</details>

---

<a name="GAS-7"></a> 
### [GAS-7] `internal` functions only called once can be inlined to save gas
If an `internal` function is only used once, there is no need to modularize it, unless the function calling it would otherwise be too long and complex. Not inlining costs 20 to 40 gas because of two extra JUMP instructions and additional stack operations needed for function calls.

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// `_requiresEndpoint` is used only once
125:     function _requiresEndpoint(address _endpoint, bytes calldata) internal view override {

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L125) 

```solidity
File: src/BaseBranchRouter.sol

/// `_transferAndApproveMultipleTokens` is used only once
186:     function _transferAndApproveMultipleTokens(

```
[#L186](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L186) 

```solidity
File: src/BranchBridgeAgent.sol

/// `_requiresEndpoint` is used only once
936:     function _requiresEndpoint(address _endpoint, bytes calldata _srcAddress) internal view virtual {

```
[#L936](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L936) 

```solidity
File: src/BranchPort.sol

/// `_excessReserves` is used only once
435:     function _excessReserves(uint256 _strategyTokenDebt, address _token) internal view returns (uint256) {

/// `_reservesLacking` is used only once
449:     function _reservesLacking(uint256 _strategyTokenDebt, address _token, uint256 currBalance)

/// `_checkTimeLimit` is used only once
485:     function _checkTimeLimit(address _token, uint256 _amount) internal {

```
[#L435](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L435) [#L449](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L449) [#L485](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L485) 

```solidity
File: src/CoreBranchRouter.sol

/// `_receiveAddGlobalToken` is used only once
166:     function _receiveAddGlobalToken(

```
[#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L166) 

```solidity
File: src/CoreRootRouter.sol

/// `_addGlobalToken` is used only once
406:     function _addGlobalToken(

/// `_addLocalToken` is used only once
452:     function _addLocalToken(

/// `_setLocalToken` is used only once
481:     function _setLocalToken(address _globalAddress, address _localAddress, uint16 _dstChainId) internal {

/// `_syncBranchBridgeAgent` is used only once
500:     function _syncBranchBridgeAgent(address _newBranchBridgeAgent, address _rootBridgeAgent, uint256 _srcChainId)

```
[#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L406) [#L452](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L452) [#L481](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L481) [#L500](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L500) 

```solidity
File: src/MulticallRootRouter.sol

/// `_requiresExecutor` is used only once
604:     function _requiresExecutor() internal view {

```
[#L604](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L604) 

```solidity
File: src/RootBridgeAgent.sol

/// `_createSettlement` is used only once
966:     function _createSettlement(

/// `_createSettlementMultiple` is used only once
1045:     function _createSettlementMultiple(

```
[#L966](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L966) [#L1045](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1045) 

```solidity
File: src/RootPort.sol

/// `addVirtualAccount` is used only once
359:     function addVirtualAccount(address _user) internal returns (VirtualAccount newAccount) {

```
[#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L359) 

</details>

---

<a name="GAS-8"></a> 
### [GAS-8] Low level `call` can be optimized with assembly
When using low-level calls, the `returnData` is copied to memory even if the variable is not utilized. The proper way to handle this is through a low level assembly call.

<details>
<summary>
There are <b>16</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

103:         _rootBridgeAgentAddress.call{value: msg.value}("");

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L103) 

```solidity
File: src/BranchBridgeAgent.sol

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

```
[#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) [#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) 

```solidity
File: src/MulticallRootRouter.sol

239:             IVirtualAccount(userAccount).call(calls);

248:             IVirtualAccount(userAccount).call(calls);

275:             IVirtualAccount(userAccount).call(calls);

328:             IVirtualAccount(userAccount).call(calls);

337:             IVirtualAccount(userAccount).call(calls);

364:             IVirtualAccount(userAccount).call(calls);

416:             IVirtualAccount(userAccount).call(calls);

425:             IVirtualAccount(userAccount).call(calls);

452:             IVirtualAccount(userAccount).call(calls);

```
[#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L239) [#L248](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L248) [#L275](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L275) [#L328](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L328) [#L337](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L337) [#L364](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L364) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L416) [#L425](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L425) [#L452](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L452) 

```solidity
File: src/RootBridgeAgent.sol

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

835:             callee.call{value: msg.value}("");

927:             callee.call{value: _value}("");

```
[#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L835](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L835) [#L927](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L927) 

</details>

---

<a name="GAS-9"></a> 
### [GAS-9] Multiple accesses of the same mapping/array key/index should be cached
The instances below point to the second+ access of a value inside a mapping/array, within a function. Caching a mapping's value in a local `storage` or `calldata` variable when the value is accessed [multiple times](https://gist.github.com/IllIllI000/ec23a57daa30a8f8ca8b9681c8ccefb0), saves ~42 gas per access due to not having to recalculate the key's keccak256 hash (Gkeccak256 - 30 gas) and that calculation's associated stack operations. Caching an array's struct avoids recalculating the array offsets into memory/calldata

<details>
<summary>
There are <b>27</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

/// `getDeposit[_depositNonce]` is also accessed on line 436
456:         delete getDeposit[_depositNonce];

/// `executionState[nonce]` is also accessed on line 604
624:             if (executionState[nonce] != STATUS_READY) revert AlreadyExecutedTransaction();

/// `executionState[nonce]` is also accessed on line 604
646:             if (executionState[nonce] != STATUS_READY) revert AlreadyExecutedTransaction();

/// `executionState[nonce]` is also accessed on line 604
671:             if (executionState[nonce] == STATUS_DONE) {

/// `executionState[nonce]` is also accessed on line 604
675:                 if (executionState[nonce] == STATUS_READY) executionState[nonce] = STATUS_RETRIEVE;

```
[#L456](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L456) [#L624](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L624) [#L646](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L646) [#L671](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L671) [#L675](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L675) 

```solidity
File: src/BranchPort.sol

/// `isBridgeAgentFactory[_bridgeAgentFactory]` is also accessed on line 124
130:         isBridgeAgentFactory[_bridgeAgentFactory] = true;

/// `isBridgeAgentFactory[_bridgeAgentFactory]` is also accessed on line 124
130:         isBridgeAgentFactory[_bridgeAgentFactory] = true;

/// `getStrategyTokenDebt[_token]` is also accessed on line 146
155:         getStrategyTokenDebt[_token] = _strategyTokenDebt + _amount;

/// `getPortStrategyTokenDebt[msg.sender]` is also accessed on line 157
169:         getPortStrategyTokenDebt[msg.sender][_token] -= _amount;

/// `getStrategyTokenDebt[_token]` is also accessed on line 146
172:         getStrategyTokenDebt[_token] -= _amount;

/// `getStrategyTokenDebt[_token]` is also accessed on line 146
190:         uint256 strategyTokenDebt = getStrategyTokenDebt[_token];

/// `getPortStrategyTokenDebt[_strategy]` is also accessed on line 199
205:         getPortStrategyTokenDebt[_strategy][_token] = portStrategyTokenDebt - amountToWithdraw;

/// `getStrategyTokenDebt[_token]` is also accessed on line 146
207:         getStrategyTokenDebt[_token] = strategyTokenDebt - amountToWithdraw;

/// `isBridgeAgent[_bridgeAgent]` is also accessed on line 320
322:         isBridgeAgent[_bridgeAgent] = true;

/// `isBridgeAgentFactory[_newBridgeAgentFactory]` is also accessed on line 339
341:         isBridgeAgentFactory[_newBridgeAgentFactory] = true;

/// `lastManaged[msg.sender]` is also accessed on line 487
490:                 lastManaged[msg.sender][_token] = (block.timestamp / 1 days) * 1 days;

/// `lastManaged[msg.sender]` is also accessed on line 487
490:                 lastManaged[msg.sender][_token] = (block.timestamp / 1 days) * 1 days;

/// `strategyDailyLimitRemaining[msg.sender]` is also accessed on line 486
493:         strategyDailyLimitRemaining[msg.sender][_token] = dailyLimit - _amount;

/// `strategyDailyLimitRemaining[msg.sender]` is also accessed on line 486
493:         strategyDailyLimitRemaining[msg.sender][_token] = dailyLimit - _amount;

```
[#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L130) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L130) [#L155](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L155) [#L169](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L169) [#L172](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L172) [#L190](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L190) [#L205](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L205) [#L207](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L207) [#L322](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L322) [#L341](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L341) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L490) [#L490](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L490) [#L493](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L493) [#L493](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L493) 

```solidity
File: src/RootBridgeAgent.sol

/// `getSettlement[_settlementNonce]` is also accessed on line 301
343:         delete getSettlement[_settlementNonce];

```
[#L343](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L343) 

```solidity
File: src/RootPort.sol

/// `getUserAccount[_user]` is also accessed on line 351
363:         getUserAccount[_user] = newAccount;

/// `isBridgeAgent[_bridgeAgent]` is also accessed on line 383
387:         isBridgeAgent[_bridgeAgent] = true;

/// `isBridgeAgent[_bridgeAgent]` is also accessed on line 383
387:         isBridgeAgent[_bridgeAgent] = true;

/// `isBridgeAgent[_bridgeAgent]` is also accessed on line 383
387:         isBridgeAgent[_bridgeAgent] = true;

/// `isBridgeAgentFactory[_bridgeAgentFactory]` is also accessed on line 422
425:         isBridgeAgentFactory[_bridgeAgentFactory] = true;

/// `isChainId[_chainId]` is also accessed on line 448
465:         isChainId[_chainId] = true;

/// `isGlobalAddress[_ecoTokenGlobalAddress]` is also accessed on line 485
499:         isGlobalAddress[_ecoTokenGlobalAddress] = true;

```
[#L363](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L363) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L387) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L387) [#L387](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L387) [#L425](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L425) [#L465](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L465) [#L499](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L499) 

</details>

---

<a name="GAS-10"></a> 
### [GAS-10] Newer versions of solidity are more gas efficient
The solidity language continues to pursue more efficient gas optimization schemes. Adopting a newer version of solidity can be more gas efficient.

<details>
<summary>
There are <b>44</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L2) 

```solidity
File: src/ArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L3) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L2) 

```solidity
File: src/BaseBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L2) 

```solidity
File: src/BranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L2) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L2) 

```solidity
File: src/BranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L3) 

```solidity
File: src/CoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L2) 

```solidity
File: src/CoreRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouterLibZip.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L2) 

```solidity
File: src/RootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L2) 

```solidity
File: src/RootBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L2) 

```solidity
File: src/RootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L3) 

```solidity
File: src/VirtualAccount.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L3) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L2) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L2) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L3) 

```solidity
File: src/interfaces/IMulticall2.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L2) 

```solidity
File: src/interfaces/IPortStrategy.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L3) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IRootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L3) 

```solidity
File: src/interfaces/IRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L2) 

```solidity
File: src/interfaces/IVirtualAccount.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L2) 

```solidity
File: src/token/ERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L2) 

```solidity
File: src/token/ERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L2) 

</details>

---

<a name="GAS-11"></a> 
### [GAS-11] Operator `>=`/`<=` costs less gas than operator `>`/`<`
The compiler uses opcodes `GT` and `ISZERO` for code that uses `>`, but only requires `LT` for `>=`. A similar behavior applies for `>`, which uses opcodes `LT` and `ISZERO`, but only requires `GT` for `<=`. It can save 3 gas for each. It should be converted to the `<=`/`>=` equivalent when comparing against integer literals.

<details>
<summary>
There are <b>48</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

127:         if (_deposit > 0) {

132:         if (_amount - _deposit > 0) {

```
[#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L127) [#L132](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L132) 

```solidity
File: src/BaseBranchRouter.sol

165:         if (_amount - _deposit > 0) {

173:         if (_deposit > 0) {

192:         for (uint256 i = 0; i < _hTokens.length;) {

```
[#L165](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L165) [#L173](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L173) [#L192](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L192) 

```solidity
File: src/BranchBridgeAgent.sol

447:         for (uint256 i = 0; i < deposit.tokens.length;) {

513:         for (uint256 i = 0; i < numOfAssets;) {

869:         if (_hTokens.length > MAX_TOKENS_LENGTH) revert InvalidInput();

906:         if (_amount - _deposit > 0) {

912:         if (_deposit > 0) {

```
[#L447](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L447) [#L513](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L513) [#L869](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L869) [#L906](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L906) [#L912](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L912) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

87:         if (_payload.length > PARAMS_SETTLEMENT_OFFSET) {

119:         if (_payload.length > settlementEndOffset) {

```
[#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L87) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L119) 

```solidity
File: src/BranchPort.sol

149:         if (_amount > _excessReserves(_strategyTokenDebt, _token)) revert InsufficientReserves();

202:         uint256 amountToWithdraw = portStrategyTokenDebt < reservesLacking ? portStrategyTokenDebt : reservesLacking;

257:         for (uint256 i = 0; i < length;) {

299:         if (length > 255) revert InvalidInputArrays();

305:         for (uint256 i = 0; i < length;) {

363:         if (_minimumReservesRatio >= DIVISIONER || _minimumReservesRatio < MIN_RESERVE_RATIO) {

440:             return currBalance > minReserves ? currBalance - minReserves : 0;

457:             return currBalance < minReserves ? minReserves - currBalance : 0;

525:         if (_hTokenAmount > 0) {

531:         if (_deposit > 0) {

```
[#L149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L149) [#L202](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L202) [#L257](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L257) [#L299](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L299) [#L305](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L305) [#L363](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L363) [#L440](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L440) [#L457](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L457) [#L525](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L525) [#L531](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L531) 

```solidity
File: src/MulticallRootRouter.sol

278:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

367:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

455:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

557:         for (uint256 i = 0; i < outputTokens.length;) {

```
[#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L278) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L367) [#L455](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L455) [#L557](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L557) 

```solidity
File: src/RootBridgeAgent.sol

318:         for (uint256 i = 0; i < settlement.hTokens.length;) {

357:         if (_dParams.amount < _dParams.deposit) revert InvalidInputParams();

363:         if (_dParams.amount > 0) {

370:         if (_dParams.deposit > 0) {

396:         if (length > MAX_TOKENS_LENGTH) revert InvalidInputParams();

399:         for (uint256 i = 0; i < length;) {

891:         } else if (_hTokens.length > 1) {

1057:         if (_globalAddresses.length > MAX_TOKENS_LENGTH) revert InvalidInputParamsLength();

1070:         for (uint256 i = 0; i < hTokens.length;) {

1142:         if (_amount < _deposit) revert InvalidInputParams();

1146:         if (_underlyingAddress == address(0)) if (_deposit > 0) revert UnrecognizedUnderlyingAddress();

1149:         if (_amount - _deposit > 0) {

1156:         if (_deposit > 0) {

```
[#L318](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L318) [#L357](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L357) [#L363](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L363) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L370) [#L396](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L396) [#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L399) [#L891](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L891) [#L1057](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1057) [#L1070](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1070) [#L1142](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1142) [#L1146](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1146) [#L1149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1149) [#L1156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1156) 

```solidity
File: src/RootBridgeAgentExecutor.sol

100:         if (_payload.length > PARAMS_TKN_SET_SIZE) {

134:         if (length > PARAMS_END_OFFSET + (numOfAssets * PARAMS_TKN_SET_SIZE_MULTIPLE)) {

185:         if (_payload.length > PARAMS_SETTLEMENT_OFFSET) {

281:         for (uint256 i = 0; i < uint256(uint8(numOfAssets));) {

```
[#L100](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L100) [#L134](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L134) [#L185](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L185) [#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L281) 

```solidity
File: src/RootPort.sol

284:         if (_amount - _deposit > 0) {

290:         if (_deposit > 0) if (!ERC20hTokenRoot(_hToken).mint(_recipient, _deposit, _srcChainId)) revert UnableToMint();

```
[#L284](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L284) [#L290](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L290) 

```solidity
File: src/VirtualAccount.sol

70:         for (uint256 i = 0; i < length;) {

90:         for (uint256 i = 0; i < length;) {

152:         return size > 0;

```
[#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L70) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L90) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L152) 

</details>

---

<a name="GAS-12"></a> 
### [GAS-12] Reduce gas usage by moving to Solidity 0.8.19 or later
Solidity version 0.8.19 introduced a number of gas optimizations, refer to the [Solidity 0.8.19 Release Announcement](https://soliditylang.org/blog/2023/02/22/solidity-0.8.19-release-announcement/) for details.

<details>
<summary>
There are <b>41</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L2) 

```solidity
File: src/ArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L3) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L2) 

```solidity
File: src/BaseBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L2) 

```solidity
File: src/BranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L2) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L2) 

```solidity
File: src/BranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L3) 

```solidity
File: src/CoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L2) 

```solidity
File: src/CoreRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouterLibZip.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L2) 

```solidity
File: src/RootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L2) 

```solidity
File: src/RootBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L2) 

```solidity
File: src/RootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L3) 

```solidity
File: src/VirtualAccount.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L3) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L2) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L2) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/interfaces/IMulticall2.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L2) 

```solidity
File: src/interfaces/IPortStrategy.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L3) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IRootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L3) 

```solidity
File: src/interfaces/IRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L2) 

```solidity
File: src/interfaces/IVirtualAccount.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L2) 

```solidity
File: src/token/ERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L2) 

```solidity
File: src/token/ERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L2) 

</details>

---

<a name="GAS-13"></a> 
### [GAS-13] Redundant state variable getters
Getters for public state variables are automatically generated so there is no need to code them manually and waste gas.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

87:     function getHTokens() external view returns (ERC20hTokenBranch[] memory) {
            return hTokens;

```
[#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L87) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

63:     function getHTokens() external view returns (ERC20hTokenRoot[] memory) {
            return hTokens;

```
[#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L63) 

</details>

---

<a name="GAS-14"></a> 
### [GAS-14] Remove or replace unused state variables
Saves a storage slot. If the variable is assigned a non-zero value, saves Gsset (20000 gas). If it's assigned a zero value, saves Gsreset (2900 gas). If the variable remains unassigned, there is no gas savings unless the variable is `public`, in which case the compiler-generated non-payable getter deployment cost is saved. If the state variable is overriding an interface's public function, mark the variable as `constant` or `immutable` so that it does not use a storage slot.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

98:     uint256 internal constant MIN_RESERVE_RATIO = 3e3;

```
[#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L98) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

49:     uint256 internal constant PARAMS_END_OFFSET = 6;

```
[#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L49) 

</details>

---

<a name="GAS-15"></a> 
### [GAS-15] `require()`/`revert()` strings longer than 32 bytes cost extra gas
Each extra memory word of bytes past the original 32 [incurs an MSTORE](https://gist.github.com/hrkrshnn/ee8fabd532058307229d65dcd5836ddc#consider-having-short-revert-strings) which costs 3 gas

<details>
<summary>
There are <b>22</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

125:         require(_rootBridgeAgentAddress != address(0), "Root Bridge Agent Address cannot be the zero address.");

126:         require(
                 _lzEndpointAddress != address(0) || _rootChainId == _localChainId,
                 "Layerzero Endpoint Address cannot be the zero address."

130:         require(_localRouterAddress != address(0), "Local Router Address cannot be the zero address.");

131:         require(_localPortAddress != address(0), "Local Port Address cannot be the zero address.");

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L125) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L126) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L131) 

```solidity
File: src/BranchPort.sol

127:         require(_bridgeAgentFactory != address(0), "BridgeAgentFactory is zero address");

```
[#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L127) 

```solidity
File: src/RootBridgeAgent.sol

111:         require(_lzEndpointAddress != address(0), "Layerzero Enpoint Address cannot be zero address");

112:         require(_localPortAddress != address(0), "Port Address cannot be zero address");

113:         require(_localRouterAddress != address(0), "Router Address cannot be zero address");

```
[#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L111) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L112) [#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L113) 

```solidity
File: src/RootPort.sol

130:         require(_bridgeAgentFactory != address(0), "Bridge Agent Factory cannot be 0 address.");

131:         require(_coreRootRouter != address(0), "Core Root Router cannot be 0 address.");

152:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0 address.");

153:         require(_coreLocalBranchBridgeAgent != address(0), "Core Local Branch Bridge Agent cannot be 0 address.");

154:         require(_localBranchPortAddress != address(0), "Local Branch Port Address cannot be 0 address.");

```
[#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L131) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L152) [#L153](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L153) [#L154](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L154) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

57:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent Address cannot be 0");

84:         require(
                msg.sender == localCoreBranchRouterAddress, "Only the Core Branch Router can create a new Bridge Agent."

87:         require(
                _rootBridgeAgentFactoryAddress == rootBridgeAgentFactoryAddress,
                "Root Bridge Agent Factory Address does not match."

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L57) [#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L84) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L87) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

61:         require(_rootBridgeAgentFactoryAddress != address(0), "Root Bridge Agent Factory Address cannot be 0");

62:         require(
                _lzEndpointAddress != address(0) || _rootChainId == _localChainId,
                "Layerzero Endpoint Address cannot be the zero address."

66:         require(_localCoreBranchRouterAddress != address(0), "Core Branch Router Address cannot be 0");

88:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0");

120:         require(
                 msg.sender == localCoreBranchRouterAddress, "Only the Core Branch Router can create a new Bridge Agent."

123:         require(
                 _rootBridgeAgentFactoryAddress == rootBridgeAgentFactoryAddress,
                 "Root Bridge Agent Factory Address does not match."

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L61) [#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L62) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L66) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L88) [#L120](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L120) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L123) 

</details>

---

<a name="GAS-16"></a> 
### [GAS-16] The result of a function call should be cached rather than re-calling the function
The function calls in solidity are expensive. If the same result of the same function calls are to be used several times, the result should be cached to reduce the gas consumption of repeated calls.

<details>
<summary>
There are <b>55</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

/// `LayerZeroUnauthorizedEndpoint` is called 2 times
125:     function _requiresEndpoint(address _endpoint, bytes calldata) internal view override {

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L125) 

```solidity
File: src/ArbitrumBranchPort.sol

/// `IRootPort` is called 2 times
50:     function depositToPort(address _depositor, address _recipient, address _underlyingAddress, uint256 _deposit)
            external
            override
            lock
            requiresBridgeAgent
        {

/// `IRootPort` is called 3 times
73:     function withdrawFromPort(address _depositor, address _recipient, address _globalAddress, uint256 _amount)
            external
            override
            lock
            requiresBridgeAgent
        {

```
[#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L50) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L73) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

/// `ERC20` is called 3 times
51:     function addLocalToken(address _underlyingAddress, GasParams calldata) external payable override {

/// `IPort` is called 2 times
85:     function _receiveAddBridgeAgent(
            address _newBranchRouter,
            address _branchBridgeAgentFactory,
            address _rootBridgeAgent,
            address _rootBridgeAgentFactory,
            address _refundee,
            GasParams memory _gParams
        ) internal override {

```
[#L51](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L51) [#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L85) 

```solidity
File: src/BaseBranchRouter.sol

/// `IBridgeAgent` is called 2 times
60:     function initialize(address _localBridgeAgentAddress) external onlyOwner {

/// `ERC20` is called 2 times
160:     function _transferAndApproveToken(address _hToken, address _token, uint256 _amount, uint256 _deposit) internal {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L60) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L160) 

```solidity
File: src/BranchBridgeAgent.sol

/// `DepositRedeemUnavailable` is called 2 times
434:     function redeemDeposit(uint32 _depositNonce) external override lock {

/// `AlreadyExecutedTransaction` is called 4 times
587:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload)
             public
             override
             requiresEndpoint(_endpoint, _srcAddress)
         {

/// `_execute` is called 2 times
587:     function lzReceiveNonBlocking(address _endpoint, bytes calldata _srcAddress, bytes calldata _payload)
             public
             override
             requiresEndpoint(_endpoint, _srcAddress)
         {

/// `InvalidInput` is called 4 times
860:     function _createDepositMultiple(
             uint32 _depositNonce,
             address payable _refundee,
             address[] memory _hTokens,
             address[] memory _tokens,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) internal {

/// `IPort` is called 2 times
903:     function _clearToken(address _recipient, address _hToken, address _token, uint256 _amount, uint256 _deposit)
             internal
         {

/// `LayerZeroUnauthorizedEndpoint` is called 2 times
936:     function _requiresEndpoint(address _endpoint, bytes calldata _srcAddress) internal view virtual {

/// `LayerZeroUnauthorizedCaller` is called 2 times
936:     function _requiresEndpoint(address _endpoint, bytes calldata _srcAddress) internal view virtual {

```
[#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L434) [#L587](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L587) [#L587](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L587) [#L860](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L860) [#L903](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L903) [#L936](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L936) [#L936](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L936) 

```solidity
File: src/BranchPort.sol

/// `ERC20` is called 2 times
167:     function replenishReserves(address _token, uint256 _amount) external override lock {

/// `ERC20` is called 2 times
188:     function replenishReserves(address _strategy, address _token) external override lock {

/// `InvalidInputArrays` is called 4 times
288:     function bridgeOutMultiple(
             address _depositor,
             address[] memory _localAddresses,
             address[] memory _underlyingAddresses,
             uint256[] memory _amounts,
             uint256[] memory _deposits
         ) external override lock requiresBridgeAgent {

```
[#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L167) [#L188](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L188) [#L288](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L288) 

```solidity
File: src/CoreBranchRouter.sol

/// `ERC20` is called 3 times
62:     function addLocalToken(address _underlyingAddress, GasParams calldata _gParams) external payable virtual {

/// `IPort` is called 2 times
199:     function _receiveAddBridgeAgent(
             address _newBranchRouter,
             address _branchBridgeAgentFactory,
             address _rootBridgeAgent,
             address _rootBridgeAgentFactory,
             address _refundee,
             GasParams memory _gParams
         ) internal virtual {

/// `IPort` is called 3 times
244:     function _toggleBranchBridgeAgentFactory(address _newBridgeAgentFactoryAddress) internal {

/// `IPort` is called 2 times
263:     function _removeBranchBridgeAgent(address _branchBridgeAgent) internal {

/// `IPort` is called 3 times
284:     function _manageStrategyToken(address _underlyingToken, uint256 _minimumReservesRatio) internal {

/// `IPort` is called 4 times
307:     function _managePortStrategy(
             address _portStrategy,
             address _underlyingToken,
             uint256 _dailyManagementLimit,
             bool _isUpdateDailyLimit
         ) internal {

```
[#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L62) [#L199](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L199) [#L244](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L244) [#L263](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L263) [#L284](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L284) [#L307](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L307) 

```solidity
File: src/CoreRootRouter.sol

/// `IPort` is called 2 times
103:     function addBranchToBridgeAgent(
             address _rootBridgeAgent,
             address _branchBridgeAgentFactory,
             address _newBranchRouter,
             address _refundee,
             uint16 _dstChainId,
             GasParams[2] calldata _gParams
         ) external payable {

/// `InvalidChainId` is called 2 times
103:     function addBranchToBridgeAgent(
             address _rootBridgeAgent,
             address _branchBridgeAgentFactory,
             address _newBranchRouter,
             address _refundee,
             uint16 _dstChainId,
             GasParams[2] calldata _gParams
         ) external payable {

/// `IBridgeAgent` is called 4 times
103:     function addBranchToBridgeAgent(
             address _rootBridgeAgent,
             address _branchBridgeAgentFactory,
             address _newBranchRouter,
             address _refundee,
             uint16 _dstChainId,
             GasParams[2] calldata _gParams
         ) external payable {

/// `IPort` is called 2 times
406:     function _addGlobalToken(
             address _refundee,
             address _globalAddress,
             uint16 _dstChainId,
             GasParams[2] memory _gParams
         ) internal {

/// `ERC20` is called 3 times
406:     function _addGlobalToken(
             address _refundee,
             address _globalAddress,
             uint16 _dstChainId,
             GasParams[2] memory _gParams
         ) internal {

/// `IPort` is called 4 times
452:     function _addLocalToken(
             address _underlyingAddress,
             address _localAddress,
             string memory _name,
             string memory _symbol,
             uint8 _decimals,
             uint16 _srcChainId
         ) internal {

/// `TokenAlreadyAdded` is called 3 times
452:     function _addLocalToken(
             address _underlyingAddress,
             address _localAddress,
             string memory _name,
             string memory _symbol,
             uint8 _decimals,
             uint16 _srcChainId
         ) internal {

/// `IPort` is called 2 times
481:     function _setLocalToken(address _globalAddress, address _localAddress, uint16 _dstChainId) internal {

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L103) [#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L103) [#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L103) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L406) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L406) [#L452](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L452) [#L452](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L452) [#L481](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L481) 

```solidity
File: src/MulticallRootRouter.sol

/// `_decode` is called 3 times
137:     function execute(bytes calldata encodedData, uint16) external payable override lock requiresExecutor {

/// `_multicall` is called 3 times
137:     function execute(bytes calldata encodedData, uint16) external payable override lock requiresExecutor {

/// `_decode` is called 3 times
223:     function executeSigned(bytes calldata encodedData, address userAccount, uint16)
             external
             payable
             override
             lock
             requiresExecutor
         {

/// `IVirtualAccount` is called 7 times
223:     function executeSigned(bytes calldata encodedData, address userAccount, uint16)
             external
             payable
             override
             lock
             requiresExecutor
         {

/// `_decode` is called 3 times
312:     function executeSignedDepositSingle(bytes calldata encodedData, DepositParams calldata, address userAccount, uint16)
             external
             payable
             override
             requiresExecutor
             lock
         {

/// `IVirtualAccount` is called 7 times
312:     function executeSignedDepositSingle(bytes calldata encodedData, DepositParams calldata, address userAccount, uint16)
             external
             payable
             override
             requiresExecutor
             lock
         {

/// `_decode` is called 3 times
401:     function executeSignedDepositMultiple(
             bytes calldata encodedData,
             DepositMultipleParams calldata,
             address userAccount,
             uint16
         ) external payable override requiresExecutor lock {

/// `IVirtualAccount` is called 7 times
401:     function executeSignedDepositMultiple(
             bytes calldata encodedData,
             DepositMultipleParams calldata,
             address userAccount,
             uint16
         ) external payable override requiresExecutor lock {

```
[#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L137) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L137) [#L223](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L223) [#L223](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L223) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L312) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L312) [#L401](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L401) [#L401](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L401) 

```solidity
File: src/RootBridgeAgent.sol

/// `SettlementRedeemUnavailable` is called 2 times
299:     function redeemSettlement(uint32 _settlementNonce) external override lock {

/// `IPort` is called 3 times
299:     function redeemSettlement(uint32 _settlementNonce) external override lock {

/// `InvalidInputParams` is called 3 times
351:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId)
             public
             override
             requiresAgentExecutor
         {

/// `IPort` is called 4 times
351:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId)
             public
             override
             requiresAgentExecutor
         {

/// `AlreadyExecutedTransaction` is called 8 times
434:     function lzReceiveNonBlocking(
             address _endpoint,
             uint16 _srcChainId,
             bytes calldata _srcAddress,
             bytes calldata _payload
         ) public override requiresEndpoint(_endpoint, _srcChainId, _srcAddress) {

/// `IPort` is called 10 times
434:     function lzReceiveNonBlocking(
             address _endpoint,
             uint16 _srcChainId,
             bytes calldata _srcAddress,
             bytes calldata _payload
         ) public override requiresEndpoint(_endpoint, _srcChainId, _srcAddress) {

/// `_execute` is called 2 times
434:     function lzReceiveNonBlocking(
             address _endpoint,
             uint16 _srcChainId,
             bytes calldata _srcAddress,
             bytes calldata _payload
         ) public override requiresEndpoint(_endpoint, _srcChainId, _srcAddress) {

/// `IPort` is called 2 times
966:     function _createSettlement(
             uint32 _settlementNonce,
             address payable _refundee,
             address _recipient,
             uint16 _dstChainId,
             bytes memory _params,
             address _globalAddress,
             uint256 _amount,
             uint256 _deposit,
             bool _hasFallbackToggled
         ) internal returns (bytes memory _payload) {

/// `InvalidInputParamsLength` is called 3 times
1045:     function _createSettlementMultiple(
              uint32 _settlementNonce,
              address payable _refundee,
              address _recipient,
              uint16 _dstChainId,
              address[] memory _globalAddresses,
              uint256[] memory _amounts,
              uint256[] memory _deposits,
              bytes memory _params,
              bool _hasFallbackToggled
          ) internal returns (bytes memory _payload) {

/// `IPort` is called 2 times
1045:     function _createSettlementMultiple(
              uint32 _settlementNonce,
              address payable _refundee,
              address _recipient,
              uint16 _dstChainId,
              address[] memory _globalAddresses,
              uint256[] memory _amounts,
              uint256[] memory _deposits,
              bytes memory _params,
              bool _hasFallbackToggled
          ) internal returns (bytes memory _payload) {

/// `InvalidInputParams` is called 2 times
1131:     function _updateStateOnBridgeOut(
              address _depositor,
              address _globalAddress,
              address _localAddress,
              address _underlyingAddress,
              uint256 _amount,
              uint256 _deposit,
              uint16 _dstChainId
          ) internal {

```
[#L299](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L299) [#L299](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L299) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L351) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L351) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L434) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L434) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L434) [#L966](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L966) [#L1045](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1045) [#L1045](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1045) [#L1131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1131) 

```solidity
File: src/RootPort.sol

/// `IBridgeAgent` is called 3 times
393:     function syncBranchBridgeAgentWithRoot(
             address _newBranchBridgeAgent,
             address _rootBridgeAgent,
             uint256 _branchChainId
         ) external override requiresCoreRootRouter {

/// `ICoreRootRouter` is called 2 times
438:     function addNewChain(
             address _coreBranchBridgeAgentAddress,
             uint256 _chainId,
             string memory _wrappedGasTokenName,
             string memory _wrappedGasTokenSymbol,
             uint8 _wrappedGasTokenDecimals,
             address _newLocalBranchWrappedNativeTokenAddress,
             address _newUnderlyingBranchWrappedNativeTokenAddress
         ) external override onlyOwner {

/// `AlreadyAddedEcosystemToken` is called 3 times
483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

```
[#L393](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L393) [#L438](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L438) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) 

```solidity
File: src/VirtualAccount.sol

/// `CallFailed` is called 2 times
85:     function payableCall(PayableCall[] calldata calls) public payable returns (bytes[] memory returnData) {

```
[#L85](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L85) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

/// `ERC20` is called 3 times
60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

</details>

---

<a name="GAS-17"></a> 
### [GAS-17] Unlimited gas consumption risk due to external call recipients
When calling an external function without specifying a gas limit , the called contract may consume all the remaining gas, causing the tx to be reverted. To mitigate this, it is recommended to explicitly set a gas limit when making low level external calls.

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

103:         _rootBridgeAgentAddress.call{value: msg.value}("");

```
[#L103](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L103) 

```solidity
File: src/BranchBridgeAgent.sol

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

```
[#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) [#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) 

```solidity
File: src/MulticallRootRouter.sol

239:             IVirtualAccount(userAccount).call(calls);

328:             IVirtualAccount(userAccount).call(calls);

416:             IVirtualAccount(userAccount).call(calls);

```
[#L239](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L239) [#L328](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L328) [#L416](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L416) 

```solidity
File: src/RootBridgeAgent.sol

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

835:             callee.call{value: msg.value}("");

927:             callee.call{value: _value}("");

```
[#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L835](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L835) [#L927](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L927) 

</details>

---

<a name="GAS-18"></a> 
### [GAS-18] Use assembly to compute hashes to save gas
If the arguments to the encode call can fit into the scratch space (two words or fewer), then it's more efficient to use assembly to generate the hash (80 gas):

`keccak256(abi.encodePacked(x, y)) -> assembly {mstore(0x00, a); mstore(0x20, b); let hash := keccak256(0x00, 0x40); }`

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: src/RootPort.sol

362:         newAccount = new VirtualAccount{salt: keccak256(abi.encode(_user))}(_user, address(this));

```
[#L362](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L362) 

</details>

---

<a name="GAS-19"></a> 
### [GAS-19] Use assembly to emit events
To efficiently emit events, it's possible to utilize assembly by making use of scratch space and the free memory pointer. This approach has the advantage of potentially avoiding the costs associated with memory expansion.

However, it's important to note that in order to safely optimize this process, it is preferable to cache and restore the free memory pointer.

A good example of such practice can be seen in [Solady's](https://github.com/Vectorized/solady/blob/main/src/tokens/ERC1155.sol#L167) codebase.

<details>
<summary>
There are <b>29</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

689:             emit LogFallback(nonce);

700:         emit LogExecute(nonce);

```
[#L689](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L689) [#L700](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L700) 

```solidity
File: src/BranchPort.sol

163:         emit DebtCreated(msg.sender, _token, _amount);

184:         emit DebtRepaid(msg.sender, _token, _amount);

218:         emit DebtRepaid(_strategy, _token, amountToWithdraw);

344:         emit BridgeAgentFactoryAdded(_newBridgeAgentFactory);

351:         emit BridgeAgentFactoryToggled(_newBridgeAgentFactory);

358:         emit BridgeAgentToggled(_bridgeAgent);

371:         emit StrategyTokenAdded(_token, _minimumReservesRatio);

378:         emit StrategyTokenToggled(_token);

392:         emit PortStrategyAdded(_portStrategy, _token, _dailyManagementLimit);

399:         emit PortStrategyToggled(_portStrategy, _token);

410:         emit PortStrategyUpdated(_portStrategy, _token, _dailyManagementLimit);

423:         emit CoreBranchSet(_coreBranchRouter, _coreBranchBridgeAgent);

```
[#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L163) [#L184](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L184) [#L218](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L218) [#L344](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L344) [#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L351) [#L358](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L358) [#L371](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L371) [#L378](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L378) [#L392](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L392) [#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L399) [#L410](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L410) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L423) 

```solidity
File: src/RootBridgeAgent.sol

726:             emit LogFallback(nonce, _srcChainId);

736:         emit LogExecute(nonce, _srcChainId);

```
[#L726](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L726) [#L736](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L736) 

```solidity
File: src/RootPort.sol

255:         emit LocalTokenAdded(_underlyingAddress, _localAddress, _globalAddress, _srcChainId);

269:         emit GlobalTokenAdded(_localAddress, _globalAddress, _srcChainId);

365:         emit VirtualAccountCreated(_user, address(newAccount));

389:         emit BridgeAgentAdded(_bridgeAgent, _manager);

406:         emit BridgeAgentSynced(_newBranchBridgeAgent, _rootBridgeAgent, _branchChainId);

417:         emit BridgeAgentToggled(_bridgeAgent);

427:         emit BridgeAgentFactoryAdded(_bridgeAgentFactory);

434:         emit BridgeAgentFactoryToggled(_bridgeAgentFactory);

479:         emit NewChainAdded(_chainId);

505:         emit EcosystemTokenAdded(_ecoTokenGlobalAddress);

517:         emit CoreRootSet(_coreRootRouter, _coreRootBridgeAgent);

535:         emit CoreBranchSet(_coreBranchRouter, _coreBranchBridgeAgent, _dstChainId);

549:         emit CoreBranchSynced(_coreBranchRouter, _coreBranchBridgeAgent, _dstChainId);

```
[#L255](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L255) [#L269](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L269) [#L365](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L365) [#L389](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L389) [#L406](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L406) [#L417](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L417) [#L427](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L427) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L434) [#L479](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L479) [#L505](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L505) [#L517](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L517) [#L535](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L535) [#L549](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L549) 

</details>

---

<a name="GAS-20"></a> 
### [GAS-20] Using a double `if` statement instead of a logical AND (`&&`)
Using a double `if` statement instead of a logical AND (`&&`) can provide similar short-circuiting behavior whereas double if is slightly [more gas efficient](https://gist.github.com/DadeKuma/931ce6794a050201ec6544dbcc31316c).

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: src/RootBridgeAgent.sol

1141:         if (_amount == 0 && _deposit == 0) revert InvalidInputParams();

```
[#L1141](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1141) 

</details>

---

<a name="GAS-21"></a> 
### [GAS-21] Use a more recent version of solidity
- Use a solidity version of at least 0.8.2 to get simple compiler automatic inlining.
- Use a solidity version of at least 0.8.3 to get better struct packing and cheaper multiple storage reads.
- Use a solidity version of at least 0.8.4 to get custom errors, which are cheaper at deployment than revert()/require() strings.
- Use a solidity version of at least 0.8.10 to have external calls skip contract existence checks if the external call has a return value.

<details>
<summary>
There are <b>44</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L2) 

```solidity
File: src/ArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L3) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L2) 

```solidity
File: src/BaseBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L2) 

```solidity
File: src/BranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L2) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L2) 

```solidity
File: src/BranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L3) 

```solidity
File: src/CoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L2) 

```solidity
File: src/CoreRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L2) 

```solidity
File: src/MulticallRootRouterLibZip.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouterLibZip.sol#L2) 

```solidity
File: src/RootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L2) 

```solidity
File: src/RootBridgeAgentExecutor.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L2) 

```solidity
File: src/RootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L3) 

```solidity
File: src/VirtualAccount.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L3) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L2) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L2) 

```solidity
File: src/interfaces/IArbitrumBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IArbitrumBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IBranchBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IBranchPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L3) 

```solidity
File: src/interfaces/IBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L2) 

```solidity
File: src/interfaces/ICoreBranchRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ICoreBranchRouter.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranch.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L2) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L2) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L3) 

```solidity
File: src/interfaces/IMulticall2.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L2) 

```solidity
File: src/interfaces/IPortStrategy.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IPortStrategy.sol#L3) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L2) 

```solidity
File: src/interfaces/IRootBridgeAgentFactory.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgentFactory.sol#L2) 

```solidity
File: src/interfaces/IRootPort.sol

3: pragma solidity ^0.8.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L3) 

```solidity
File: src/interfaces/IRootRouter.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L2) 

```solidity
File: src/interfaces/IVirtualAccount.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IVirtualAccount.sol#L2) 

```solidity
File: src/token/ERC20hTokenBranch.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L2) 

```solidity
File: src/token/ERC20hTokenRoot.sol

2: pragma solidity ^0.8.0;

```
[#L2](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L2) 

</details>

---

<a name="GAS-22"></a> 
### [GAS-22] Use `unchecked` block for safe subtractions
If it can be confirmed that the subtraction operation will not overflow, using an unchecked block can save gas. For example, `require(x <= y); z = y - x;` can be optimized to `require(x <= y); unchecked { z = y - x; }`

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

/// Checked on line 440
440:             return currBalance > minReserves ? currBalance - minReserves : 0;

/// Checked on line 440
457:             return currBalance < minReserves ? minReserves - currBalance : 0;

```
[#L440](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L440) [#L457](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L457) 

```solidity
File: src/RootBridgeAgent.sol

/// Checked on line 1142
1149:         if (_amount - _deposit > 0) {

/// Checked on line 1142
1151:                 _globalAddress.safeTransferFrom(_depositor, localPortAddress, _amount - _deposit);

```
[#L1149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1149) [#L1151](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1151) 

</details>

---

<a name="GAS-23"></a> 
### [GAS-23] Using bitmap to store bool states can save gas
Using a bitmap instead of a bool array or a bool mapping to store boolean states can save gas fees. This is because the bitmap can store 256 boolean values in a single slot instead of 256 slots, which can save gas when writing bool values or when reading multiple bool values from the same slot.

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

32:     mapping(address bridgeAgent => bool isActiveBridgeAgent) public isBridgeAgent;

42:     mapping(address bridgeAgentFactory => bool isActiveBridgeAgentFactory) public isBridgeAgentFactory;

52:     mapping(address token => bool allowsStrategies) public isStrategyToken;

68:     mapping(address strategy => mapping(address token => bool isActiveStrategy)) public isPortStrategy;

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L32) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L42) [#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L52) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L68) 

```solidity
File: src/RootBridgeAgent.sol

68:     mapping(uint256 chainId => bool allowed) public isBranchBridgeAgentAllowed;

```
[#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L68) 

```solidity
File: src/RootPort.sol

54:     mapping(VirtualAccount acount => mapping(address router => bool allowed)) public isRouterApproved;

61:     mapping(uint256 chainId => bool isActive) public isChainId;

64:     mapping(address bridgeAgent => bool isActive) public isBridgeAgent;

77:     mapping(address bridgeAgentFactory => bool isActive) public isBridgeAgentFactory;

87:     mapping(address token => bool isGlobalToken) public isGlobalAddress;

```
[#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L54) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L61) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L64) [#L77](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L77) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L87) 

</details>

---

<a name="GAS-24"></a> 
### [GAS-24] Use `selfbalance()` instead of `address(this).balance`
Use assembly when getting a contract's balance of ETH.

You can use `selfbalance()` instead of `address(this).balance` when getting your contract's balance of ETH to save gas.
Additionally, you can use `balance(address)` instead of `address.balance()` when getting an external contract's balance of ETH.

*Saves 15 gas when checking internal balance, 6 for external*

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

717:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

737:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

787:         ILayerZeroEndpoint(lzEndpointAddress).send{value: address(this).balance}(

```
[#L717](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L717) [#L737](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L737) [#L787](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L787) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

92:             _recipient.safeTransferETH(address(this).balance);

126:             _recipient.safeTransferETH(address(this).balance);

```
[#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L92) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L126) 

```solidity
File: src/RootBridgeAgent.sol

695:                 address(this).balance

754:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

779:         (bool success,) = bridgeAgentExecutorAddress.call{value: address(this).balance}(_calldata);

940:         ILayerZeroEndpoint(lzEndpointAddress).send{value: address(this).balance}(

```
[#L695](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L695) [#L754](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L754) [#L779](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L779) [#L940](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L940) 

</details>

---

<a name="GAS-25"></a> 
### [GAS-25] Using bools for storage incurs overhead
Use uint256(1) and uint256(2) for true/false to avoid a Gwarmaccess (100 gas), and to avoid Gsset (20000 gas) when changing from ‘false’ to ‘true’, after having been ‘true’ in the past. See [source](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/58f635312aa21f947cae5f8578638a85aa2519f5/contracts/security/ReentrancyGuard.sol#L23-L27).

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: src/BranchPort.sol

32:     mapping(address bridgeAgent => bool isActiveBridgeAgent) public isBridgeAgent;

42:     mapping(address bridgeAgentFactory => bool isActiveBridgeAgentFactory) public isBridgeAgentFactory;

52:     mapping(address token => bool allowsStrategies) public isStrategyToken;

68:     mapping(address strategy => mapping(address token => bool isActiveStrategy)) public isPortStrategy;

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L32) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L42) [#L52](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L52) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L68) 

```solidity
File: src/CoreRootRouter.sol

44:     bool internal _setup;

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L44) 

```solidity
File: src/RootBridgeAgent.sol

68:     mapping(uint256 chainId => bool allowed) public isBranchBridgeAgentAllowed;

```
[#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L68) 

```solidity
File: src/RootPort.sol

24:     bool internal _setup;

27:     bool internal _setupCore;

54:     mapping(VirtualAccount acount => mapping(address router => bool allowed)) public isRouterApproved;

61:     mapping(uint256 chainId => bool isActive) public isChainId;

64:     mapping(address bridgeAgent => bool isActive) public isBridgeAgent;

77:     mapping(address bridgeAgentFactory => bool isActive) public isBridgeAgentFactory;

87:     mapping(address token => bool isGlobalToken) public isGlobalAddress;

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L24) [#L27](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L27) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L54) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L61) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L64) [#L77](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L77) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L87) 

</details>

---

<a name="GAS-26"></a> 
### [GAS-26] Cache array length outside of loop
If not cached, the solidity compiler will always read the length of the array during each iteration. That is, if it is a storage array, this is an extra sload operation (100 additional extra gas for each iteration except for the first) and if it is a memory array, this is an extra mload operation (3 additional gas for each iteration except for the first).

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

192:         for (uint256 i = 0; i < _hTokens.length;) {

```
[#L192](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L192) 

```solidity
File: src/BranchBridgeAgent.sol

447:         for (uint256 i = 0; i < deposit.tokens.length;) {

```
[#L447](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L447) 

```solidity
File: src/MulticallRootRouter.sol

278:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

367:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

455:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

557:         for (uint256 i = 0; i < outputTokens.length;) {

```
[#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L278) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L367) [#L455](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L455) [#L557](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L557) 

```solidity
File: src/RootBridgeAgent.sol

318:         for (uint256 i = 0; i < settlement.hTokens.length;) {

1070:         for (uint256 i = 0; i < hTokens.length;) {

```
[#L318](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L318) [#L1070](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1070) 

</details>

---

<a name="GAS-27"></a> 
### [GAS-27] State variables should be cached in stack variables rather than re-reading them from storage
The instances below point to the second+ access of a state variable within a function. Caching of a state variable replaces each Gwarmaccess (100 gas) with a much cheaper stack read. Other less obvious fixes/optimizations include having local memory caches of state variable structs, or having local caches of state variable contracts/addresses.

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

/// More than 1 read for `localBridgeAgentAddress`, line 62 and 61
62:         localBridgeAgentAddress = _localBridgeAgentAddress;

```
[#L62](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L62) 

```solidity
File: src/BranchPort.sol

/// More than 1 read for `coreBranchRouterAddress`, line 129 and 123
129:         coreBranchRouterAddress = _coreBranchRouter;

/// More than 1 read for `coreBranchRouterAddress`, line 129 and 123
129:         coreBranchRouterAddress = _coreBranchRouter;

/// More than 1 read for `getStrategyTokenDebt`, line 190 and 146
190:         uint256 strategyTokenDebt = getStrategyTokenDebt[_token];

/// More than 1 read for `coreBranchRouterAddress`, line 334 and 332
334:         coreBranchRouterAddress = _newCoreRouter;

```
[#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L129) [#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L129) [#L190](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L190) [#L334](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L334) 

```solidity
File: src/MulticallRootRouter.sol

/// More than 1 read for `bridgeAgentAddress`, line 112 and 110
112:         bridgeAgentAddress = payable(_bridgeAgentAddress);

/// More than 1 read for `bridgeAgentAddress`, line 112 and 110
112:         bridgeAgentAddress = payable(_bridgeAgentAddress);

```
[#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L112) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L112) 

```solidity
File: src/RootPort.sol

/// More than 1 read for `localBranchPortAddress`, line 160 and 154
160:         localBranchPortAddress = _localBranchPortAddress;

```
[#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L160) 

</details>

---

<a name="GAS-28"></a> 
### [GAS-28] Use `calldata` instead of `memory` for function arguments that do not get mutated
Mark data types as `calldata` instead of `memory` where possible. This makes it so that the data is not automatically loaded into memory. If the data passed into the function does not need to be changed (like updating values in an array), it can be passed in as `calldata`. The one exception to this is if the argument must later be passed into another function that takes an argument that specifies `memory` storage.

<details>
<summary>
There are <b>70</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

128:     function executeSettlement(bytes calldata, SettlementParams memory)

139:     function executeSettlementMultiple(bytes calldata, SettlementMultipleParams memory)

```
[#L128](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L128) [#L139](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L139) 

```solidity
File: src/BranchBridgeAgent.sol

212:         DepositInput memory _dParams,

234:         DepositMultipleInput memory _dParams,

279:         DepositInput memory _dParams,

309:         DepositMultipleInput memory _dParams,

```
[#L212](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L212) [#L234](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L234) [#L279](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L279) [#L309](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L309) 

```solidity
File: src/BranchPort.sol

248:         address[] memory _localAddresses,

249:         address[] memory _underlyingAddresses,

250:         uint256[] memory _amounts,

251:         uint256[] memory _deposits

290:         address[] memory _localAddresses,

291:         address[] memory _underlyingAddresses,

292:         uint256[] memory _amounts,

293:         uint256[] memory _deposits

```
[#L248](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L248) [#L249](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L249) [#L250](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L250) [#L251](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L251) [#L290](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L290) [#L291](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L291) [#L292](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L292) [#L293](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L293) 

```solidity
File: src/CoreRootRouter.sol

350:     function executeDepositSingle(bytes memory, DepositParams memory, uint16)

350:     function executeDepositSingle(bytes memory, DepositParams memory, uint16)

360:     function executeDepositMultiple(bytes calldata, DepositMultipleParams memory, uint16)

370:     function executeSigned(bytes memory, address, uint16) external payable override requiresExecutor {

375:     function executeSignedDepositSingle(bytes memory, DepositParams memory, address, uint16)

375:     function executeSignedDepositSingle(bytes memory, DepositParams memory, address, uint16)

385:     function executeSignedDepositMultiple(bytes memory, DepositMultipleParams memory, address, uint16)

385:     function executeSignedDepositMultiple(bytes memory, DepositMultipleParams memory, address, uint16)

```
[#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L350) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L350) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L360) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L370) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L375) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L375) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L385) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L385) 

```solidity
File: src/MulticallRootRouter.sol

123:     function executeResponse(bytes memory, uint16) external payable override {

```
[#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L123) 

```solidity
File: src/RootBridgeAgent.sol

351:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId)

```
[#L351](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L351) 

```solidity
File: src/RootPort.sol

441:         string memory _wrappedGasTokenName,

442:         string memory _wrappedGasTokenSymbol,

```
[#L441](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L441) [#L442](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L442) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

42:     constructor(uint16 _localChainId, address _localPortAddress, string memory _chainName, string memory _chainSymbol) {

42:     constructor(uint16 _localChainId, address _localPortAddress, string memory _chainName, string memory _chainSymbol) {

96:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

96:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L42) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L42) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L96) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L96) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

76:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

76:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

```
[#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L76) [#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L76) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

166:         DepositInput memory depositParams,

182:         DepositMultipleInput memory depositParams,

211:         DepositInput memory depositParams,

230:         DepositMultipleInput memory depositParams,

```
[#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L166) [#L182](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L182) [#L211](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L211) [#L230](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L230) 

```solidity
File: src/interfaces/IBranchPort.sol

105:         address[] memory _localAddresses,

106:         address[] memory _underlyingAddresses,

107:         uint256[] memory _amounts,

108:         uint256[] memory _deposits

137:         address[] memory _localAddresses,

138:         address[] memory _underlyingAddresses,

139:         uint256[] memory _amounts,

140:         uint256[] memory _deposits

```
[#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L105) [#L106](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L106) [#L107](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L107) [#L108](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L108) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L137) [#L138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L138) [#L139](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L139) [#L140](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchPort.sol#L140) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L24) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L24) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L24) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L24) 

```solidity
File: src/interfaces/IMulticall2.sol

20:     function aggregate(Call[] memory calls) external returns (uint256 blockNumber, bytes[] memory returnData);

```
[#L20](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IMulticall2.sol#L20) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

172:         bytes memory _params,

271:     function bridgeIn(address _recipient, DepositParams memory _dParams, uint256 _srcChainId) external;

```
[#L172](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L172) [#L271](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L271) 

```solidity
File: src/interfaces/IRootPort.sol

322:         string memory _wrappedGasTokenName,

323:         string memory _wrappedGasTokenSymbol,

```
[#L322](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L322) [#L323](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L323) 

```solidity
File: src/interfaces/IRootRouter.sol

25:     function executeResponse(bytes memory params, uint16 srcChainId) external payable;

33:     function execute(bytes memory params, uint16 srcChainId) external payable;

42:     function executeDepositSingle(bytes memory params, DepositParams memory dParams, uint16 srcChainId)

42:     function executeDepositSingle(bytes memory params, DepositParams memory dParams, uint16 srcChainId)

53:     function executeDepositMultiple(bytes memory params, DepositMultipleParams memory dParams, uint16 srcChainId)

53:     function executeDepositMultiple(bytes memory params, DepositMultipleParams memory dParams, uint16 srcChainId)

63:     function executeSigned(bytes memory params, address userAccount, uint16 srcChainId) external payable;

73:         bytes memory params,

74:         DepositParams memory dParams,

87:         bytes memory params,

88:         DepositMultipleParams memory dParams,

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L25) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L33) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L42) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L42) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L53) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L53) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L63) [#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L73) [#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L74) [#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L87) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L88) 

```solidity
File: src/token/ERC20hTokenBranch.sol

14:         string memory chainName,

15:         string memory chainSymbol,

16:         string memory _name,

17:         string memory _symbol,

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L14) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L15) [#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L16) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L17) 

```solidity
File: src/token/ERC20hTokenRoot.sol

35:         string memory _name,

36:         string memory _symbol,

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L35) [#L36](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L36) 

</details>

---

<a name="GAS-29"></a> 
### [GAS-29] Use Custom Errors
[Source](https://blog.soliditylang.org/2021/04/21/custom-errors/)
Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

<details>
<summary>
There are <b>44</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L39) 

```solidity
File: src/BaseBranchRouter.sol

61:         require(_localBridgeAgentAddress != address(0), "Bridge Agent address cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L61) 

```solidity
File: src/BranchBridgeAgent.sol

125:         require(_rootBridgeAgentAddress != address(0), "Root Bridge Agent Address cannot be the zero address.");

130:         require(_localRouterAddress != address(0), "Local Router Address cannot be the zero address.");

131:         require(_localPortAddress != address(0), "Local Port Address cannot be the zero address.");

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L125) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L131) 

```solidity
File: src/BranchPort.sol

109:         require(_owner != address(0), "Owner is zero address");

123:         require(coreBranchRouterAddress == address(0), "Contract already initialized");

124:         require(!isBridgeAgentFactory[_bridgeAgentFactory], "Contract already initialized");

126:         require(_coreBranchRouter != address(0), "CoreBranchRouter is zero address");

127:         require(_bridgeAgentFactory != address(0), "BridgeAgentFactory is zero address");

136:         revert("Cannot renounce ownership");

181:         require(ERC20(_token).balanceOf(address(this)) - currBalance == _amount, "Port Strategy Withdraw Failed");

332:         require(coreBranchRouterAddress != address(0), "CoreRouter address is zero");

333:         require(_newCoreRouter != address(0), "New CoreRouter address is zero");

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L109) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L123) [#L124](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L124) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L126) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L127) [#L136](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L136) [#L181](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L181) [#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L332) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L333) 

```solidity
File: src/CoreRootRouter.sol

84:         require(_setup, "Contract is already initialized");

278:         require(msg.sender == rootPortAddress, "Only root port can call");

```
[#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L84) [#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L278) 

```solidity
File: src/MulticallRootRouter.sol

93:         require(_localPortAddress != address(0), "Local Port Address cannot be 0");

94:         require(_multicallAddress != address(0), "Multicall Address cannot be 0");

110:         require(_bridgeAgentAddress != address(0), "Bridge Agent Address cannot be 0");

```
[#L93](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L93) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L94) [#L110](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L110) 

```solidity
File: src/RootBridgeAgent.sol

111:         require(_lzEndpointAddress != address(0), "Layerzero Enpoint Address cannot be zero address");

112:         require(_localPortAddress != address(0), "Port Address cannot be zero address");

113:         require(_localRouterAddress != address(0), "Router Address cannot be zero address");

```
[#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L111) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L112) [#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L113) 

```solidity
File: src/RootPort.sol

130:         require(_bridgeAgentFactory != address(0), "Bridge Agent Factory cannot be 0 address.");

131:         require(_coreRootRouter != address(0), "Core Root Router cannot be 0 address.");

132:         require(_setup, "Setup ended.");

152:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0 address.");

153:         require(_coreLocalBranchBridgeAgent != address(0), "Core Local Branch Bridge Agent cannot be 0 address.");

154:         require(_localBranchPortAddress != address(0), "Local Branch Port Address cannot be 0 address.");

155:         require(isBridgeAgent[_coreRootBridgeAgent], "Core Bridge Agent doesn't exist.");

156:         require(_setupCore, "Core Setup ended.");

167:         revert("Cannot renounce ownership");

```
[#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L131) [#L132](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L132) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L152) [#L153](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L153) [#L154](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L154) [#L155](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L155) [#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L156) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L167) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

57:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent Address cannot be 0");

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L57) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

61:         require(_rootBridgeAgentFactoryAddress != address(0), "Root Bridge Agent Factory Address cannot be 0");

66:         require(_localCoreBranchRouterAddress != address(0), "Core Branch Router Address cannot be 0");

67:         require(_localPortAddress != address(0), "Port Address cannot be 0");

68:         require(_owner != address(0), "Owner cannot be 0");

88:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L61) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L66) [#L67](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L67) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L68) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L88) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

43:         require(_localPortAddress != address(0), "Port address cannot be 0");

61:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L43) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L61) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

35:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

50:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L35) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L50) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

32:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L32) 

```solidity
File: src/token/ERC20hTokenRoot.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

40:         require(_factoryAddress != address(0), "Factory Address cannot be 0");

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L39) [#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L40) 

</details>

---

<a name="GAS-30"></a> 
### [GAS-30] Don't initialize variables with default value

<details>
<summary>
There are <b>17</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

192:         for (uint256 i = 0; i < _hTokens.length;) {

```
[#L192](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L192) 

```solidity
File: src/BranchBridgeAgent.sol

447:         for (uint256 i = 0; i < deposit.tokens.length;) {

513:         for (uint256 i = 0; i < numOfAssets;) {

```
[#L447](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L447) [#L513](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L513) 

```solidity
File: src/BranchPort.sol

257:         for (uint256 i = 0; i < length;) {

305:         for (uint256 i = 0; i < length;) {

```
[#L257](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L257) [#L305](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L305) 

```solidity
File: src/MulticallRootRouter.sol

278:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

367:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

455:             for (uint256 i = 0; i < outputParams.outputTokens.length;) {

557:         for (uint256 i = 0; i < outputTokens.length;) {

```
[#L278](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L278) [#L367](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L367) [#L455](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L455) [#L557](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L557) 

```solidity
File: src/RootBridgeAgent.sol

318:         for (uint256 i = 0; i < settlement.hTokens.length;) {

399:         for (uint256 i = 0; i < length;) {

1070:         for (uint256 i = 0; i < hTokens.length;) {

```
[#L318](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L318) [#L399](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L399) [#L1070](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1070) 

```solidity
File: src/RootBridgeAgentExecutor.sol

281:         for (uint256 i = 0; i < uint256(uint8(numOfAssets));) {

```
[#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L281) 

```solidity
File: src/VirtualAccount.sol

70:         for (uint256 i = 0; i < length;) {

90:         for (uint256 i = 0; i < length;) {

```
[#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L70) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L90) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

23:     uint8 internal constant STATUS_SUCCESS = 0;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) 

</details>

---

<a name="GAS-31"></a> 
### [GAS-31] Usage of `int`s/`uint`s smaller than 32 bytes incurs overhead
Using `int`s/`uint`s smaller than 32 bytes may cost more gas. This is because the EVM operates on 32 bytes at a time, so if an element is smaller than 32 bytes, the EVM must perform more operations to reduce the size of the element from 32 bytes to the desired size.

<details>
<summary>
There are <b>281</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchBridgeAgent.sol

11:     function deploy(uint16 _localChainId, address _daoAddress, address _localRouterAddress, address _localPortAddress)

44:         uint16 _localChainId,

89:     function retrySettlement(uint32, bytes calldata, GasParams[2] calldata, bool) external payable override lock {}

112:     function _performFallbackCall(address payable, uint32 _settlementNonce) internal override {

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L11) [#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L44) [#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L89) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchBridgeAgent.sol#L112) 

```solidity
File: src/ArbitrumBranchPort.sol

22:     uint16 public immutable localChainId;

38:     constructor(uint16 _localChainId, address _rootPortAddress, address _owner) BranchPort(_owner) {

```
[#L22](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L22) [#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L38) 

```solidity
File: src/BaseBranchRouter.sol

74:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

```
[#L74](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L74) 

```solidity
File: src/BranchBridgeAgent.sol

25:         uint16 _rootChainId,

26:         uint16 _localChainId,

53:     uint16 public immutable rootChainId;

56:     uint16 public immutable localChainId;

84:     uint32 public depositNonce;

118:         uint16 _rootChainId,

119:         uint16 _localChainId,

156:     function getDepositEntry(uint32 _depositNonce) external view override returns (Deposit memory) {

171:             abi.encodePacked(uint16(2), _gasLimit, _remoteBranchExecutionGas, rootBridgeAgentAddress)

216:         uint32 _depositNonce = depositNonce;

238:         uint32 _depositNonce = depositNonce;

243:             uint8(_dParams.hTokens.length),

284:         uint32 _depositNonce = depositNonce;

314:         uint32 _depositNonce = depositNonce;

320:             uint8(_dParams.hTokens.length),

345:         uint32 _depositNonce,

359:         if (uint8(deposit.hTokens.length) == 1) {

383:         } else if (uint8(deposit.hTokens.length) > 1) {

389:                     uint8(deposit.hTokens.length),

400:                     uint8(deposit.hTokens.length),

422:     function retrieveDeposit(uint32 _depositNonce, GasParams calldata _gParams) external payable override lock {

434:     function redeemDeposit(uint32 _depositNonce) external override lock {

465:         uint32 _settlementNonce,

501:         uint8 numOfAssets = uint8(bytes1(_sParams[0]));

501:         uint8 numOfAssets = uint8(bytes1(_sParams[0]));

504:         uint32 nonce = uint32(bytes4(_sParams[PARAMS_START:PARAMS_TKN_START]));

504:         uint32 nonce = uint32(bytes4(_sParams[PARAMS_START:PARAMS_TKN_START]));

519:                 uint160(

532:                 uint160(

578:     function lzReceive(uint16, bytes calldata _srcAddress, uint64, bytes calldata _payload) public override {

578:     function lzReceive(uint16, bytes calldata _srcAddress, uint64, bytes calldata _payload) public override {

596:         uint32 nonce;

601:             nonce = uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED]));

618:             address payable recipient = payable(address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED]))));

621:             nonce = uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED]));

640:             address payable recipient = payable(address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED]))));

643:             nonce = uint32(bytes4(_payload[22:26]));

665:             address payable recipient = payable(address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED]))));

668:             nonce = uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED]));

683:             nonce = uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START]));

730:     function _execute(bool _hasFallbackToggled, uint32 _settlementNonce, address _refundee, bytes memory _calldata)

776:             abi.encodePacked(uint16(2), _gParams.gasLimit, _gParams.remoteBranchExecutionGas, rootBridgeAgentAddress)

785:     function _performFallbackCall(address payable _refundee, uint32 _settlementNonce) internal virtual {

813:         uint32 _depositNonce,

861:         uint32 _depositNonce,

943:         if (rootBridgeAgentAddress != address(uint160(bytes20(_srcAddress[20:])))) revert LayerZeroUnauthorizedCaller();

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L25) [#L26](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L26) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L53) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L56) [#L84](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L84) [#L118](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L118) [#L119](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L119) [#L156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L156) [#L171](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L171) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L216) [#L238](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L238) [#L243](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L243) [#L284](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L284) [#L314](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L314) [#L320](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L320) [#L345](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L345) [#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L359) [#L383](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L383) [#L389](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L389) [#L400](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L400) [#L422](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L422) [#L434](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L434) [#L465](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L465) [#L501](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L501) [#L501](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L501) [#L504](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L504) [#L504](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L504) [#L519](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L519) [#L532](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L532) [#L578](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L578) [#L578](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L578) [#L596](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L596) [#L601](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L601) [#L618](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L618) [#L621](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L621) [#L640](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L640) [#L643](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L643) [#L665](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L665) [#L668](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L668) [#L683](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L683) [#L730](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L730) [#L776](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L776) [#L785](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L785) [#L813](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L813) [#L861](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L861) [#L943](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L943) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

73:             settlementNonce: uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED])),

75:             hToken: address(uint160(bytes20(_payload[PARAMS_TKN_START_SIGNED:45]))),

76:             token: address(uint160(bytes20(_payload[45:65]))),

110:         uint256 assetsOffset = uint8(bytes1(_payload[PARAMS_START_SIGNED])) * PARAMS_TKN_SET_SIZE_MULTIPLE;

```
[#L73](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L73) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L75) [#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L76) [#L110](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L110) 

```solidity
File: src/CoreBranchRouter.sol

64:         uint8 decimals = ERC20(_underlyingAddress).decimals();

93:                 uint8 decimals,

96:             ) = abi.decode(_params[1:], (address, string, string, uint8, address, GasParams));

170:         uint8 _decimals,

```
[#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L64) [#L93](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L93) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L96) [#L170](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L170) 

```solidity
File: src/CoreRootRouter.sol

108:         uint16 _dstChainId,

160:         uint16 _dstChainId,

189:         uint16 _dstChainId,

216:         uint16 _dstChainId,

247:         uint16 _dstChainId,

274:         uint16 _dstChainId,

297:     function executeResponse(bytes calldata _encodedData, uint16 _srcChainId)

308:             (address underlyingAddress, address localAddress, string memory name, string memory symbol, uint8 decimals)

309:             = abi.decode(_encodedData[1:], (address, address, string, string, uint8));

332:     function execute(bytes calldata _encodedData, uint16) external payable override requiresExecutor {

338:             (address refundee, address globalAddress, uint16 dstChainId, GasParams[2] memory gasParams) =

339:                 abi.decode(_encodedData[1:], (address, address, uint16, GasParams[2]));

350:     function executeDepositSingle(bytes memory, DepositParams memory, uint16)

360:     function executeDepositMultiple(bytes calldata, DepositMultipleParams memory, uint16)

370:     function executeSigned(bytes memory, address, uint16) external payable override requiresExecutor {

375:     function executeSignedDepositSingle(bytes memory, DepositParams memory, address, uint16)

385:     function executeSignedDepositMultiple(bytes memory, DepositMultipleParams memory, address, uint16)

409:         uint16 _dstChainId,

457:         uint8 _decimals,

458:         uint16 _srcChainId

481:     function _setLocalToken(address _globalAddress, address _localAddress, uint16 _dstChainId) internal {

```
[#L108](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L108) [#L160](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L160) [#L189](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L189) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L216) [#L247](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L247) [#L274](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L274) [#L297](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L297) [#L308](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L308) [#L309](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L309) [#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L332) [#L338](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L338) [#L339](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L339) [#L350](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L350) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L360) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L370) [#L375](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L375) [#L385](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L385) [#L409](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L409) [#L457](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L457) [#L458](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L458) [#L481](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L481) 

```solidity
File: src/MulticallRootRouter.sol

123:     function executeResponse(bytes memory, uint16) external payable override {

137:     function execute(bytes calldata encodedData, uint16) external payable override lock requiresExecutor {

155:                 uint16 dstChainId,

157:             ) = abi.decode(_decode(encodedData[1:]), (IMulticall.Call[], OutputParams, uint16, GasParams));

179:                 uint16 dstChainId,

181:             ) = abi.decode(_decode(encodedData[1:]), (IMulticall.Call[], OutputMultipleParams, uint16, GasParams));

203:     function executeDepositSingle(bytes calldata, DepositParams calldata, uint16) external payable override {

209:     function executeDepositMultiple(bytes calldata, DepositMultipleParams calldata, uint16) external payable {

223:     function executeSigned(bytes calldata encodedData, address userAccount, uint16)

244:             (Call[] memory calls, OutputParams memory outputParams, uint16 dstChainId, GasParams memory gasParams) =

245:                 abi.decode(_decode(encodedData[1:]), (Call[], OutputParams, uint16, GasParams));

270:                 uint16 dstChainId,

272:             ) = abi.decode(_decode(encodedData[1:]), (Call[], OutputMultipleParams, uint16, GasParams));

312:     function executeSignedDepositSingle(bytes calldata encodedData, DepositParams calldata, address userAccount, uint16)

333:             (Call[] memory calls, OutputParams memory outputParams, uint16 dstChainId, GasParams memory gasParams) =

334:                 abi.decode(_decode(encodedData[1:]), (Call[], OutputParams, uint16, GasParams));

359:                 uint16 dstChainId,

361:             ) = abi.decode(_decode(encodedData[1:]), (Call[], OutputMultipleParams, uint16, GasParams));

405:         uint16

421:             (Call[] memory calls, OutputParams memory outputParams, uint16 dstChainId, GasParams memory gasParams) =

422:                 abi.decode(_decode(encodedData[1:]), (Call[], OutputParams, uint16, GasParams));

447:                 uint16 dstChainId,

449:             ) = abi.decode(_decode(encodedData[1:]), (Call[], OutputMultipleParams, uint16, GasParams));

514:         uint16 dstChainId,

550:         uint16 dstChainId,

```
[#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L123) [#L137](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L137) [#L155](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L155) [#L157](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L157) [#L179](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L179) [#L181](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L181) [#L203](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L203) [#L209](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L209) [#L223](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L223) [#L244](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L244) [#L245](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L245) [#L270](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L270) [#L272](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L272) [#L312](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L312) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L333) [#L334](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L334) [#L359](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L359) [#L361](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L361) [#L405](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L405) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L421) [#L422](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L422) [#L447](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L447) [#L449](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L449) [#L514](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L514) [#L550](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L550) 

```solidity
File: src/RootBridgeAgent.sol

40:     uint16 public immutable localChainId;

75:     uint32 public settlementNonce;

106:         uint16 _localChainId,

135:     function getSettlementEntry(uint32 _settlementNonce) external view override returns (Settlement memory) {

144:         uint16 _dstChainId

151:             abi.encodePacked(uint16(2), _gasLimit, _remoteBranchExecutionGas, getBranchBridgeAgent[_dstChainId])

163:         uint16 _dstChainId,

178:         uint16 _dstChainId,

205:         uint16 _dstChainId,

234:         uint32 _settlementNonce,

274:     function retrieveSettlement(uint32 _settlementNonce, GasParams calldata _gParams) external payable lock {

299:     function redeemSettlement(uint32 _settlementNonce) external override lock {

423:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64, bytes calldata _payload) public {

423:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64, bytes calldata _payload) public {

436:         uint16 _srcChainId,

441:         uint32 nonce;

446:             nonce = uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START]));

454:             uint16 srcChainId = _srcChainId;

469:             nonce = uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START]));

477:             uint16 srcChainId = _srcChainId;

492:             nonce = uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START]));

500:             uint16 srcChainId = _srcChainId;

515:             nonce = uint32(bytes4(_payload[2:6]));

523:             uint16 srcChainId = _srcChainId;

541:             nonce = uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED]));

550:                 address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED])))

557:             uint16 srcChainId = _srcChainId;

579:             nonce = uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED]));

588:                 address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED])))

595:             uint16 srcChainId = _srcChainId;

602:                 address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED]))),

619:             nonce = uint32(bytes4(_payload[PARAMS_START_SIGNED + PARAMS_START:PARAMS_START_SIGNED + PARAMS_TKN_START]));

628:                 address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED])))

635:             uint16 srcChainId = _srcChainId;

642:                 address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED]))),

664:             (nonce, owner, params, gParams) = abi.decode(_payload[PARAMS_START:], (uint32, address, bytes, GasParams));

701:             nonce = uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED]));

713:                     payable(address(uint160(bytes20(_payload[PARAMS_START:PARAMS_START_SIGNED])))), nonce, _srcChainId

720:             nonce = uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START]));

749:     function _execute(uint256 _depositNonce, bytes memory _calldata, uint16 _srcChainId) private {

770:         uint32 _depositNonce,

773:         uint16 _srcChainId

809:         uint16 _dstChainId,

829:                 abi.encodePacked(uint16(2), _gParams.gasLimit, _gParams.remoteBranchExecutionGas, callee)

863:         uint32 _settlementNonce,

866:         uint16 _dstChainId,

896:                 uint8(_hTokens.length),

921:                 abi.encodePacked(uint16(2), _gParams.gasLimit, _gParams.remoteBranchExecutionGas, callee)

938:     function _performFallbackCall(address payable _refundee, uint32 _depositNonce, uint16 _dstChainId) internal {

938:     function _performFallbackCall(address payable _refundee, uint32 _depositNonce, uint16 _dstChainId) internal {

967:         uint32 _settlementNonce,

970:         uint16 _dstChainId,

1004:         uint32 cachedSettlementNonce = _settlementNonce;

1046:         uint32 _settlementNonce,

1049:         uint16 _dstChainId,

1076:             uint16 destChainId = _dstChainId;

1092:             uint8(hTokens.length),

1138:         uint16 _dstChainId

1204:     modifier requiresEndpoint(address _endpoint, uint16 _srcChain, bytes calldata _srcAddress) virtual {

1212:             if (getBranchBridgeAgent[_srcChain] != address(uint160(bytes20(_srcAddress[PARAMS_ADDRESS_SIZE:])))) {

```
[#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L40) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L75) [#L106](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L106) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L135) [#L144](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L144) [#L151](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L151) [#L163](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L163) [#L178](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L178) [#L205](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L205) [#L234](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L234) [#L274](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L274) [#L299](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L299) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L423) [#L423](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L423) [#L436](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L436) [#L441](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L441) [#L446](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L446) [#L454](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L454) [#L469](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L469) [#L477](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L477) [#L492](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L492) [#L500](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L500) [#L515](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L515) [#L523](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L523) [#L541](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L541) [#L550](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L550) [#L557](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L557) [#L579](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L579) [#L588](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L588) [#L595](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L595) [#L602](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L602) [#L619](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L619) [#L628](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L628) [#L635](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L635) [#L642](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L642) [#L664](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L664) [#L701](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L701) [#L713](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L713) [#L720](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L720) [#L749](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L749) [#L770](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L770) [#L773](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L773) [#L809](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L809) [#L829](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L829) [#L863](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L863) [#L866](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L866) [#L896](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L896) [#L921](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L921) [#L938](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L938) [#L938](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L938) [#L967](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L967) [#L970](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L970) [#L1004](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1004) [#L1046](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1046) [#L1049](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1049) [#L1076](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1076) [#L1092](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1092) [#L1138](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1138) [#L1204](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1204) [#L1212](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1212) 

```solidity
File: src/RootBridgeAgentExecutor.sol

50:     function executeSystemRequest(address _router, bytes calldata _payload, uint16 _srcChainId)

66:     function executeNoDeposit(address _router, bytes calldata _payload, uint16 _srcChainId)

82:     function executeWithDeposit(address _router, bytes calldata _payload, uint16 _srcChainId)

89:             depositNonce: uint32(bytes4(_payload[PARAMS_START:PARAMS_TKN_START])),

90:             hToken: address(uint160(bytes20(_payload[PARAMS_TKN_START:PARAMS_TKN_START_SIGNED]))),

91:             token: address(uint160(bytes20(_payload[PARAMS_TKN_START_SIGNED:45]))),

115:     function executeWithDepositMultiple(address _router, bytes calldata _payload, uint16 _srcChainId)

125:                     PARAMS_END_OFFSET + uint256(uint8(bytes1(_payload[PARAMS_START]))) * PARAMS_TKN_SET_SIZE_MULTIPLE

130:         uint256 numOfAssets = uint8(bytes1(_payload[PARAMS_START]));

150:     function executeSignedNoDeposit(address _account, address _router, bytes calldata _payload, uint16 _srcChainId)

167:     function executeSignedWithDeposit(address _account, address _router, bytes calldata _payload, uint16 _srcChainId)

174:             depositNonce: uint32(bytes4(_payload[PARAMS_START_SIGNED:PARAMS_TKN_START_SIGNED])),

175:             hToken: address(uint160(bytes20(_payload[PARAMS_TKN_START_SIGNED:45]))),

176:             token: address(uint160(bytes20(_payload[45:65]))),

205:         uint16 _srcChainId

213:                         + uint256(uint8(bytes1(_payload[PARAMS_START_SIGNED]))) * PARAMS_TKN_SET_SIZE_MULTIPLE

222:                     + uint256(uint8(bytes1(_payload[PARAMS_START_SIGNED]))) * PARAMS_TKN_SET_SIZE_MULTIPLE

228:                         + uint256(uint8(bytes1(_payload[PARAMS_START_SIGNED]))) * PARAMS_TKN_SET_SIZE_MULTIPLE:

243:     function _bridgeIn(address _recipient, DepositParams memory _dParams, uint16 _srcChainId) internal {

268:     function _bridgeInMultiple(address _recipient, bytes calldata _dParams, uint16 _srcChainId)

273:         uint8 numOfAssets = uint8(bytes1(_dParams[0]));

273:         uint8 numOfAssets = uint8(bytes1(_dParams[0]));

274:         uint32 nonce = uint32(bytes4(_dParams[PARAMS_START:5]));

274:         uint32 nonce = uint32(bytes4(_dParams[PARAMS_START:5]));

281:         for (uint256 i = 0; i < uint256(uint8(numOfAssets));) {

287:                 uint160(

300:                 uint160(

```
[#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L50) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L66) [#L82](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L82) [#L89](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L89) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L90) [#L91](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L91) [#L115](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L115) [#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L125) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L130) [#L150](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L150) [#L167](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L167) [#L174](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L174) [#L175](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L175) [#L176](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L176) [#L205](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L205) [#L213](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L213) [#L222](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L222) [#L228](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L228) [#L243](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L243) [#L268](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L268) [#L273](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L273) [#L273](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L273) [#L274](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L274) [#L274](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L274) [#L281](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L281) [#L287](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L287) [#L300](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L300) 

```solidity
File: src/RootPort.sol

443:         uint8 _wrappedGasTokenDecimals,

525:         uint16 _dstChainId,

539:     function syncNewCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent, uint16 _dstChainId)

```
[#L443](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L443) [#L525](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L525) [#L539](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L539) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

31:         uint16 _rootChainId,

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L31) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

21:     uint16 public immutable localChainId;

24:     uint16 public immutable rootChainId;

53:         uint16 _localChainId,

54:         uint16 _rootChainId,

```
[#L21](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L21) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L24) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L53) [#L54](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L54) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

42:     constructor(uint16 _localChainId, address _localPortAddress, string memory _chainName, string memory _chainSymbol) {

96:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L42) [#L96](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L96) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

14:     uint16 public immutable localChainId;

34:     constructor(uint16 _localChainId, address _rootPortAddress) {

76:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L14) [#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L34) [#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L76) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

13:     uint16 public immutable rootChainId;

31:     constructor(uint16 _rootChainId, address _lzEndpointAddress, address _rootPortAddress) {

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L13) [#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L31) 

```solidity
File: src/interfaces/BridgeAgentConstants.sol

13:     uint8 internal constant STATUS_READY = 0;

15:     uint8 internal constant STATUS_DONE = 1;

17:     uint8 internal constant STATUS_RETRIEVE = 2;

21:     uint8 internal constant STATUS_FAILED = 1;

23:     uint8 internal constant STATUS_SUCCESS = 0;

```
[#L13](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L13) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L15) [#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L17) [#L21](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L21) [#L23](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentConstants.sol#L23) 

```solidity
File: src/interfaces/BridgeAgentStructs.sol

14:     uint8 status;

40:     uint8 numberOfAssets; //Number of assets to deposit.

41:     uint32 depositNonce; //Deposit nonce.

50:     uint32 depositNonce; //Deposit nonce.

58:     uint16 dstChainId; //Destination chain for interaction.

59:     uint80 status; //Status of the settlement

81:     uint32 settlementNonce; // Settlement nonce.

90:     uint8 numberOfAssets; // Number of assets to deposit.

92:     uint32 settlementNonce; // Settlement nonce.

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L14) [#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L40) [#L41](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L41) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L50) [#L58](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L58) [#L59](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L59) [#L81](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L81) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L90) [#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/BridgeAgentStructs.sol#L92) 

```solidity
File: src/interfaces/IBranchBridgeAgent.sol

109:     function getDepositEntry(uint32 depositNonce) external view returns (Deposit memory);

250:         uint32 depositNonce,

263:     function retrieveDeposit(uint32 depositNonce, GasParams calldata gasParams) external payable;

270:     function redeemDeposit(uint32 depositNonce) external;

286:         uint32 settlementNonce,

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L109) [#L250](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L250) [#L263](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L263) [#L270](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L270) [#L286](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchBridgeAgent.sol#L286) 

```solidity
File: src/interfaces/IBranchRouter.sol

79:     function getDepositEntry(uint32 depositNonce) external view returns (Deposit memory);

```
[#L79](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IBranchRouter.sol#L79) 

```solidity
File: src/interfaces/IERC20hTokenBranchFactory.sol

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals, bool _addPrefix)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenBranchFactory.sol#L24) 

```solidity
File: src/interfaces/IERC20hTokenRoot.sol

19:     function localChainId() external view returns (uint16);

```
[#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRoot.sol#L19) 

```solidity
File: src/interfaces/IERC20hTokenRootFactory.sol

24:     function createToken(string memory _name, string memory _symbol, uint8 _decimals)

```
[#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IERC20hTokenRootFactory.sol#L24) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

16:         uint16 _dstChainId,

32:         uint16 _srcChainId,

35:         uint64 _nonce,

43:     function getInboundNonce(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (uint64);

43:     function getInboundNonce(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (uint64);

47:     function getOutboundNonce(uint16 _dstChainId, address _srcAddress) external view returns (uint64);

47:     function getOutboundNonce(uint16 _dstChainId, address _srcAddress) external view returns (uint64);

56:         uint16 _dstChainId,

64:     function getChainId() external view returns (uint16);

70:     function retryPayload(uint16 _srcChainId, bytes calldata _srcAddress, bytes calldata _payload) external;

75:     function hasStoredPayload(uint16 _srcChainId, bytes calldata _srcAddress) external view returns (bool);

98:     function getConfig(uint16 _version, uint16 _chainId, address _userApplication, uint256 _configType)

98:     function getConfig(uint16 _version, uint16 _chainId, address _userApplication, uint256 _configType)

105:     function getSendVersion(address _userApplication) external view returns (uint16);

109:     function getReceiveVersion(address _userApplication) external view returns (uint16);

```
[#L16](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L16) [#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L32) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L35) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L43) [#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L43) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L47) [#L47](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L47) [#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L56) [#L64](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L64) [#L70](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L70) [#L75](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L75) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L98) [#L98](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L98) [#L105](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L105) [#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L109) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

11:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64 _nonce, bytes calldata _payload) external;

11:     function lzReceive(uint16 _srcChainId, bytes calldata _srcAddress, uint64 _nonce, bytes calldata _payload) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L11) [#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L11) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

11:     function setConfig(uint16 _version, uint16 _chainId, uint256 _configType, bytes calldata _config) external;

11:     function setConfig(uint16 _version, uint16 _chainId, uint256 _configType, bytes calldata _config) external;

15:     function setSendVersion(uint16 _version) external;

19:     function setReceiveVersion(uint16 _version) external;

24:     function forceResumeReceive(uint16 _srcChainId, bytes calldata _srcAddress) external;

```
[#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L11) [#L11](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L11) [#L15](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L15) [#L19](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L19) [#L24](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L24) 

```solidity
File: src/interfaces/IRootBridgeAgent.sol

104:     function settlementNonce() external view returns (uint32 nonce);

111:     function getSettlementEntry(uint32 _settlementNonce) external view returns (Settlement memory);

153:         uint16 _dstChainId

171:         uint16 _dstChainId,

192:         uint16 _dstChainId,

216:         uint16 _dstChainId,

237:         uint32 _settlementNonce,

250:     function retrieveSettlement(uint32 _settlementNonce, GasParams calldata _gParams) external payable;

257:     function redeemSettlement(uint32 _depositNonce) external;

311:         uint16 _srcChainId,

```
[#L104](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L104) [#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L111) [#L153](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L153) [#L171](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L171) [#L192](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L192) [#L216](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L216) [#L237](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L237) [#L250](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L250) [#L257](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L257) [#L311](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootBridgeAgent.sol#L311) 

```solidity
File: src/interfaces/IRootPort.sol

17:         uint16 _dstChainId,

324:         uint8 _wrappedGasTokenDecimals,

354:         uint16 _dstChainId,

364:     function syncNewCoreBranchRouter(address _coreBranchRouter, address _coreBranchBridgeAgent, uint16 _dstChainId)

389:         address indexed coreBranchRouter, address indexed coreBranchBridgeAgent, uint16 indexed dstChainId

392:         address indexed coreBranchRouter, address indexed coreBranchBridgeAgent, uint16 indexed dstChainId

```
[#L17](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L17) [#L324](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L324) [#L354](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L354) [#L364](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L364) [#L389](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L389) [#L392](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootPort.sol#L392) 

```solidity
File: src/interfaces/IRootRouter.sol

25:     function executeResponse(bytes memory params, uint16 srcChainId) external payable;

33:     function execute(bytes memory params, uint16 srcChainId) external payable;

42:     function executeDepositSingle(bytes memory params, DepositParams memory dParams, uint16 srcChainId)

53:     function executeDepositMultiple(bytes memory params, DepositMultipleParams memory dParams, uint16 srcChainId)

63:     function executeSigned(bytes memory params, address userAccount, uint16 srcChainId) external payable;

76:         uint16 srcChainId

90:         uint16 srcChainId

```
[#L25](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L25) [#L33](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L33) [#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L42) [#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L53) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L63) [#L76](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L76) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/IRootRouter.sol#L90) 

```solidity
File: src/token/ERC20hTokenBranch.sol

18:         uint8 _decimals,

```
[#L18](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L18) 

```solidity
File: src/token/ERC20hTokenRoot.sol

14:     uint16 public immutable override localChainId;

32:         uint16 _localChainId,

37:         uint8 _decimals

```
[#L14](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L14) [#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L32) [#L37](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L37) 

</details>

---

<a name="GAS-32"></a> 
### [GAS-32] Constructors can be marked as `payable` to save deployment gas
Payable functions cost less gas to execute, because the compiler does not have to add extra checks to ensure that no payment is provided. A constructor can be safely marked as payable, because only the deployer would be able to pass funds, and the project itself would not pass any funds.

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

38:     constructor(uint16 _localChainId, address _rootPortAddress, address _owner) BranchPort(_owner) {

```
[#L38](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L38) 

```solidity
File: src/ArbitrumCoreBranchRouter.sol

44:     constructor() CoreBranchRouter(address(0)) {}

```
[#L44](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumCoreBranchRouter.sol#L44) 

```solidity
File: src/BaseBranchRouter.sol

48:     constructor() {

```
[#L48](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L48) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

39:     constructor() {

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L39) 

```solidity
File: src/BranchPort.sol

108:     constructor(address _owner) {

```
[#L108](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L108) 

```solidity
File: src/CoreBranchRouter.sol

30:     constructor(address _hTokenFactoryAddress) BaseBranchRouter() {

```
[#L30](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreBranchRouter.sol#L30) 

```solidity
File: src/CoreRootRouter.sol

71:     constructor(uint256 _rootChainId, address _rootPortAddress) {

```
[#L71](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L71) 

```solidity
File: src/MulticallRootRouter.sol

92:     constructor(uint256 _localChainId, address _localPortAddress, address _multicallAddress) {

```
[#L92](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L92) 

```solidity
File: src/RootBridgeAgentExecutor.sol

35:     constructor(address _rootBridgeAgent) {

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgentExecutor.sol#L35) 

```solidity
File: src/RootPort.sol

111:     constructor(uint256 _localChainId) {

```
[#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L111) 

```solidity
File: src/VirtualAccount.sol

35:     constructor(address _userAddress, address _localPortAddress) {

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L35) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

42:     constructor(uint16 _localChainId, address _localPortAddress, string memory _chainName, string memory _chainSymbol) {

```
[#L42](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L42) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

34:     constructor(uint16 _localChainId, address _rootPortAddress) {

```
[#L34](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L34) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

31:     constructor(uint16 _rootChainId, address _lzEndpointAddress, address _rootPortAddress) {

```
[#L31](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L31) 

</details>

---

<a name="GAS-33"></a> 
### [GAS-33] Functions guaranteed to revert when called by normal users can be marked `payable`
If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function. Marking the function as `payable` will lower the gas cost for legitimate callers because the compiler will not include checks for whether a payment was provided.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: src/BaseBranchRouter.sol

60:     function initialize(address _localBridgeAgentAddress) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L60) 

```solidity
File: src/BranchBridgeAgentExecutor.sol

53:     function executeNoSettlement(address _router, bytes calldata _payload) external payable onlyOwner {

```
[#L53](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgentExecutor.sol#L53) 

```solidity
File: src/BranchPort.sol

122:     function initialize(address _coreBranchRouter, address _bridgeAgentFactory) external virtual onlyOwner {

135:     function renounceOwnership() public payable override onlyOwner {

```
[#L122](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L122) [#L135](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L135) 

```solidity
File: src/CoreRootRouter.sol

83:     function initialize(address _bridgeAgentAddress, address _hTokenFactory) external onlyOwner {

```
[#L83](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L83) 

```solidity
File: src/MulticallRootRouter.sol

109:     function initialize(address _bridgeAgentAddress) external onlyOwner {

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L109) 

```solidity
File: src/RootPort.sol

129:     function initialize(address _bridgeAgentFactory, address _coreRootRouter) external onlyOwner {

166:     function renounceOwnership() public payable override onlyOwner {

414:     function toggleBridgeAgent(address _bridgeAgent) external override onlyOwner {

421:     function addBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

431:     function toggleBridgeAgentFactory(address _bridgeAgentFactory) external override onlyOwner {

483:     function addEcosystemToken(address _ecoTokenGlobalAddress) external override onlyOwner {

509:     function setCoreRootRouter(address _coreRootRouter, address _coreRootBridgeAgent) external override onlyOwner {

```
[#L129](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L129) [#L166](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L166) [#L414](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L414) [#L421](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L421) [#L431](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L431) [#L483](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L483) [#L509](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L509) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

56:     function initialize(address _coreRootBridgeAgent) external override onlyOwner {

```
[#L56](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L56) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

87:     function initialize(address _coreRootBridgeAgent) external virtual onlyOwner {

```
[#L87](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L87) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

60:     function initialize(address _wrappedNativeTokenAddress, address _coreRouter) external onlyOwner {

```
[#L60](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L60) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

49:     function initialize(address _coreRouter) external onlyOwner {

```
[#L49](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L49) 

```solidity
File: src/token/ERC20hTokenBranch.sol

29:     function mint(address account, uint256 amount) external override onlyOwner returns (bool) {

35:     function burn(uint256 amount) public override onlyOwner {

```
[#L29](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L29) [#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenBranch.sol#L35) 

```solidity
File: src/token/ERC20hTokenRoot.sol

57:     function mint(address to, uint256 amount, uint256 chainId) external onlyOwner returns (bool) {

69:     function burn(address from, uint256 amount, uint256 chainId) external onlyOwner {

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L57) [#L69](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L69) 

</details>

---

<a name="GAS-34"></a> 
### [GAS-34] `++i` costs less gas than `i++`, especially when it's used in `for`-loops (`--i`/`i--` too)
*Saves 5 gas per loop*

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: src/BranchBridgeAgent.sol

188:         bytes memory payload = abi.encodePacked(bytes1(0x00), depositNonce++, _params);

202:         bytes memory payload = abi.encodePacked(bytes1(0x01), depositNonce++, _params);

269:         bytes memory payload = abi.encodePacked(bytes1(0x04), msg.sender, depositNonce++, _params);

```
[#L188](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L188) [#L202](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L202) [#L269](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L269) 

```solidity
File: src/BranchPort.sol

309:                 i++;

```
[#L309](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L309) 

```solidity
File: src/RootBridgeAgent.sol

168:         bytes memory payload = abi.encodePacked(bytes1(0x00), _recipient, settlementNonce++, _params);

```
[#L168](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L168) 

</details>

---

<a name="GAS-35"></a> 
### [GAS-35] Use `!= 0` instead of `> 0` for unsigned integer comparison
Using `== 0`, `!= 0` instead of `> 0`, `>= 1`, `< 1`, `<= 0` can save gas.

<details>
<summary>
There are <b>21</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

127:         if (_deposit > 0) {

132:         if (_amount - _deposit > 0) {

```
[#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L127) [#L132](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L132) 

```solidity
File: src/BaseBranchRouter.sol

165:         if (_amount - _deposit > 0) {

173:         if (_deposit > 0) {

```
[#L165](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L165) [#L173](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L173) 

```solidity
File: src/BranchBridgeAgent.sol

906:         if (_amount - _deposit > 0) {

912:         if (_deposit > 0) {

```
[#L906](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L906) [#L912](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L912) 

```solidity
File: src/BranchPort.sol

259:             if (_amounts[i] - _deposits[i] > 0) {

266:             if (_deposits[i] > 0) {

525:         if (_hTokenAmount > 0) {

531:         if (_deposit > 0) {

```
[#L259](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L259) [#L266](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L266) [#L525](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L525) [#L531](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L531) 

```solidity
File: src/RootBridgeAgent.sol

363:         if (_dParams.amount > 0) {

370:         if (_dParams.deposit > 0) {

1146:         if (_underlyingAddress == address(0)) if (_deposit > 0) revert UnrecognizedUnderlyingAddress();

1149:         if (_amount - _deposit > 0) {

1156:         if (_deposit > 0) {

```
[#L363](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L363) [#L370](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L370) [#L1146](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1146) [#L1149](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1149) [#L1156](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1156) 

```solidity
File: src/RootPort.sol

284:         if (_amount - _deposit > 0) {

290:         if (_deposit > 0) if (!ERC20hTokenRoot(_hToken).mint(_recipient, _deposit, _srcChainId)) revert UnableToMint();

```
[#L284](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L284) [#L290](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L290) 

```solidity
File: src/VirtualAccount.sol

152:         return size > 0;

```
[#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/VirtualAccount.sol#L152) 

```solidity
File: src/interfaces/ILayerZeroEndpoint.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroEndpoint.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroReceiver.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroReceiver.sol#L3) 

```solidity
File: src/interfaces/ILayerZeroUserApplicationConfig.sol

3: pragma solidity >=0.5.0;

```
[#L3](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/interfaces/ILayerZeroUserApplicationConfig.sol#L3) 

</details>

---

<a name="GAS-36"></a> 
### [GAS-36] Using assembly to check for zero can save gas
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

<details>
<summary>
There are <b>74</b> instances (click to show):
</summary>

```solidity
File: src/ArbitrumBranchPort.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

63:         if (_globalToken == address(0)) revert UnknownGlobalToken();

90:         if (_underlyingAddress == address(0)) revert UnknownUnderlyingToken();

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L39) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L63) [#L90](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/ArbitrumBranchPort.sol#L90) 

```solidity
File: src/BaseBranchRouter.sol

61:         require(_localBridgeAgentAddress != address(0), "Bridge Agent address cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BaseBranchRouter.sol#L61) 

```solidity
File: src/BranchBridgeAgent.sol

125:         require(_rootBridgeAgentAddress != address(0), "Root Bridge Agent Address cannot be the zero address.");

127:             _lzEndpointAddress != address(0) || _rootChainId == _localChainId,

130:         require(_localRouterAddress != address(0), "Local Router Address cannot be the zero address.");

131:         require(_localPortAddress != address(0), "Local Port Address cannot be the zero address.");

412:         if (payload.length == 0) revert DepositRetryUnavailableUseCallout();

440:         if (deposit.owner == address(0)) revert DepositRedeemUnavailable();

```
[#L125](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L125) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L127) [#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L131) [#L412](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L412) [#L440](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchBridgeAgent.sol#L440) 

```solidity
File: src/BranchPort.sol

109:         require(_owner != address(0), "Owner is zero address");

123:         require(coreBranchRouterAddress == address(0), "Contract already initialized");

126:         require(_coreBranchRouter != address(0), "CoreBranchRouter is zero address");

127:         require(_bridgeAgentFactory != address(0), "BridgeAgentFactory is zero address");

332:         require(coreBranchRouterAddress != address(0), "CoreRouter address is zero");

333:         require(_newCoreRouter != address(0), "New CoreRouter address is zero");

```
[#L109](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L109) [#L123](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L123) [#L126](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L126) [#L127](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L127) [#L332](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L332) [#L333](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/BranchPort.sol#L333) 

```solidity
File: src/CoreRootRouter.sol

120:         if (IBridgeAgent(_rootBridgeAgent).getBranchBridgeAgent(_dstChainId) != address(0)) revert InvalidChainId();

```
[#L120](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/CoreRootRouter.sol#L120) 

```solidity
File: src/MulticallRootRouter.sol

93:         require(_localPortAddress != address(0), "Local Port Address cannot be 0");

94:         require(_multicallAddress != address(0), "Multicall Address cannot be 0");

110:         require(_bridgeAgentAddress != address(0), "Bridge Agent Address cannot be 0");

```
[#L93](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L93) [#L94](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L94) [#L110](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/MulticallRootRouter.sol#L110) 

```solidity
File: src/RootBridgeAgent.sol

111:         require(_lzEndpointAddress != address(0), "Layerzero Enpoint Address cannot be zero address");

112:         require(_localPortAddress != address(0), "Port Address cannot be zero address");

113:         require(_localRouterAddress != address(0), "Router Address cannot be zero address");

244:         if (settlementReference.owner == address(0)) revert SettlementRetryUnavailable();

282:         if (settlementOwner == address(0)) revert SettlementRetrieveUnavailable();

308:         if (settlementOwner == address(0)) revert SettlementRedeemUnavailable();

323:             if (_hToken != address(0)) {

670:             if (settlementReference.owner == address(0)) revert SettlementRetryUnavailable();

818:         if (callee == address(0)) revert UnrecognizedBridgeAgent();

871:         if (_hTokens.length == 0) revert SettlementRetryUnavailableUseCallout();

910:         if (callee == address(0)) revert UnrecognizedBridgeAgent();

1141:         if (_amount == 0 && _deposit == 0) revert InvalidInputParams();

1141:         if (_amount == 0 && _deposit == 0) revert InvalidInputParams();

1145:         if (_localAddress == address(0)) revert UnrecognizedLocalAddress();

1146:         if (_underlyingAddress == address(0)) if (_deposit > 0) revert UnrecognizedUnderlyingAddress();

1171:         if (getBranchBridgeAgent[_branchChainId] != address(0)) revert AlreadyAddedBridgeAgent();

```
[#L111](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L111) [#L112](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L112) [#L113](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L113) [#L244](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L244) [#L282](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L282) [#L308](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L308) [#L323](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L323) [#L670](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L670) [#L818](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L818) [#L871](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L871) [#L910](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L910) [#L1141](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1141) [#L1141](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1141) [#L1145](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1145) [#L1146](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1146) [#L1171](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootBridgeAgent.sol#L1171) 

```solidity
File: src/RootPort.sol

130:         require(_bridgeAgentFactory != address(0), "Bridge Agent Factory cannot be 0 address.");

131:         require(_coreRootRouter != address(0), "Core Root Router cannot be 0 address.");

152:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0 address.");

153:         require(_coreLocalBranchBridgeAgent != address(0), "Core Local Branch Bridge Agent cannot be 0 address.");

154:         require(_localBranchPortAddress != address(0), "Local Branch Port Address cannot be 0 address.");

212:         return getLocalTokenFromGlobal[_globalAddress][_srcChainId] != address(0);

217:         return getGlobalTokenFromLocal[_localAddress][_srcChainId] != address(0);

226:         return _getLocalToken(_localAddress, _srcChainId, _dstChainId) != address(0);

231:         return getLocalTokenFromUnderlying[_underlyingToken][_srcChainId] != address(0);

245:         if (_globalAddress == address(0)) revert InvalidGlobalAddress();

246:         if (_localAddress == address(0)) revert InvalidLocalAddress();

247:         if (_underlyingAddress == address(0)) revert InvalidUnderlyingAddress();

264:         if (_localAddress == address(0)) revert InvalidLocalAddress();

352:         if (address(account) == address(0)) account = addVirtualAccount(_user);

360:         if (_user == address(0)) revert InvalidUserAddress();

398:         if (IBridgeAgent(_rootBridgeAgent).getBranchBridgeAgent(_branchChainId) != address(0)) {

488:         if (getUnderlyingTokenFromLocal[_ecoTokenGlobalAddress][localChainId] != address(0)) {

493:         if (getLocalTokenFromUnderlying[_ecoTokenGlobalAddress][localChainId] != address(0)) {

510:         if (_coreRootRouter == address(0)) revert InvalidCoreRootRouter();

511:         if (_coreRootBridgeAgent == address(0)) revert InvalidCoreRootBridgeAgent();

528:         if (_coreBranchRouter == address(0)) revert InvalidCoreBranchRouter();

529:         if (_coreBranchBridgeAgent == address(0)) revert InvalidCoreBrancBridgeAgent();

544:         if (_coreBranchRouter == address(0)) revert InvalidCoreBranchRouter();

545:         if (_coreBranchBridgeAgent == address(0)) revert InvalidCoreBrancBridgeAgent();

```
[#L130](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L130) [#L131](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L131) [#L152](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L152) [#L153](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L153) [#L154](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L154) [#L212](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L212) [#L217](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L217) [#L226](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L226) [#L231](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L231) [#L245](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L245) [#L246](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L246) [#L247](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L247) [#L264](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L264) [#L352](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L352) [#L360](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L360) [#L398](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L398) [#L488](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L488) [#L493](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L493) [#L510](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L510) [#L511](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L511) [#L528](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L528) [#L529](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L529) [#L544](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L544) [#L545](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/RootPort.sol#L545) 

```solidity
File: src/factories/ArbitrumBranchBridgeAgentFactory.sol

57:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent Address cannot be 0");

```
[#L57](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ArbitrumBranchBridgeAgentFactory.sol#L57) 

```solidity
File: src/factories/BranchBridgeAgentFactory.sol

61:         require(_rootBridgeAgentFactoryAddress != address(0), "Root Bridge Agent Factory Address cannot be 0");

63:             _lzEndpointAddress != address(0) || _rootChainId == _localChainId,

66:         require(_localCoreBranchRouterAddress != address(0), "Core Branch Router Address cannot be 0");

67:         require(_localPortAddress != address(0), "Port Address cannot be 0");

68:         require(_owner != address(0), "Owner cannot be 0");

88:         require(_coreRootBridgeAgent != address(0), "Core Root Bridge Agent cannot be 0");

```
[#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L61) [#L63](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L63) [#L66](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L66) [#L67](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L67) [#L68](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L68) [#L88](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/BranchBridgeAgentFactory.sol#L88) 

```solidity
File: src/factories/ERC20hTokenBranchFactory.sol

43:         require(_localPortAddress != address(0), "Port address cannot be 0");

61:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L43](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L43) [#L61](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenBranchFactory.sol#L61) 

```solidity
File: src/factories/ERC20hTokenRootFactory.sol

35:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

50:         require(_coreRouter != address(0), "CoreRouter address cannot be 0");

```
[#L35](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L35) [#L50](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/ERC20hTokenRootFactory.sol#L50) 

```solidity
File: src/factories/RootBridgeAgentFactory.sol

32:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

```
[#L32](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/factories/RootBridgeAgentFactory.sol#L32) 

```solidity
File: src/token/ERC20hTokenRoot.sol

39:         require(_rootPortAddress != address(0), "Root Port Address cannot be 0");

40:         require(_factoryAddress != address(0), "Factory Address cannot be 0");

```
[#L39](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L39) [#L40](https://github.com/code-423n4/2023-09-maia/blob/f5ba4de628836b2a29f9b5fff59499690008c463/src/token/ERC20hTokenRoot.sol#L40) 

</details>

---

