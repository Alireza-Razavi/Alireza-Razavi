# Report


## Medium Issues


Total <b>12</b> instances over <b>1</b> issue:

|ID|Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | Centralization Risk for trusted owners | 12 |

## Low Issues


Total <b>25</b> instances over <b>10</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Governance functions should be controlled by time locks | 4 |
| [L-2](#L-2) | Missing storage gap for upgradable contracts | 2 |
| [L-3](#L-3) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 1 |
| [L-4](#L-4) | Using zero as a parameter | 9 |
| [L-5](#L-5) | Zero address check in initializer | 1 |
| [L-6](#L-6) | Empty Function Body - Consider commenting why | 2 |
| [L-7](#L-7) | Initializers could be front-run | 2 |
| [L-8](#L-8) | Functions calling contracts/addresses with transfer hooks should be protected by reentrancy guard | 1 |
| [L-9](#L-9) | Unsafe ERC20 operation(s) | 1 |
| [L-10](#L-10) | Upgradable contracts need a constructor to lock the implementation contract when it is deployed | 2 |

## Non Critical Issues


Total <b>397</b> instances over <b>30</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | `assert()` should be replaced with `require()` or `revert()` | 2 |
| [NC-2](#NC-2) | Contract declarations should have NatSpec `@author` annotations | 8 |
| [NC-3](#NC-3) | Custom errors has no error details | 1 |
| [NC-4](#NC-4) | Custom errors should be used rather than `revert()`/`require()` | 25 |
| [NC-5](#NC-5) | Functions and modifiers should be named in mixedCase style | 2 |
| [NC-6](#NC-6) | Import declarations should import specific identifiers, rather than the whole file | 52 |
| [NC-7](#NC-7) | Missing zero address check in functions with address parameters | 60 |
| [NC-8](#NC-8) | Consider moving `msg.sender` checks to `modifier`s | 9 |
| [NC-9](#NC-9) | NatSpec documentation for contract is missing | 3 |
| [NC-10](#NC-10) | Event declarations should have NatSpec descriptions | 13 |
| [NC-11](#NC-11) | NatSpec documentation for function is missing | 31 |
| [NC-12](#NC-12) | Missing NatSpec `@param` | 38 |
| [NC-13](#NC-13) | Public variable declarations should have NatSpec descriptions | 6 |
| [NC-14](#NC-14) | NatSpec `@return` is missing | 46 |
| [NC-15](#NC-15) | Redundant inheritance specifier | 1 |
| [NC-16](#NC-16) | Contract declarations should have NatSpec `@title` annotations | 2 |
| [NC-17](#NC-17) | Lines are too long | 2 |
| [NC-18](#NC-18) | Unused contract variables | 7 |
| [NC-19](#NC-19) | Consider using `delete` rather than assigning zero to clear values | 5 |
| [NC-20](#NC-20) | Expressions for constant values should use `immutable` rather than `constant` | 1 |
| [NC-21](#NC-21) | Use `@inheritdoc` for overridden functions | 6 |
| [NC-22](#NC-22) | Visibility of state variables is not explicitly defined | 1 |
| [NC-23](#NC-23) | Whitespace in Expressions | 5 |
| [NC-24](#NC-24) | Common functions should be refactored to a common base contract | 2 |
| [NC-25](#NC-25) | Names of `private`/`internal` functions should be prefixed with an underscore | 32 |
| [NC-26](#NC-26) | Names of `private`/`internal` state variables should be prefixed with an underscore | 6 |
| [NC-27](#NC-27) | Variables should be named in mixedCase style | 1 |
| [NC-28](#NC-28) | `TODO`s left in the code | 1 |
| [NC-29](#NC-29) | Event is missing `indexed` fields | 12 |
| [NC-30](#NC-30) | Functions not used internally could be marked external | 17 |

## Gas Optimizations


Total <b>99</b> instances over <b>8</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [GAS-1](#GAS-1) | Use `calldata` instead of `memory` for function arguments that do not get mutated | 2 |
| [GAS-2](#GAS-2) | Use Custom Errors | 25 |
| [GAS-3](#GAS-3) | Don't use `SafeMath` once the solidity version is 0.8.0 or greater | 2 |
| [GAS-4](#GAS-4) | Long revert strings | 10 |
| [GAS-5](#GAS-5) | Functions guaranteed to revert when called by normal users can be marked `payable` | 15 |
| [GAS-6](#GAS-6) | Use != 0 instead of > 0 for unsigned integer comparison | 14 |
| [GAS-7](#GAS-7) | Using assembly to check for zero can save gas | 26 |
| [GAS-8](#GAS-8) | `internal` functions not called by the contract should be removed | 5 |

## Medium Issues

<a name="M-1"></a> 
#### [M-1] Centralization Risk for trusted owners
Contracts have owners with privileged rights to perform admin tasks and need to be trusted to not perform malicious updates or drain funds.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

155:     function setUnbondingPeriod(uint64 _unbondingPeriod) external onlyControllerOwner {

167:     function setTreasuryRewardCutRate(uint256 _cutRate) external onlyControllerOwner {

176:     function setTreasuryBalanceCeiling(uint256 _ceiling) external onlyControllerOwner {

186:     function setNumActiveTranscoders(uint256 _numActiveTranscoders) external onlyControllerOwner {

306:     ) external whenSystemNotPaused onlyTicketBroker {

399:     ) external whenSystemNotPaused onlyVerifier autoClaimEarnings(_transcoder) autoCheckpoint(_transcoder) {

462:     function setCurrentRoundTotalActiveStake() external onlyRoundsManager {

```
[#L155](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L155) [#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L167) [#L176](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L176) [#L186](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L186) [#L306](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L306) [#L399](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L399) [#L462](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L462) 

```solidity
File: contracts/bonding/BondingVotes.sol

167:     function getPastVotes(address _account, uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

194:     function getPastTotalSupply(uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

218:     function delegatedAt(address _account, uint256 _round) external view onlyPastRounds(_round) returns (address) {

266:     ) external virtual onlyBondingManager {

303:     function checkpointTotalActiveStake(uint256 _totalStake, uint256 _round) external virtual onlyBondingManager {

```
[#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L167) [#L194](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L194) [#L218](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L218) [#L266](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L266) [#L303](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L303) 

</details>

---


## Low Issues

<a name="L-1"></a> 
#### [L-1] Governance functions should be controlled by time locks
Governance functions (such as upgrading contracts, setting critical parameters) should be controlled using time locks to introduce a delay between a proposal and its execution. This gives users time to exit before a potentially dangerous or malicious operation is applied.

<details>
<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

155:     function setUnbondingPeriod(uint64 _unbondingPeriod) external onlyControllerOwner {

167:     function setTreasuryRewardCutRate(uint256 _cutRate) external onlyControllerOwner {

176:     function setTreasuryBalanceCeiling(uint256 _ceiling) external onlyControllerOwner {

186:     function setNumActiveTranscoders(uint256 _numActiveTranscoders) external onlyControllerOwner {

```
[#L155](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L155) [#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L167) [#L176](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L176) [#L186](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L186) 

</details>

---

<a name="L-2"></a> 
#### [L-2] Missing storage gap for upgradable contracts
Each upgradable contract should include a state variable (usually named `__gap`) to provide reserved space in storage. This allows the team to freely add new state variables in the future upgrades without compromising the storage compatibility with existing deployments.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

21: abstract contract GovernorCountingOverridable is Initializable, GovernorUpgradeable {

```
[#L21](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L21) 

```solidity
File: contracts/treasury/Treasury.sol

15: contract Treasury is Initializable, TimelockControllerUpgradeable {

```
[#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L15) 

</details>

---

<a name="L-3"></a> 
#### [L-3] Solidity version 0.8.20 or above may not work on other chains due to PUSH0
Solidity version 0.8.20 or above uses the new [Shanghai EVM](https://blog.soliditylang.org/2023/05/10/solidity-0.8.20-release-announcement/#important-note) which introduces the PUSH0 opcode. This op code may not yet be implemented on all evm-chains or Layer2s, so deployment on these chains will fail. Consider using an earlier solidity version.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/IBondingVotes.sol

2: pragma solidity ^0.8.9;

```
[#L2](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingVotes.sol#L2) 

</details>

---

<a name="L-4"></a> 
#### [L-4] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

199:         transcoderWithHint(_rewardCut, _feeShare, address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

216:         unbondWithHint(_amount, address(0), address(0));

224:         rebondWithHint(_unbondingLockId, address(0), address(0));

233:         rebondFromUnbondedWithHint(_to, _unbondingLockId, address(0), address(0));

294:         rewardWithHint(address(0), address(0));

436:                 emit TranscoderSlashed(_transcoder, address(0), penalty, 0);

439:             emit TranscoderSlashed(_transcoder, _finder, 0, 0);

875:                 _setTreasuryRewardCutRate(0);

```
[#L199](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L199) [#L208](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L208) [#L216](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L216) [#L224](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L224) [#L233](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L233) [#L294](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L294) [#L436](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L436) [#L439](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L439) [#L875](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L875) 

</details>

---

<a name="L-5"></a> 
#### [L-5] Zero address check in initializer

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/treasury/Treasury.sol

16:     function initialize(
            uint256 minDelay,
            address[] memory proposers,
            address[] memory executors,
            address admin
        ) external initializer {

```
[#L16](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L16) 

</details>

---

<a name="L-6"></a> 
#### [L-6] Empty Function Body - Consider commenting why

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

149:     constructor(address _controller) Manager(_controller) {}

```
[#L149](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L149) 

```solidity
File: contracts/bonding/BondingVotes.sol

107:     constructor(address _controller) Manager(_controller) {}

```
[#L107](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L107) 

</details>

---

<a name="L-7"></a> 
#### [L-7] Initializers could be front-run
Initializers could be front-run, allowing an attacker to either set their own values, take ownership of the contract, and in the best case forcing a re-deployment

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/LivepeerGovernor.sol

54:     function initialize(

```
[#L54](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L54) 

```solidity
File: contracts/treasury/Treasury.sol

16:     function initialize(

```
[#L16](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L16) 

</details>

---

<a name="L-8"></a> 
#### [L-8] Functions calling contracts/addresses with transfer hooks should be protected by reentrancy guard
Even if the function follows the best practice of check-effects-interaction, not using a reentrancy guard when there may be transfer hooks opens the users of this protocol up to [read-only reentrancy vulnerability](https://chainsecurity.com/curve-lp-oracle-manipulation-post-mortem/) with no way to protect them except by block-listing the entire protocol.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

285:         minter().trustedWithdrawETH(_recipient, _amount);

```
[#L285](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L285) 

</details>

---

<a name="L-9"></a> 
#### [L-9] Unsafe ERC20 operation(s)

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

616:             livepeerToken().transferFrom(msg.sender, address(minter()), _amount);

```
[#L616](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L616) 

</details>

---

<a name="L-10"></a> 
#### [L-10] Upgradable contracts need a constructor to lock the implementation contract when it is deployed
An uninitialized contract can be taken over by an attacker. For an upgradable contract, this applies to both the proxy and its implementation contract, which may impact the proxy. To prevent the implementation contract from being used, we should trigger the initialization in the constructor to automatically lock it when it is deployed. For contracts that inherit `Initializable`, the `_disableInitializers()` function [is suggested to do this job.](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/4d9d9073b84f56fe3eea360e5067c6ffd864c43d/contracts/proxy/utils/Initializable.sol#L43-L56)

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

21: abstract contract GovernorCountingOverridable is Initializable, GovernorUpgradeable {

```
[#L21](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L21) 

```solidity
File: contracts/treasury/Treasury.sol

15: contract Treasury is Initializable, TimelockControllerUpgradeable {

```
[#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L15) 

</details>

---


## Non Critical Issues

<a name="NC-1"></a> 
#### [NC-1] `assert()` should be replaced with `require()` or `revert()`
In versions of Solidity prior to 0.8.0, when encountering an assert all the remaining gas will be consumed. Even after solidity 0.8.0, the assert function is still not recommended, as described in the [documentation](https://docs.soliditylang.org/en/v0.8.20/control-structures.html#panic-via-assert-and-error-via-require):
> Assert should only be used to test for internal errors, and to check invariants. Properly functioning code should never create a Panic, not even on invalid external input. If this happens, then there is a bug in your contract which you should fix.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

41:         assert(upperIdx < len);

```
[#L41](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L41) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

206:                 assert(delegateSupport == VoteType.Abstain);

```
[#L206](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L206) 

</details>

---

<a name="NC-2"></a> 
#### [NC-2] Contract declarations should have NatSpec `@author` annotations

<details>
<summary>
There are <b>8</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

23: contract BondingManager is ManagerProxyTarget, IBondingManager {

```
[#L23](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L23) 

```solidity
File: contracts/bonding/BondingVotes.sol

20: contract BondingVotes is ManagerProxyTarget, IBondingVotes {

```
[#L20](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L20) 

```solidity
File: contracts/bonding/IBondingManager.sol

8: interface IBondingManager {

```
[#L8](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L8) 

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

9: library EarningsPoolLIP36 {

```
[#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L9) 

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

12: library SortedArrays {

```
[#L12](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L12) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

21: abstract contract GovernorCountingOverridable is Initializable, GovernorUpgradeable {

```
[#L21](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L21) 

```solidity
File: contracts/treasury/IVotes.sol

6: interface IVotes is IERC5805Upgradeable {

```
[#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L6) 

```solidity
File: contracts/treasury/Treasury.sol

15: contract Treasury is Initializable, TimelockControllerUpgradeable {

```
[#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L15) 

</details>

---

<a name="NC-3"></a> 
#### [NC-3] Custom errors has no error details
Consider adding parameters to the error to indicate which user or values caused the failure.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

23:     error VoteAlreadyCast();

```
[#L23](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L23) 

</details>

---

<a name="NC-4"></a> 
#### [NC-4] Custom errors should be used rather than `revert()`/`require()`
Custom errors are available from solidity version 0.8.4. Custom errors are more easily processed in try-catch blocks, and are easier to re-use and maintain.

<details>
<summary>
There are <b>25</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

253:         require(isValidUnbondingLock(msg.sender, _unbondingLockId), "invalid unbonding lock ID");

279:         require(_recipient != address(0), "invalid recipient");

281:         require(fees >= _amount, "insufficient fees to withdraw");

310:         require(isRegisteredTranscoder(_transcoder), "transcoder must be registered");

491:         require(!roundsManager().currentRoundLocked(), "can't update transcoder params, current round is locked");

492:         require(MathUtils.validPerc(_rewardCut), "invalid rewardCut percentage");

493:         require(MathUtils.validPerc(_feeShare), "invalid feeShare percentage");

494:         require(isRegisteredTranscoder(msg.sender), "transcoder must be registered");

563:                 require(_to != _owner, "INVALID_DELEGATE");

565:                 require(currentDelegate == _to, "INVALID_DELEGATE_CHANGE");

582:             require(!isRegisteredTranscoder(_owner), "registered transcoders can't delegate towards other addresses");

606:         require(delegationAmount > 0, "delegation amount must be greater than 0");

722:             require(oldDelDelegate != _delegator, "INVALID_DELEGATOR");

750:         require(delegatorStatus(msg.sender) == DelegatorStatus.Bonded, "caller must be bonded");

754:         require(_amount > 0, "unbond amount must be greater than 0");

755:         require(_amount <= del.bondedAmount, "amount is greater than bonded amount");

801:         require(delegatorStatus(msg.sender) != DelegatorStatus.Unbonded, "caller must be bonded");

824:         require(delegatorStatus(msg.sender) == DelegatorStatus.Unbonded, "caller must be unbonded");

850:         require(isActiveTranscoder(msg.sender), "caller must be an active transcoder");

1177:         require(PreciseMathUtils.validPerc(_cutRate), "_cutRate is invalid precise percentage");

1573:         require(isValidUnbondingLock(_delegator, _unbondingLockId), "invalid unbonding lock ID");

1652:         require(msg.sender == controller.getContract(keccak256("TicketBroker")), "caller must be TicketBroker");

1656:         require(msg.sender == controller.getContract(keccak256("RoundsManager")), "caller must be RoundsManager");

1660:         require(msg.sender == controller.getContract(keccak256("Verifier")), "caller must be Verifier");

1664:         require(roundsManager().currentRoundInitialized(), "current round is not initialized");

```
[#L253](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L253) [#L279](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L279) [#L281](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L281) [#L310](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L310) [#L491](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L491) [#L492](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L492) [#L493](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L493) [#L494](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L494) [#L563](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L563) [#L565](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L565) [#L582](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L582) [#L606](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L606) [#L722](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L722) [#L750](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L750) [#L754](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L754) [#L755](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L755) [#L801](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L801) [#L824](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L824) [#L850](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L850) [#L1177](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1177) [#L1573](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1573) [#L1652](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1652) [#L1656](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1656) [#L1660](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1660) [#L1664](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1664) 

</details>

---

<a name="NC-5"></a> 
#### [NC-5] Functions and modifiers should be named in mixedCase style
As the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.21/style-guide.html#function-names) suggests: functions and modifiers should be named in mixedCase style.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingVotes.sol

145:     function CLOCK_MODE() external pure returns (string memory) {

```
[#L145](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L145) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

76:     function COUNTING_MODE() public pure virtual override returns (string memory) {

```
[#L76](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L76) 

</details>

---

<a name="NC-6"></a> 
#### [NC-6] Import declarations should import specific identifiers, rather than the whole file
Using import declarations of the form `import {<identifier_name>} from "some/file.sol"` avoids polluting the symbol namespace making flattened files smaller, and speeds up compilation (but does not save any gas).

<details>
<summary>
There are <b>52</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

4: import "../ManagerProxyTarget.sol";

5: import "./IBondingManager.sol";

6: import "../libraries/SortedDoublyLL.sol";

7: import "../libraries/MathUtils.sol";

8: import "../libraries/PreciseMathUtils.sol";

9: import "./libraries/EarningsPool.sol";

10: import "./libraries/EarningsPoolLIP36.sol";

11: import "../token/ILivepeerToken.sol";

12: import "../token/IMinter.sol";

13: import "../rounds/IRoundsManager.sol";

14: import "../snapshots/IMerkleSnapshot.sol";

15: import "./IBondingVotes.sol";

17: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L4) [#L5](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L5) [#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L6) [#L7](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L7) [#L8](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L8) [#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L9) [#L10](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L10) [#L11](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L11) [#L12](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L12) [#L13](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L13) [#L14](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L14) [#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L15) [#L17](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L17) 

```solidity
File: contracts/bonding/BondingVotes.sol

4: import "@openzeppelin/contracts/utils/Arrays.sol";

5: import "@openzeppelin/contracts/utils/math/SafeCast.sol";

7: import "./libraries/EarningsPool.sol";

8: import "./libraries/EarningsPoolLIP36.sol";

9: import "./libraries/SortedArrays.sol";

11: import "../ManagerProxyTarget.sol";

12: import "./IBondingVotes.sol";

13: import "./IBondingManager.sol";

14: import "../rounds/IRoundsManager.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L4) [#L5](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L5) [#L7](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L7) [#L8](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L8) [#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L9) [#L11](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L11) [#L12](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L12) [#L13](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L13) [#L14](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L14) 

```solidity
File: contracts/bonding/IBondingVotes.sol

4: import "../treasury/IVotes.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingVotes.sol#L4) 

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

4: import "./EarningsPool.sol";

5: import "../../libraries/PreciseMathUtils.sol";

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L4) [#L5](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L5) [#L7](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L7) 

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

4: import "../../libraries/MathUtils.sol";

6: import "@openzeppelin/contracts/utils/Arrays.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L4) [#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L6) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

8: import "../bonding/libraries/EarningsPool.sol";

9: import "../bonding/libraries/EarningsPoolLIP36.sol";

11: import "../Manager.sol";

12: import "../IController.sol";

13: import "../rounds/IRoundsManager.sol";

14: import "./IVotes.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L4) [#L5](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L5) [#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L6) [#L8](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L8) [#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L9) [#L11](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L11) [#L12](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L12) [#L13](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L13) [#L14](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L14) 

```solidity
File: contracts/treasury/IVotes.sol

4: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L4) 

```solidity
File: contracts/treasury/LivepeerGovernor.sol

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesUpgradeable.sol";

7: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesQuorumFractionUpgradeable.sol";

8: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorSettingsUpgradeable.sol";

9: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorTimelockControlUpgradeable.sol";

11: import "../bonding/libraries/EarningsPool.sol";

12: import "../bonding/libraries/EarningsPoolLIP36.sol";

14: import "../ManagerProxyTarget.sol";

15: import "../IController.sol";

16: import "../rounds/IRoundsManager.sol";

17: import "./GovernorCountingOverridable.sol";

18: import "./Treasury.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L4) [#L5](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L5) [#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L6) [#L7](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L7) [#L8](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L8) [#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L9) [#L11](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L11) [#L12](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L12) [#L14](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L14) [#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L15) [#L16](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L16) [#L17](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L17) [#L18](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L18) 

```solidity
File: contracts/treasury/Treasury.sol

4: import "@openzeppelin/contracts-upgradeable/governance/TimelockControllerUpgradeable.sol";

```
[#L4](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L4) 

</details>

---

<a name="NC-7"></a> 
#### [NC-7] Missing zero address check in functions with address parameters
Adding a zero address check for each address type parameter can prevent errors.

<details>
<summary>
There are <b>60</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

// Missing zero check for `_to`
207:     function bond(uint256 _amount, address _to) external {

// Missing zero check for `_to`
232:     function rebondFromUnbonded(address _to, uint256 _unbondingLockId) external {

// Missing zero check for `_account`
241:     function checkpointBondingState(address _account) external {

// Missing zero check for `_transcoder`
302:     function updateTranscoderWithFees(
             address _transcoder,
             uint256 _fees,
             uint256 _round
         ) external whenSystemNotPaused onlyTicketBroker {

// Missing zero check for `_transcoder`
394:     function slashTranscoder(
             address _transcoder,
             address _finder,
             uint256 _slashAmount,
             uint256 _finderFee
         ) external whenSystemNotPaused onlyVerifier autoClaimEarnings(_transcoder) autoCheckpoint(_transcoder) {

// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
485:     function transcoderWithHint(
             uint256 _rewardCut,
             uint256 _feeShare,
             address _newPosPrev,
             address _newPosNext
         ) public whenSystemNotPaused currentRoundInitialized {

// Missing zero check for `_owner`
// Missing zero check for `_to`
// Missing zero check for `_oldDelegateNewPosPrev`
// Missing zero check for `_oldDelegateNewPosNext`
// Missing zero check for `_currDelegateNewPosPrev`
// Missing zero check for `_currDelegateNewPosNext`
537:     function bondForWithHint(
             uint256 _amount,
             address _owner,
             address _to,
             address _oldDelegateNewPosPrev,
             address _oldDelegateNewPosNext,
             address _currDelegateNewPosPrev,
             address _currDelegateNewPosNext
         ) public whenSystemNotPaused currentRoundInitialized {

// Missing zero check for `_to`
// Missing zero check for `_oldDelegateNewPosPrev`
// Missing zero check for `_oldDelegateNewPosNext`
// Missing zero check for `_currDelegateNewPosPrev`
// Missing zero check for `_currDelegateNewPosNext`
640:     function bondWithHint(
             uint256 _amount,
             address _to,
             address _oldDelegateNewPosPrev,
             address _oldDelegateNewPosNext,
             address _currDelegateNewPosPrev,
             address _currDelegateNewPosNext
         ) public {

// Missing zero check for `_delegator`
// Missing zero check for `_oldDelegateNewPosPrev`
// Missing zero check for `_oldDelegateNewPosNext`
// Missing zero check for `_newDelegateNewPosPrev`
// Missing zero check for `_newDelegateNewPosNext`
679:     function transferBond(
             address _delegator,
             uint256 _amount,
             address _oldDelegateNewPosPrev,
             address _oldDelegateNewPosNext,
             address _newDelegateNewPosPrev,
             address _newDelegateNewPosNext
         ) public whenSystemNotPaused currentRoundInitialized {

// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
745:     function unbondWithHint(
             uint256 _amount,
             address _newPosPrev,
             address _newPosNext
         ) public whenSystemNotPaused currentRoundInitialized autoClaimEarnings(msg.sender) autoCheckpoint(msg.sender) {

// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
796:     function rebondWithHint(
             uint256 _unbondingLockId,
             address _newPosPrev,
             address _newPosNext
         ) public whenSystemNotPaused currentRoundInitialized autoClaimEarnings(msg.sender) {

// Missing zero check for `_to`
// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
818:     function rebondFromUnbondedWithHint(
             address _to,
             uint256 _unbondingLockId,
             address _newPosPrev,
             address _newPosNext
         ) public whenSystemNotPaused currentRoundInitialized autoClaimEarnings(msg.sender) {

// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
842:     function rewardWithHint(address _newPosPrev, address _newPosNext)
             public
             whenSystemNotPaused
             currentRoundInitialized
             autoCheckpoint(msg.sender)
         {

// Missing zero check for `_delegator`
908:     function pendingStake(address _delegator, uint256 _endRound) public view returns (uint256) {

// Missing zero check for `_delegator`
923:     function pendingFees(address _delegator, uint256 _endRound) public view returns (uint256) {

// Missing zero check for `_transcoder`
937:     function transcoderTotalStake(address _transcoder) public view returns (uint256) {

// Missing zero check for `_transcoder`
946:     function transcoderStatus(address _transcoder) public view returns (TranscoderStatus) {

// Missing zero check for `_delegator`
956:     function delegatorStatus(address _delegator) public view returns (DelegatorStatus) {

// Missing zero check for `_transcoder`
987:     function getTranscoder(address _transcoder)
             public
             view
             returns (
                 uint256 lastRewardRound,
                 uint256 rewardCut,
                 uint256 feeShare,
                 uint256 lastActiveStakeUpdateRound,
                 uint256 activationRound,
                 uint256 deactivationRound,
                 uint256 activeCumulativeRewards,
                 uint256 cumulativeRewards,
                 uint256 cumulativeFees,
                 uint256 lastFeeRound
             )
         {

// Missing zero check for `_transcoder`
1027:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)
              public
              view
              returns (
                  uint256 totalStake,
                  uint256 transcoderRewardCut,
                  uint256 transcoderFeeShare,
                  uint256 cumulativeRewardFactor,
                  uint256 cumulativeFeeFactor
              )
          {

// Missing zero check for `_delegator`
1058:     function getDelegator(address _delegator)
              public
              view
              returns (
                  uint256 bondedAmount,
                  uint256 fees,
                  address delegateAddress,
                  uint256 delegatedAmount,
                  uint256 startRound,
                  uint256 lastClaimRound,
                  uint256 nextUnbondingLockId
              )
          {

// Missing zero check for `_delegator`
1089:     function getDelegatorUnbondingLock(address _delegator, uint256 _unbondingLockId)
              public
              view
              returns (uint256 amount, uint256 withdrawRound)
          {

// Missing zero check for `_transcoder`
1128:     function getNextTranscoderInPool(address _transcoder) public view returns (address) {

// Missing zero check for `_transcoder`
1145:     function isActiveTranscoder(address _transcoder) public view returns (bool) {

// Missing zero check for `_transcoder`
1156:     function isRegisteredTranscoder(address _transcoder) public view returns (bool) {

// Missing zero check for `_delegator`
1167:     function isValidUnbondingLock(address _delegator, uint256 _unbondingLockId) public view returns (bool) {

// Missing zero check for `_delegator`
1259:     function pendingStakeAndFees(address _delegator, uint256 _endRound)
              internal
              view
              returns (uint256 stake, uint256 fees)
          {

// Missing zero check for `_delegate`
// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
1294:     function increaseTotalStake(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegate) {

// Missing zero check for `_delegate`
// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
1307:     function increaseTotalStakeUncheckpointed(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal {

// Missing zero check for `_delegate`
// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
1352:     function decreaseTotalStake(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegate) {

// Missing zero check for `_transcoder`
// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
1392:     function tryToJoinActiveSet(
              address _transcoder,
              uint256 _totalStake,
              uint256 _activationRound,
              address _newPosPrev,
              address _newPosNext
          ) internal {

// Missing zero check for `_transcoder`
1437:     function resignTranscoder(address _transcoder) internal {

// Missing zero check for `_transcoder`
// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
1459:     function updateTranscoderWithRewards(
              address _transcoder,
              uint256 _rewards,
              uint256 _round,
              address _newPosPrev,
              address _newPosNext
          ) internal {

// Missing zero check for `_delegator`
1500:     function updateDelegatorWithEarnings(
              address _delegator,
              uint256 _endRound,
              uint256 _lastClaimRound
          ) internal {

// Missing zero check for `_delegator`
// Missing zero check for `_newPosPrev`
// Missing zero check for `_newPosNext`
1564:     function processRebond(
              address _delegator,
              uint256 _unbondingLockId,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegator) {

// Missing zero check for `_owner`
1591:     function _checkpointBondingState(
              address _owner,
              Delegator storage _delegator,
              Transcoder storage _transcoder
          ) internal {

// Missing zero check for `_delegator`
1667:     function _autoClaimEarnings(address _delegator) internal {

```
[#L207](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L207) [#L232](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L232) [#L241](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L241) [#L302](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L302) [#L394](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L394) [#L485](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L485) [#L537](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L537) [#L640](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L640) [#L679](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L679) [#L745](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L745) [#L796](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L796) [#L818](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L818) [#L842](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L842) [#L908](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L908) [#L923](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L923) [#L937](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L937) [#L946](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L946) [#L956](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L956) [#L987](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L987) [#L1027](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1027) [#L1058](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1058) [#L1089](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1089) [#L1128](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1128) [#L1145](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1145) [#L1156](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1156) [#L1167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1167) [#L1259](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1259) [#L1294](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1294) [#L1307](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1307) [#L1352](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1352) [#L1392](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1392) [#L1437](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1437) [#L1459](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1459) [#L1500](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1500) [#L1564](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1564) [#L1591](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1591) [#L1667](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1667) 

```solidity
File: contracts/bonding/BondingVotes.sol

// Missing zero check for `_account`
155:     function getVotes(address _account) external view returns (uint256) {

// Missing zero check for `_account`
167:     function getPastVotes(address _account, uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

// Missing zero check for `_account`
205:     function delegates(address _account) external view returns (address) {

// Missing zero check for `_account`
218:     function delegatedAt(address _account, uint256 _round) external view onlyPastRounds(_round) returns (address) {

// Missing zero check for ``
226:     function delegate(address) external pure {

// Missing zero check for ``
233:     function delegateBySig(
             address,
             uint256,
             uint256,
             uint8,
             bytes32,
             bytes32
         ) external pure {

// Missing zero check for `_account`
// Missing zero check for `_delegateAddress`
258:     function checkpointBondingState(
             address _account,
             uint256 _startRound,
             uint256 _bondedAmount,
             address _delegateAddress,
             uint256 _delegatedAmount,
             uint256 _lastClaimRound,
             uint256 _lastRewardRound
         ) external virtual onlyBondingManager {

// Missing zero check for `_account`
315:     function hasCheckpoint(address _account) public view returns (bool) {

// Missing zero check for `_account`
361:     function getBondingStateAt(address _account, uint256 _round)
             public
             view
             virtual
             returns (uint256 amount, address delegateAddress)
         {

// Missing zero check for `_account`
387:     function onBondingCheckpointChanged(
             address _account,
             BondingCheckpoint memory previous,
             BondingCheckpoint memory current
         ) internal {

// Missing zero check for `_account`
422:     function getBondingCheckpointAt(address _account, uint256 _round)
             internal
             view
             returns (BondingCheckpoint storage)
         {

// Missing zero check for `_transcoder`
499:     function getLastTranscoderRewardsEarningsPool(address _transcoder, uint256 _round)
             internal
             view
             returns (uint256 rewardRound, EarningsPool.Data memory pool)
         {

// Missing zero check for `_transcoder`
520:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)
             internal
             view
             returns (EarningsPool.Data memory pool)
         {

```
[#L155](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L155) [#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L167) [#L205](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L205) [#L218](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L218) [#L226](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L226) [#L233](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L233) [#L258](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L258) [#L315](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L315) [#L361](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L361) [#L387](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L387) [#L422](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L422) [#L499](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L499) [#L520](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L520) 

```solidity
File: contracts/bonding/IBondingManager.sol

// Missing zero check for `_transcoder`
59:     function updateTranscoderWithFees(

// Missing zero check for `_transcoder`
// Missing zero check for `_finder`
65:     function slashTranscoder(

// Missing zero check for `_transcoder`
77:     function transcoderTotalStake(address _transcoder) external view returns (uint256);

// Missing zero check for `_transcoder`
79:     function isActiveTranscoder(address _transcoder) external view returns (bool);

// Missing zero check for `_transcoder`
85:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)

```
[#L59](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L59) [#L65](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L65) [#L77](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L77) [#L79](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L79) [#L85](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L85) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

// Missing zero check for `_account`
83:     function hasVoted(uint256 _proposalId, address _account) public view virtual override returns (bool) {

// Missing zero check for `_account`
130:     function _countVote(
             uint256 _proposalId,
             address _account,
             uint8 _supportInt,
             uint256 _weight,
             bytes memory // params
         ) internal virtual override {

// Missing zero check for `_account`
174:     function _handleVoteOverrides(
             uint256 _proposalId,
             ProposalTally storage _tally,
             ProposalVoterState storage _voter,
             address _account,
             uint256 _weight
         ) internal returns (uint256) {

```
[#L83](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L83) [#L130](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L130) [#L174](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L174) 

```solidity
File: contracts/treasury/IVotes.sol

// Missing zero check for `account`
9:     function delegatedAt(address account, uint256 timepoint) external returns (address);

```
[#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L9) 

```solidity
File: contracts/treasury/Treasury.sol

// Missing zero check for `admin`
16:     function initialize(
            uint256 minDelay,
            address[] memory proposers,
            address[] memory executors,
            address admin
        ) external initializer {

```
[#L16](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L16) 

</details>

---

<a name="NC-8"></a> 
#### [NC-8] Consider moving `msg.sender` checks to `modifier`s
If some functions are only allowed to be called by some specific users, consider using a modifier instead of checking with a require statement, especially if this check is done in multiple functions.

<details>
<summary>
There are <b>9</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

253:         require(isValidUnbondingLock(msg.sender, _unbondingLockId), "invalid unbonding lock ID");

494:         require(isRegisteredTranscoder(msg.sender), "transcoder must be registered");

750:         require(delegatorStatus(msg.sender) == DelegatorStatus.Bonded, "caller must be bonded");

801:         require(delegatorStatus(msg.sender) != DelegatorStatus.Unbonded, "caller must be bonded");

824:         require(delegatorStatus(msg.sender) == DelegatorStatus.Unbonded, "caller must be unbonded");

850:         require(isActiveTranscoder(msg.sender), "caller must be an active transcoder");

1652:         require(msg.sender == controller.getContract(keccak256("TicketBroker")), "caller must be TicketBroker");

1656:         require(msg.sender == controller.getContract(keccak256("RoundsManager")), "caller must be RoundsManager");

1660:         require(msg.sender == controller.getContract(keccak256("Verifier")), "caller must be Verifier");

```
[#L253](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L253) [#L494](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L494) [#L750](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L750) [#L801](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L801) [#L824](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L824) [#L850](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L850) [#L1652](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1652) [#L1656](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1656) [#L1660](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1660) 

</details>

---

<a name="NC-9"></a> 
#### [NC-9] NatSpec documentation for contract is missing
e.g. `@dev` or `@notice`, and it must appear above the contract definition braces in order to be identified by the compiler as NatSpec.

<details>
<summary>
There are <b>3</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/IBondingManager.sol

8: interface IBondingManager {

```
[#L8](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L8) 

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

9: library EarningsPoolLIP36 {

```
[#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L9) 

```solidity
File: contracts/treasury/IVotes.sol

6: interface IVotes is IERC5805Upgradeable {

```
[#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L6) 

</details>

---

<a name="NC-10"></a> 
#### [NC-10] Event declarations should have NatSpec descriptions

<details>
<summary>
There are <b>13</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/IBondingManager.sol

9:     event TranscoderUpdate(address indexed transcoder, uint256 rewardCut, uint256 feeShare);

10:     event TranscoderActivated(address indexed transcoder, uint256 activationRound);

11:     event TranscoderDeactivated(address indexed transcoder, uint256 deactivationRound);

12:     event TranscoderSlashed(address indexed transcoder, address finder, uint256 penalty, uint256 finderReward);

13:     event Reward(address indexed transcoder, uint256 amount);

14:     event TreasuryReward(address indexed transcoder, address treasury, uint256 amount);

15:     event Bond(

22:     event Unbond(

29:     event Rebond(address indexed delegate, address indexed delegator, uint256 unbondingLockId, uint256 amount);

30:     event TransferBond(

37:     event WithdrawStake(address indexed delegator, uint256 unbondingLockId, uint256 amount, uint256 withdrawRound);

38:     event WithdrawFees(address indexed delegator, address recipient, uint256 amount);

39:     event EarningsClaimed(

```
[#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L9) [#L10](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L10) [#L11](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L11) [#L12](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L12) [#L13](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L13) [#L14](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L14) [#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L15) [#L22](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L22) [#L29](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L29) [#L30](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L30) [#L37](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L37) [#L38](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L38) [#L39](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L39) 

</details>

---

<a name="NC-11"></a> 
#### [NC-11] NatSpec documentation for function is missing
It is recommended that Solidity contracts are fully annotated using NatSpec for all public interfaces (everything in the ABI). It is clearly stated in the Solidity official documentation. In complex projects such as DeFi, the interpretation of all functions and their arguments and returns is important for code readability and auditability.

<details>
<summary>
There are <b>31</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

1643:     function treasury() internal view returns (address) {

1647:     function bondingVotes() internal view returns (IBondingVotes) {

1651:     function _onlyTicketBroker() internal view {

1655:     function _onlyRoundsManager() internal view {

1659:     function _onlyVerifier() internal view {

1663:     function _currentRoundInitialized() internal view {

1667:     function _autoClaimEarnings(address _delegator) internal {

```
[#L1643](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1643) [#L1647](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1647) [#L1651](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1651) [#L1655](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1655) [#L1659](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1659) [#L1663](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1663) [#L1667](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1667) 

```solidity
File: contracts/bonding/IBondingManager.sol

59:     function updateTranscoderWithFees(

65:     function slashTranscoder(

72:     function setCurrentRoundTotalActiveStake() external;

75:     function getTranscoderPoolSize() external view returns (uint256);

77:     function transcoderTotalStake(address _transcoder) external view returns (uint256);

79:     function isActiveTranscoder(address _transcoder) external view returns (bool);

81:     function getTotalBonded() external view returns (uint256);

83:     function nextRoundTotalActiveStake() external view returns (uint256);

85:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)

```
[#L59](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L59) [#L65](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L65) [#L72](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L72) [#L75](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L75) [#L77](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L77) [#L79](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L79) [#L81](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L81) [#L83](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L83) [#L85](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L85) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

68:     function __GovernorCountingOverridable_init_unchained(uint256 _quota) internal onlyInitializing {

```
[#L64](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L64) [#L68](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L68) 

```solidity
File: contracts/treasury/IVotes.sol

7:     function totalSupply() external view returns (uint256);

9:     function delegatedAt(address account, uint256 timepoint) external returns (address);

13:     function name() external view returns (string memory);

15:     function symbol() external view returns (string memory);

17:     function decimals() external view returns (uint8);

```
[#L7](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L7) [#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L9) [#L13](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L13) [#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L15) [#L17](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L17) 

```solidity
File: contracts/treasury/LivepeerGovernor.sol

54:     function initialize(
            uint256 initialVotingDelay,
            uint256 initialVotingPeriod,
            uint256 initialProposalThreshold,
            uint256 initialQuorum,
            uint256 quota
        ) public initializer {

114:     function proposalThreshold()
             public
             view
             override(GovernorUpgradeable, GovernorSettingsUpgradeable)
             returns (uint256)
         {

123:     function state(uint256 proposalId)
             public
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (ProposalState)
         {

132:     function _execute(
             uint256 proposalId,
             address[] memory targets,
             uint256[] memory values,
             bytes[] memory calldatas,
             bytes32 descriptionHash
         ) internal override(GovernorUpgradeable, GovernorTimelockControlUpgradeable) {

142:     function _cancel(
             address[] memory targets,
             uint256[] memory values,
             bytes[] memory calldatas,
             bytes32 descriptionHash
         ) internal override(GovernorUpgradeable, GovernorTimelockControlUpgradeable) returns (uint256) {

151:     function _executor()
             internal
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (address)
         {

160:     function supportsInterface(bytes4 interfaceId)
             public
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (bool)
         {

```
[#L54](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L54) [#L114](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L114) [#L123](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L123) [#L132](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L132) [#L142](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L142) [#L151](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L151) [#L160](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L160) 

```solidity
File: contracts/treasury/Treasury.sol

16:     function initialize(
            uint256 minDelay,
            address[] memory proposers,
            address[] memory executors,
            address admin
        ) external initializer {

```
[#L16](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L16) 

</details>

---

<a name="NC-12"></a> 
#### [NC-12] Missing NatSpec `@param`
Some functions have an incomplete NatSpec: add a `@param` notation to describe the function parameters to improve the code documentation.

<details>
<summary>
There are <b>38</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

// Missing @param for _recipient
// Missing @param for _amount
273:     function withdrawFees(address payable _recipient, uint256 _amount)
             external
             whenSystemNotPaused
             currentRoundInitialized
             autoClaimEarnings(msg.sender)
         {

// Missing @param for _round
302:     function updateTranscoderWithFees(
             address _transcoder,
             uint256 _fees,
             uint256 _round
         ) external whenSystemNotPaused onlyTicketBroker {

// Missing @param for _cutRate
1176:     function _setTreasuryRewardCutRate(uint256 _cutRate) internal {

// Missing @param for _newPosPrev
// Missing @param for _newPosNext
1294:     function increaseTotalStake(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegate) {

// Missing @param for _delegate
// Missing @param for _amount
// Missing @param for _newPosPrev
// Missing @param for _newPosNext
1307:     function increaseTotalStakeUncheckpointed(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal {

// Missing @param for _newPosPrev
// Missing @param for _newPosNext
1352:     function decreaseTotalStake(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegate) {

// Missing @param for _newPosPrev
// Missing @param for _newPosNext
1392:     function tryToJoinActiveSet(
              address _transcoder,
              uint256 _totalStake,
              uint256 _activationRound,
              address _newPosPrev,
              address _newPosNext
          ) internal {

// Missing @param for _transcoder
1437:     function resignTranscoder(address _transcoder) internal {

// Missing @param for _owner
// Missing @param for _delegator
// Missing @param for _transcoder
1591:     function _checkpointBondingState(
              address _owner,
              Delegator storage _delegator,
              Transcoder storage _transcoder
          ) internal {

// Missing @param for _delegator
1667:     function _autoClaimEarnings(address _delegator) internal {

```
[#L273](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L273) [#L302](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L302) [#L1176](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1176) [#L1294](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1294) [#L1307](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1307) [#L1352](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1352) [#L1392](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1392) [#L1437](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1437) [#L1591](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1591) [#L1667](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1667) 

```solidity
File: contracts/bonding/BondingVotes.sol

// Missing @param for _account
155:     function getVotes(address _account) external view returns (uint256) {

// Missing @param for _account
// Missing @param for _round
167:     function getPastVotes(address _account, uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

// Missing @param for _round
194:     function getPastTotalSupply(uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

// Missing @param for _account
205:     function delegates(address _account) external view returns (address) {

// Missing @param for _account
// Missing @param for _round
218:     function delegatedAt(address _account, uint256 _round) external view onlyPastRounds(_round) returns (address) {

// Missing @param for _account
315:     function hasCheckpoint(address _account) public view returns (bool) {

// Missing @param for _account
// Missing @param for previous
// Missing @param for current
387:     function onBondingCheckpointChanged(
             address _account,
             BondingCheckpoint memory previous,
             BondingCheckpoint memory current
         ) internal {

// Missing @param for _transcoder
// Missing @param for _round
520:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)
             internal
             view
             returns (EarningsPool.Data memory pool)
         {

```
[#L155](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L155) [#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L167) [#L194](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L194) [#L205](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L205) [#L218](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L218) [#L315](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L315) [#L387](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L387) [#L520](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L520) 

```solidity
File: contracts/bonding/IBondingManager.sol

// Missing @param for _transcoder
// Missing @param for _fees
// Missing @param for _round
59:     function updateTranscoderWithFees(

// Missing @param for _transcoder
// Missing @param for _finder
// Missing @param for _slashAmount
// Missing @param for _finderFee
65:     function slashTranscoder(

// Missing @param for _transcoder
77:     function transcoderTotalStake(address _transcoder) external view returns (uint256);

// Missing @param for _transcoder
79:     function isActiveTranscoder(address _transcoder) external view returns (bool);

// Missing @param for _transcoder
// Missing @param for _round
85:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)

```
[#L59](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L59) [#L65](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L65) [#L77](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L77) [#L79](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L79) [#L85](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L85) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

// Missing @param for _quota
64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

// Missing @param for _quota
68:     function __GovernorCountingOverridable_init_unchained(uint256 _quota) internal onlyInitializing {

// Missing @param for _proposalId
// Missing @param for _account
83:     function hasVoted(uint256 _proposalId, address _account) public view virtual override returns (bool) {

// Missing @param for _proposalId
90:     function proposalVotes(uint256 _proposalId)
            public
            view
            virtual
            returns (
                uint256 againstVotes,
                uint256 forVotes,
                uint256 abstainVotes
            )
        {

// Missing @param for _proposalId
107:     function _quorumReached(uint256 _proposalId) internal view virtual override returns (bool) {

// Missing @param for _proposalId
118:     function _voteSucceeded(uint256 _proposalId) internal view virtual override returns (bool) {

// Missing @param for _proposalId
// Missing @param for _account
// Missing @param for _supportInt
// Missing @param for _weight
130:     function _countVote(
             uint256 _proposalId,
             address _account,
             uint8 _supportInt,
             uint256 _weight,
             bytes memory // params
         ) internal virtual override {

```
[#L64](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L64) [#L68](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L68) [#L83](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L83) [#L90](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L90) [#L107](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L107) [#L118](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L118) [#L130](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L130) 

```solidity
File: contracts/treasury/IVotes.sol

// Missing @param for account
// Missing @param for timepoint
9:     function delegatedAt(address account, uint256 timepoint) external returns (address);

```
[#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L9) 

```solidity
File: contracts/treasury/LivepeerGovernor.sol

// Missing @param for _controller
43:     constructor(address _controller) Manager(_controller) {

// Missing @param for initialVotingDelay
// Missing @param for initialVotingPeriod
// Missing @param for initialProposalThreshold
// Missing @param for initialQuorum
// Missing @param for quota
54:     function initialize(
            uint256 initialVotingDelay,
            uint256 initialVotingPeriod,
            uint256 initialProposalThreshold,
            uint256 initialQuorum,
            uint256 quota
        ) public initializer {

// Missing @param for proposalId
123:     function state(uint256 proposalId)
             public
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (ProposalState)
         {

// Missing @param for proposalId
// Missing @param for targets
// Missing @param for values
// Missing @param for calldatas
// Missing @param for descriptionHash
132:     function _execute(
             uint256 proposalId,
             address[] memory targets,
             uint256[] memory values,
             bytes[] memory calldatas,
             bytes32 descriptionHash
         ) internal override(GovernorUpgradeable, GovernorTimelockControlUpgradeable) {

// Missing @param for targets
// Missing @param for values
// Missing @param for calldatas
// Missing @param for descriptionHash
142:     function _cancel(
             address[] memory targets,
             uint256[] memory values,
             bytes[] memory calldatas,
             bytes32 descriptionHash
         ) internal override(GovernorUpgradeable, GovernorTimelockControlUpgradeable) returns (uint256) {

// Missing @param for interfaceId
160:     function supportsInterface(bytes4 interfaceId)
             public
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (bool)
         {

```
[#L43](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L43) [#L54](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L54) [#L123](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L123) [#L132](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L132) [#L142](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L142) [#L160](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L160) 

```solidity
File: contracts/treasury/Treasury.sol

// Missing @param for minDelay
// Missing @param for proposers
// Missing @param for executors
// Missing @param for admin
16:     function initialize(
            uint256 minDelay,
            address[] memory proposers,
            address[] memory executors,
            address admin
        ) external initializer {

```
[#L16](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L16) 

</details>

---

<a name="NC-13"></a> 
#### [NC-13] Public variable declarations should have NatSpec descriptions

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

35:     uint64 public unbondingPeriod;

88:     uint256 public currentRoundTotalActiveStake;

90:     uint256 public nextRoundTotalActiveStake;

98:     uint256 public treasuryRewardCutRate;

100:     uint256 public nextRoundTreasuryRewardCutRate;

103:     uint256 public treasuryBalanceCeiling;

```
[#L35](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L35) [#L88](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L88) [#L90](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L90) [#L98](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L98) [#L100](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L100) [#L103](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L103) 

</details>

---

<a name="NC-14"></a> 
#### [NC-14] NatSpec `@return` is missing
It is recommended that Solidity contracts are fully annotated using NatSpec

<details>
<summary>
There are <b>46</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

1189:     function cumulativeFactorsPool(Transcoder storage _transcoder, uint256 _round)
              internal
              view
              returns (EarningsPool.Data memory pool)
          {

1643:     function treasury() internal view returns (address) {

1647:     function bondingVotes() internal view returns (IBondingVotes) {

```
[#L1189](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1189) [#L1643](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1643) [#L1647](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1647) 

```solidity
File: contracts/bonding/BondingVotes.sol

115:     function name() external pure returns (string memory) {

122:     function symbol() external pure returns (string memory) {

129:     function decimals() external pure returns (uint8) {

137:     function clock() public view returns (uint48) {

145:     function CLOCK_MODE() external pure returns (string memory) {

155:     function getVotes(address _account) external view returns (uint256) {

167:     function getPastVotes(address _account, uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

181:     function totalSupply() external view returns (uint256) {

194:     function getPastTotalSupply(uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

205:     function delegates(address _account) external view returns (address) {

218:     function delegatedAt(address _account, uint256 _round) external view onlyPastRounds(_round) returns (address) {

315:     function hasCheckpoint(address _account) public view returns (bool) {

325:     function getTotalActiveStakeAt(uint256 _round) public view virtual returns (uint256) {

520:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)
             internal
             view
             returns (EarningsPool.Data memory pool)
         {

539:     function bondingManager() internal view returns (IBondingManager) {

546:     function roundsManager() internal view returns (IRoundsManager) {

```
[#L115](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L115) [#L122](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L122) [#L129](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L129) [#L137](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L137) [#L145](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L145) [#L155](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L155) [#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L167) [#L181](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L181) [#L194](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L194) [#L205](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L205) [#L218](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L218) [#L315](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L315) [#L325](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L325) [#L520](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L520) [#L539](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L539) [#L546](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L546) 

```solidity
File: contracts/bonding/IBondingManager.sol

75:     function getTranscoderPoolSize() external view returns (uint256);

77:     function transcoderTotalStake(address _transcoder) external view returns (uint256);

79:     function isActiveTranscoder(address _transcoder) external view returns (bool);

81:     function getTotalBonded() external view returns (uint256);

83:     function nextRoundTotalActiveStake() external view returns (uint256);

85:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)

```
[#L75](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L75) [#L77](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L77) [#L79](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L79) [#L81](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L81) [#L83](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L83) [#L85](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L85) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

76:     function COUNTING_MODE() public pure virtual override returns (string memory) {

83:     function hasVoted(uint256 _proposalId, address _account) public view virtual override returns (bool) {

90:     function proposalVotes(uint256 _proposalId)
            public
            view
            virtual
            returns (
                uint256 againstVotes,
                uint256 forVotes,
                uint256 abstainVotes
            )
        {

107:     function _quorumReached(uint256 _proposalId) internal view virtual override returns (bool) {

118:     function _voteSucceeded(uint256 _proposalId) internal view virtual override returns (bool) {

174:     function _handleVoteOverrides(
             uint256 _proposalId,
             ProposalTally storage _tally,
             ProposalVoterState storage _voter,
             address _account,
             uint256 _weight
         ) internal returns (uint256) {

217:     function votes() public view virtual returns (IVotes);

```
[#L76](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L76) [#L83](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L83) [#L90](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L90) [#L107](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L107) [#L118](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L118) [#L174](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L174) [#L217](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L217) 

```solidity
File: contracts/treasury/IVotes.sol

7:     function totalSupply() external view returns (uint256);

9:     function delegatedAt(address account, uint256 timepoint) external returns (address);

13:     function name() external view returns (string memory);

15:     function symbol() external view returns (string memory);

17:     function decimals() external view returns (uint8);

```
[#L7](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L7) [#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L9) [#L13](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L13) [#L15](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L15) [#L17](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L17) 

```solidity
File: contracts/treasury/LivepeerGovernor.sol

78:     function quorumDenominator() public view virtual override returns (uint256) {

85:     function votes() public view override returns (IVotes) {

101:     function bondingVotes() internal view returns (IVotes) {

108:     function treasury() internal view returns (Treasury) {

114:     function proposalThreshold()
             public
             view
             override(GovernorUpgradeable, GovernorSettingsUpgradeable)
             returns (uint256)
         {

123:     function state(uint256 proposalId)
             public
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (ProposalState)
         {

142:     function _cancel(
             address[] memory targets,
             uint256[] memory values,
             bytes[] memory calldatas,
             bytes32 descriptionHash
         ) internal override(GovernorUpgradeable, GovernorTimelockControlUpgradeable) returns (uint256) {

151:     function _executor()
             internal
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (address)
         {

160:     function supportsInterface(bytes4 interfaceId)
             public
             view
             override(GovernorUpgradeable, GovernorTimelockControlUpgradeable)
             returns (bool)
         {

```
[#L78](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L78) [#L85](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L85) [#L101](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L101) [#L108](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L108) [#L114](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L114) [#L123](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L123) [#L142](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L142) [#L151](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L151) [#L160](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L160) 

</details>

---

<a name="NC-15"></a> 
#### [NC-15] Redundant inheritance specifier
The contracts below already extend the specified contract, so there is no need to list it in the inheritance list again.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/treasury/LivepeerGovernor.sol

// No need for LivepeerGovernor to inherit from Initializable, GovernorCountingOverridable is already inherited from Initializable
// No need for LivepeerGovernor to inherit from GovernorUpgradeable, GovernorCountingOverridable is already inherited from GovernorUpgradeable
26: contract LivepeerGovernor is
        ManagerProxyTarget,
        Initializable,
        GovernorUpgradeable,
        GovernorSettingsUpgradeable,
        GovernorTimelockControlUpgradeable,
        GovernorVotesUpgradeable,
        GovernorVotesQuorumFractionUpgradeable,
        GovernorCountingOverridable

```
[#L26](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L26) 

</details>

---

<a name="NC-16"></a> 
#### [NC-16] Contract declarations should have NatSpec `@title` annotations
Some contract definitions have an incomplete NatSpec: add a `@title` notation to describe the contract to improve the code documentation.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

9: library EarningsPoolLIP36 {

```
[#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L9) 

```solidity
File: contracts/treasury/IVotes.sol

6: interface IVotes is IERC5805Upgradeable {

```
[#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol#L6) 

</details>

---

<a name="NC-17"></a> 
#### [NC-17] Lines are too long
The [solidity style guide](https://docs.soliditylang.org/en/v0.8.17/style-guide.html#maximum-line-length) recommends a maximum line length of 120 characters. Lines of code that are longer than 120 should be wrapped.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

47:         uint256 cumulativeRewards; // The transcoder's cumulative rewards (earned via the its active staked rewards and its reward cut).

48:         uint256 cumulativeFees; // The transcoder's cumulative fees (earned via the its active staked rewards and its fee share)

```
[#L47](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L47) [#L48](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L48) 

</details>

---

<a name="NC-18"></a> 
#### [NC-18] Unused contract variables
The following state variables are defined but not used. It is recommended to check the code for logical omissions that cause them not to be used. If it's determined that they are not needed anywhere, it's best to remove them from the codebase to improve code clarity and minimize confusion.

<details>
<summary>
There are <b>7</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

1: // SPDX-License-Identifier: MIT

1: // SPDX-License-Identifier: MIT

1: // SPDX-License-Identifier: MIT

```
[#L1](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1) [#L1](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1) [#L1](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1) 

```solidity
File: contracts/bonding/BondingVotes.sol

1: // SPDX-License-Identifier: MIT

1: // SPDX-License-Identifier: MIT

```
[#L1](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L1) [#L1](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L1) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

1: // SPDX-License-Identifier: MIT

224:     uint256[48] private __gap;

```
[#L1](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L1) [#L224](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L224) 

</details>

---

<a name="NC-19"></a> 
#### [NC-19] Consider using `delete` rather than assigning zero to clear values
The `delete` keyword more closely matches the semantics of what is being done, and draws more attention to the changing of state, which may lead to a more thorough audit of its associated logic.

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

771:             del.delegateAddress = address(0);

773:             del.startRound = 0;

1535:                 t.cumulativeFees = 0;

1536:                 t.cumulativeRewards = 0;

```
[#L771](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L771) [#L773](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L773) [#L1535](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1535) [#L1536](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1536) 

```solidity
File: contracts/bonding/BondingVotes.sol

373:             amount = 0;

```
[#L373](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L373) 

</details>

---

<a name="NC-20"></a> 
#### [NC-20] Expressions for constant values should use `immutable` rather than `constant`
While it doesn't save any gas because the compiler knows that developers often make this mistake, it's still best to use the right tool for the task at hand. There is a difference between `constant` variables and `immutable` variables, and they should each be used in their appropriate contexts. `constants` should be used for literal values written into the code, and `immutable` variables should be used for expressions, or values calculated in, or passed into the constructor.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

32:     uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

```
[#L32](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L32) 

</details>

---

<a name="NC-21"></a> 
#### [NC-21] Use `@inheritdoc` for overridden functions

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

76:     function COUNTING_MODE() public pure virtual override returns (string memory) {

83:     function hasVoted(uint256 _proposalId, address _account) public view virtual override returns (bool) {

107:     function _quorumReached(uint256 _proposalId) internal view virtual override returns (bool) {

118:     function _voteSucceeded(uint256 _proposalId) internal view virtual override returns (bool) {

```
[#L76](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L76) [#L83](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L83) [#L107](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L107) [#L118](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L118) 

```solidity
File: contracts/treasury/LivepeerGovernor.sol

78:     function quorumDenominator() public view virtual override returns (uint256) {

85:     function votes() public view override returns (IVotes) {

```
[#L78](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L78) [#L85](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L85) 

</details>

---

<a name="NC-22"></a> 
#### [NC-22] Visibility of state variables is not explicitly defined
To avoid misunderstandings and unexpected state accesses, it is recommended to explicitly define the visibility of each state variable.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

32:     uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

```
[#L32](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L32) 

</details>

---

<a name="NC-23"></a> 
#### [NC-23] Whitespace in Expressions
See the [Whitespace in Expressions](https://docs.soliditylang.org/en/latest/style-guide.html#whitespace-in-expressions) section of the Solidity Style Guide.

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

913:         (uint256 stake, ) = pendingStakeAndFees(_delegator, endRound);

```
[#L913](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L913) 

```solidity
File: contracts/bonding/BondingVotes.sol

156:         (uint256 amount, ) = getBondingStateAt(_account, clock() + 1);

168:         (uint256 amount, ) = getBondingStateAt(_account, _round + 1);

480:         (uint256 stakeWithRewards, ) = EarningsPoolLIP36.delegatorCumulativeStakeAndFees(

```
[#L156](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L156) [#L168](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L168) [#L480](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L480) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

119:         (uint256 againstVotes, uint256 forVotes, ) = proposalVotes(_proposalId);

```
[#L119](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L119) 

</details>

---

<a name="NC-24"></a> 
#### [NC-24] Common functions should be refactored to a common base contract
The functions below have the same implementation as is seen in other files. The functions should be refactored into functions of a common base contract.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

// Seen in contracts/bonding/BondingVotes.sol
1639:     function roundsManager() internal view returns (IRoundsManager) {

```
[#L1639](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1639) 

```solidity
File: contracts/bonding/BondingVotes.sol

// Seen in contracts/bonding/BondingManager.sol
546:     function roundsManager() internal view returns (IRoundsManager) {

```
[#L546](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L546) 

</details>

---

<a name="NC-25"></a> 
#### [NC-25] Names of `private`/`internal` functions should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>32</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

1189:     function cumulativeFactorsPool(Transcoder storage _transcoder, uint256 _round)
              internal
              view
              returns (EarningsPool.Data memory pool)
          {

1206:     function latestCumulativeFactorsPool(Transcoder storage _transcoder, uint256 _round)
              internal
              view
              returns (EarningsPool.Data memory pool)
          {

1238:     function delegatorCumulativeStakeAndFees(
              Transcoder storage _transcoder,
              uint256 _startRound,
              uint256 _endRound,
              uint256 _stake,
              uint256 _fees
          ) internal view returns (uint256 cStake, uint256 cFees) {

1259:     function pendingStakeAndFees(address _delegator, uint256 _endRound)
              internal
              view
              returns (uint256 stake, uint256 fees)
          {

1294:     function increaseTotalStake(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegate) {

1307:     function increaseTotalStakeUncheckpointed(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal {

1352:     function decreaseTotalStake(
              address _delegate,
              uint256 _amount,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegate) {

1392:     function tryToJoinActiveSet(
              address _transcoder,
              uint256 _totalStake,
              uint256 _activationRound,
              address _newPosPrev,
              address _newPosNext
          ) internal {

1437:     function resignTranscoder(address _transcoder) internal {

1459:     function updateTranscoderWithRewards(
              address _transcoder,
              uint256 _rewards,
              uint256 _round,
              address _newPosPrev,
              address _newPosNext
          ) internal {

1500:     function updateDelegatorWithEarnings(
              address _delegator,
              uint256 _endRound,
              uint256 _lastClaimRound
          ) internal {

1564:     function processRebond(
              address _delegator,
              uint256 _unbondingLockId,
              address _newPosPrev,
              address _newPosNext
          ) internal autoCheckpoint(_delegator) {

1615:     function livepeerToken() internal view returns (ILivepeerToken) {

1623:     function minter() internal view returns (IMinter) {

1631:     function l2Migrator() internal view returns (address) {

1639:     function roundsManager() internal view returns (IRoundsManager) {

1643:     function treasury() internal view returns (address) {

1647:     function bondingVotes() internal view returns (IBondingVotes) {

```
[#L1189](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1189) [#L1206](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1206) [#L1238](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1238) [#L1259](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1259) [#L1294](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1294) [#L1307](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1307) [#L1352](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1352) [#L1392](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1392) [#L1437](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1437) [#L1459](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1459) [#L1500](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1500) [#L1564](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1564) [#L1615](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1615) [#L1623](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1623) [#L1631](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1631) [#L1639](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1639) [#L1643](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1643) [#L1647](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1647) 

```solidity
File: contracts/bonding/BondingVotes.sol

387:     function onBondingCheckpointChanged(
             address _account,
             BondingCheckpoint memory previous,
             BondingCheckpoint memory current
         ) internal {

422:     function getBondingCheckpointAt(address _account, uint256 _round)
             internal
             view
             returns (BondingCheckpoint storage)
         {

459:     function delegatorCumulativeStakeAt(BondingCheckpoint storage bond, uint256 _round)
             internal
             view
             returns (uint256)
         {

499:     function getLastTranscoderRewardsEarningsPool(address _transcoder, uint256 _round)
             internal
             view
             returns (uint256 rewardRound, EarningsPool.Data memory pool)
         {

520:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)
             internal
             view
             returns (EarningsPool.Data memory pool)
         {

539:     function bondingManager() internal view returns (IBondingManager) {

546:     function roundsManager() internal view returns (IRoundsManager) {

```
[#L387](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L387) [#L422](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L422) [#L459](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L459) [#L499](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L499) [#L520](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L520) [#L539](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L539) [#L546](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L546) 

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

18:     function updateCumulativeFeeFactor(
            EarningsPool.Data storage earningsPool,
            EarningsPool.Data memory _prevEarningsPool,
            uint256 _fees
        ) internal {

47:     function updateCumulativeRewardFactor(
            EarningsPool.Data storage earningsPool,
            EarningsPool.Data memory _prevEarningsPool,
            uint256 _rewards
        ) internal {

71:     function delegatorCumulativeStakeAndFees(
            EarningsPool.Data memory _startPool,
            EarningsPool.Data memory _endPool,
            uint256 _stake,
            uint256 _fees
        ) internal pure returns (uint256 cStake, uint256 cFees) {

```
[#L18](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L18) [#L47](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L47) [#L71](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L71) 

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

28:     function findLowerBound(uint256[] storage _array, uint256 _val) internal view returns (uint256) {

64:     function pushSorted(uint256[] storage array, uint256 val) internal {

```
[#L28](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L28) [#L64](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L64) 

```solidity
File: contracts/treasury/LivepeerGovernor.sol

101:     function bondingVotes() internal view returns (IVotes) {

108:     function treasury() internal view returns (Treasury) {

```
[#L101](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L101) [#L108](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L108) 

</details>

---

<a name="NC-26"></a> 
#### [NC-26] Names of `private`/`internal` state variables should be prefixed with an underscore
It is recommended by the [Solidity Style Guide](https://docs.soliditylang.org/en/v0.8.20/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

<details>
<summary>
There are <b>6</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

84:     mapping(address => Delegator) private delegators;

85:     mapping(address => Transcoder) private transcoders;

95:     SortedDoublyLL.Data private transcoderPool;

```
[#L84](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L84) [#L85](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L85) [#L95](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L95) 

```solidity
File: contracts/bonding/BondingVotes.sol

78:     mapping(address => BondingCheckpointsByRound) private bondingCheckpoints;

82:     TotalActiveStakeByRound private totalStakeCheckpoints;

96:         uint256 currentRound = clock();

```
[#L78](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L78) [#L82](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L82) [#L96](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L96) 

</details>

---

<a name="NC-27"></a> 
#### [NC-27] Variables should be named in mixedCase style
As the [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html#naming-styles) suggests: arguments, local variables and mutable state variables should be named in mixedCase style.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

224:     uint256[48] private __gap;

```
[#L224](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L224) 

</details>

---

<a name="NC-28"></a> 
#### [NC-28] `TODO`s left in the code
TODOs may signal that a feature is missing or not ready for audit, consider resolving the issue and removing the TODO comment.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/IBondingManager.sol

6:  * TODO: switch to interface type

```
[#L6](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L6) 

</details>

---

<a name="NC-29"></a> 
#### [NC-29] Event is missing `indexed` fields
Index event fields make the field more quickly accessible to off-chain tools that parse events. However, note that each index field costs extra gas during emission, so it's not necessarily best to index the maximum allowed per event (three fields). Each event should use three indexed fields if there are three or more fields, and gas usage is not particularly of concern for the events in question. If there are fewer than three fields, all of the fields should be indexed.

<details>
<summary>
There are <b>12</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/IBondingManager.sol

9:     event TranscoderUpdate(address indexed transcoder, uint256 rewardCut, uint256 feeShare);

10:     event TranscoderActivated(address indexed transcoder, uint256 activationRound);

11:     event TranscoderDeactivated(address indexed transcoder, uint256 deactivationRound);

12:     event TranscoderSlashed(address indexed transcoder, address finder, uint256 penalty, uint256 finderReward);

13:     event Reward(address indexed transcoder, uint256 amount);

14:     event TreasuryReward(address indexed transcoder, address treasury, uint256 amount);

22:     event Unbond(

29:     event Rebond(address indexed delegate, address indexed delegator, uint256 unbondingLockId, uint256 amount);

30:     event TransferBond(

37:     event WithdrawStake(address indexed delegator, uint256 unbondingLockId, uint256 amount, uint256 withdrawRound);

38:     event WithdrawFees(address indexed delegator, address recipient, uint256 amount);

39:     event EarningsClaimed(

```
[#L9](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L9) [#L10](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L10) [#L11](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L11) [#L12](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L12) [#L13](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L13) [#L14](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L14) [#L22](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L22) [#L29](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L29) [#L30](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L30) [#L37](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L37) [#L38](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L38) [#L39](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol#L39) 

</details>

---

<a name="NC-30"></a> 
#### [NC-30] Functions not used internally could be marked external

<details>
<summary>
There are <b>17</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

679:     function transferBond(

908:     function pendingStake(address _delegator, uint256 _endRound) public view returns (uint256) {

923:     function pendingFees(address _delegator, uint256 _endRound) public view returns (uint256) {

946:     function transcoderStatus(address _transcoder) public view returns (TranscoderStatus) {

987:     function getTranscoder(address _transcoder)

1027:     function getTranscoderEarningsPoolForRound(address _transcoder, uint256 _round)

1058:     function getDelegator(address _delegator)

1089:     function getDelegatorUnbondingLock(address _delegator, uint256 _unbondingLockId)

1103:     function getTranscoderPoolMaxSize() public view returns (uint256) {

1111:     function getTranscoderPoolSize() public view returns (uint256) {

1119:     function getFirstTranscoderInPool() public view returns (address) {

1128:     function getNextTranscoderInPool(address _transcoder) public view returns (address) {

1136:     function getTotalBonded() public view returns (uint256) {

```
[#L679](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L679) [#L908](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L908) [#L923](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L923) [#L946](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L946) [#L987](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L987) [#L1027](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1027) [#L1058](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1058) [#L1089](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1089) [#L1103](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1103) [#L1111](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1111) [#L1119](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1119) [#L1128](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1128) [#L1136](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1136) 

```solidity
File: contracts/treasury/LivepeerGovernor.sol

54:     function initialize(

114:     function proposalThreshold()

123:     function state(uint256 proposalId)

160:     function supportsInterface(bytes4 interfaceId)

```
[#L54](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L54) [#L114](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L114) [#L123](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L123) [#L160](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol#L160) 

</details>

---


## Gas Optimizations

<a name="GAS-1"></a> 
#### [GAS-1] Use `calldata` instead of `memory` for function arguments that do not get mutated
Mark data types as `calldata` instead of `memory` where possible. This makes it so that the data is not automatically loaded into memory. If the data passed into the function does not need to be changed (like updating values in an array), it can be passed in as `calldata`. The one exception to this is if the argument must later be passed into another function that takes an argument that specifies `memory` storage.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/Treasury.sol

18:         address[] memory proposers,

19:         address[] memory executors,

```
[#L18](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L18) [#L19](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol#L19) 

</details>

---

<a name="GAS-2"></a> 
#### [GAS-2] Use Custom Errors
[Source](https://blog.soliditylang.org/2021/04/21/custom-errors/)
Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

<details>
<summary>
There are <b>25</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

253:         require(isValidUnbondingLock(msg.sender, _unbondingLockId), "invalid unbonding lock ID");

279:         require(_recipient != address(0), "invalid recipient");

281:         require(fees >= _amount, "insufficient fees to withdraw");

310:         require(isRegisteredTranscoder(_transcoder), "transcoder must be registered");

491:         require(!roundsManager().currentRoundLocked(), "can't update transcoder params, current round is locked");

492:         require(MathUtils.validPerc(_rewardCut), "invalid rewardCut percentage");

493:         require(MathUtils.validPerc(_feeShare), "invalid feeShare percentage");

494:         require(isRegisteredTranscoder(msg.sender), "transcoder must be registered");

563:                 require(_to != _owner, "INVALID_DELEGATE");

565:                 require(currentDelegate == _to, "INVALID_DELEGATE_CHANGE");

582:             require(!isRegisteredTranscoder(_owner), "registered transcoders can't delegate towards other addresses");

606:         require(delegationAmount > 0, "delegation amount must be greater than 0");

722:             require(oldDelDelegate != _delegator, "INVALID_DELEGATOR");

750:         require(delegatorStatus(msg.sender) == DelegatorStatus.Bonded, "caller must be bonded");

754:         require(_amount > 0, "unbond amount must be greater than 0");

755:         require(_amount <= del.bondedAmount, "amount is greater than bonded amount");

801:         require(delegatorStatus(msg.sender) != DelegatorStatus.Unbonded, "caller must be bonded");

824:         require(delegatorStatus(msg.sender) == DelegatorStatus.Unbonded, "caller must be unbonded");

850:         require(isActiveTranscoder(msg.sender), "caller must be an active transcoder");

1177:         require(PreciseMathUtils.validPerc(_cutRate), "_cutRate is invalid precise percentage");

1573:         require(isValidUnbondingLock(_delegator, _unbondingLockId), "invalid unbonding lock ID");

1652:         require(msg.sender == controller.getContract(keccak256("TicketBroker")), "caller must be TicketBroker");

1656:         require(msg.sender == controller.getContract(keccak256("RoundsManager")), "caller must be RoundsManager");

1660:         require(msg.sender == controller.getContract(keccak256("Verifier")), "caller must be Verifier");

1664:         require(roundsManager().currentRoundInitialized(), "current round is not initialized");

```
[#L253](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L253) [#L279](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L279) [#L281](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L281) [#L310](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L310) [#L491](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L491) [#L492](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L492) [#L493](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L493) [#L494](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L494) [#L563](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L563) [#L565](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L565) [#L582](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L582) [#L606](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L606) [#L722](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L722) [#L750](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L750) [#L754](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L754) [#L755](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L755) [#L801](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L801) [#L824](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L824) [#L850](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L850) [#L1177](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1177) [#L1573](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1573) [#L1652](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1652) [#L1656](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1656) [#L1660](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1660) [#L1664](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1664) 

</details>

---

<a name="GAS-3"></a> 
#### [GAS-3] Don't use `SafeMath` once the solidity version is 0.8.0 or greater
Solidity 0.8.0 introduces internal overflow checks, so using SafeMath is redundant and adds overhead.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

17: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[#L17](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L17) 

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[#L7](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L7) 

</details>

---

<a name="GAS-4"></a> 
#### [GAS-4] Long revert strings

<details>
<summary>
There are <b>10</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

491:         require(!roundsManager().currentRoundLocked(), "can't update transcoder params, current round is locked");

582:             require(!isRegisteredTranscoder(_owner), "registered transcoders can't delegate towards other addresses");

606:         require(delegationAmount > 0, "delegation amount must be greater than 0");

754:         require(_amount > 0, "unbond amount must be greater than 0");

755:         require(_amount <= del.bondedAmount, "amount is greater than bonded amount");

850:         require(isActiveTranscoder(msg.sender), "caller must be an active transcoder");

1177:         require(PreciseMathUtils.validPerc(_cutRate), "_cutRate is invalid precise percentage");

1652:         require(msg.sender == controller.getContract(keccak256("TicketBroker")), "caller must be TicketBroker");

1656:         require(msg.sender == controller.getContract(keccak256("RoundsManager")), "caller must be RoundsManager");

1660:         require(msg.sender == controller.getContract(keccak256("Verifier")), "caller must be Verifier");

```
[#L491](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L491) [#L582](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L582) [#L606](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L606) [#L754](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L754) [#L755](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L755) [#L850](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L850) [#L1177](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1177) [#L1652](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1652) [#L1656](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1656) [#L1660](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1660) 

</details>

---

<a name="GAS-5"></a> 
#### [GAS-5] Functions guaranteed to revert when called by normal users can be marked `payable`
If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function. Marking the function as `payable` will lower the gas cost for legitimate callers because the compiler will not include checks for whether a payment was provided.

<details>
<summary>
There are <b>15</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

155:     function setUnbondingPeriod(uint64 _unbondingPeriod) external onlyControllerOwner {

167:     function setTreasuryRewardCutRate(uint256 _cutRate) external onlyControllerOwner {

176:     function setTreasuryBalanceCeiling(uint256 _ceiling) external onlyControllerOwner {

186:     function setNumActiveTranscoders(uint256 _numActiveTranscoders) external onlyControllerOwner {

462:     function setCurrentRoundTotalActiveStake() external onlyRoundsManager {

1651:     function _onlyTicketBroker() internal view {

1655:     function _onlyRoundsManager() internal view {

1659:     function _onlyVerifier() internal view {

```
[#L155](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L155) [#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L167) [#L176](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L176) [#L186](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L186) [#L462](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L462) [#L1651](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1651) [#L1655](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1655) [#L1659](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1659) 

```solidity
File: contracts/bonding/BondingVotes.sol

167:     function getPastVotes(address _account, uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

194:     function getPastTotalSupply(uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

218:     function delegatedAt(address _account, uint256 _round) external view onlyPastRounds(_round) returns (address) {

303:     function checkpointTotalActiveStake(uint256 _totalStake, uint256 _round) external virtual onlyBondingManager {

553:     function _onlyBondingManager() internal view {

```
[#L167](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L167) [#L194](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L194) [#L218](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L218) [#L303](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L303) [#L553](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L553) 

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

68:     function __GovernorCountingOverridable_init_unchained(uint256 _quota) internal onlyInitializing {

```
[#L64](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L64) [#L68](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol#L68) 

</details>

---

<a name="GAS-6"></a> 
#### [GAS-6] Use != 0 instead of > 0 for unsigned integer comparison

<details>
<summary>
There are <b>14</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

402:         if (del.bondedAmount > 0) {

576:         } else if (currentBondedAmount > 0 && currentDelegate != _to) {

606:         require(delegationAmount > 0, "delegation amount must be greater than 0");

614:         if (_amount > 0) {

754:         require(_amount > 0, "unbond amount must be greater than 0");

871:         if (treasuryBalanceCeiling > 0) {

873:             if (treasuryBalance >= treasuryBalanceCeiling && nextRoundTreasuryRewardCutRate > 0) {

884:         if (treasuryRewards > 0) {

1158:         return d.delegateAddress == _transcoder && d.bondedAmount > 0;

1169:         return delegators[_delegator].unbondingLocks[_unbondingLockId].withdrawRound > 0;

```
[#L402](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L402) [#L576](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L576) [#L606](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L606) [#L614](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L614) [#L754](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L754) [#L871](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L871) [#L873](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L873) [#L884](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L884) [#L1158](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1158) [#L1169](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1169) 

```solidity
File: contracts/bonding/BondingVotes.sol

316:         return bondingCheckpoints[_account].startRounds.length > 0;

331:         if (exactCheckpoint > 0) {

436:         if (bond.bondedAmount > 0) {

507:         if (rewardRound > 0) {

```
[#L316](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L316) [#L331](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L331) [#L436](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L436) [#L507](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L507) 

</details>

---

<a name="GAS-7"></a> 
#### [GAS-7] Using assembly to check for zero can save gas
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

<details>
<summary>
There are <b>26</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

279:         require(_recipient != address(0), "invalid recipient");

343:         if (prevEarningsPool.cumulativeRewardFactor == 0 && lastRewardRound == currentRound) {

424:             if (_finder != address(0)) {

595:             if (currPool.cumulativeRewardFactor == 0) {

599:             if (currPool.cumulativeFeeFactor == 0) {

719:         if (newDel.delegateAddress == address(0) && newDel.bondedAmount == 0) {

719:         if (newDel.delegateAddress == address(0) && newDel.bondedAmount == 0) {

769:         if (del.bondedAmount == 0) {

959:         if (del.bondedAmount == 0) {

1215:         if (pool.cumulativeRewardFactor == 0 && lastRewardRound < _round) {

1221:         if (pool.cumulativeFeeFactor == 0 && lastFeeRound < _round) {

1512:         if (del.delegateAddress != address(0)) {

1520:             if (endEarningsPool.cumulativeRewardFactor == 0) {

1527:             if (endEarningsPool.cumulativeFeeFactor == 0) {

```
[#L279](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L279) [#L343](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L343) [#L424](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L424) [#L595](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L595) [#L599](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L599) [#L719](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L719) [#L719](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L719) [#L769](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L769) [#L959](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L959) [#L1215](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1215) [#L1221](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1221) [#L1512](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1512) [#L1520](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1520) [#L1527](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol#L1527) 

```solidity
File: contracts/bonding/BondingVotes.sol

98:             revert FutureLookup(_round, currentRound == 0 ? 0 : currentRound - 1);

337:         if (upper == 0) {

372:         if (bond.bondedAmount == 0) {

510:             if (pool.cumulativeRewardFactor == 0) {

```
[#L98](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L98) [#L337](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L337) [#L372](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L372) [#L510](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol#L510) 

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

24:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

29:         if (earningsPool.cumulativeFeeFactor == 0) {

52:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

78:         if (_startPool.cumulativeRewardFactor == 0) {

83:         if (_endPool.cumulativeRewardFactor == 0) {

```
[#L24](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L24) [#L29](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L29) [#L52](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L52) [#L78](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L78) [#L83](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L83) 

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

30:         if (len == 0) {

49:         if (upperIdx == 0) {

65:         if (array.length == 0) {

```
[#L30](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L30) [#L49](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L49) [#L65](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L65) 

</details>

---

<a name="GAS-8"></a> 
#### [GAS-8] `internal` functions not called by the contract should be removed
If the functions are required by an interface, the contract should inherit from that interface and use the `override` keyword

<details>
<summary>
There are <b>5</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

18:     function updateCumulativeFeeFactor(

47:     function updateCumulativeRewardFactor(

71:     function delegatorCumulativeStakeAndFees(

```
[#L18](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L18) [#L47](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L47) [#L71](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol#L71) 

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

28:     function findLowerBound(uint256[] storage _array, uint256 _val) internal view returns (uint256) {

64:     function pushSorted(uint256[] storage array, uint256 val) internal {

```
[#L28](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L28) [#L64](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol#L64) 

</details>

---

