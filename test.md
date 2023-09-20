# Report


## Medium Issues


Total <b>11</b> instances over <b>1</b> issue:

|ID|Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | Centralization Risk for trusted owners | 11 |

## Low Issues


Total <b>56</b> instances over <b>10</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Governance functions should be controlled by time locks | 4 |
| [L-2](#L-2) | Missing storage gap for upgradable contracts | 2 |
| [L-3](#L-3) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 1 |
| [L-4](#L-4) | Using zero as a parameter | 40 |
| [L-5](#L-5) | Zero address check in initializer | 1 |
| [L-6](#L-6) | Empty Function Body - Consider commenting why | 2 |
| [L-7](#L-7) | Initializers could be front-run | 2 |
| [L-8](#L-8) | Functions calling contracts/addresses with transfer hooks should be protected by reentrancy guard | 1 |
| [L-9](#L-9) | Unsafe ERC20 operation(s) | 1 |
| [L-10](#L-10) | Upgradable contracts need a constructor to lock the implementation contract when it is deployed | 2 |

## Non Critical Issues


Total <b>94</b> instances over <b>7</b> issues:

|ID|Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Custom errors has no error details | 1 |
| [NC-2](#NC-2) | Import declarations should import specific identifiers, rather than the whole file | 52 |
| [NC-3](#NC-3) | Consider moving `msg.sender` checks to `modifier`s | 9 |
| [NC-4](#NC-4) | Redundant inheritance specifier | 2 |
| [NC-5](#NC-5) | Visibility of state variables is not explicitly defined | 1 |
| [NC-6](#NC-6) | Event is missing `indexed` fields | 12 |
| [NC-7](#NC-7) | Functions not used internally could be marked external | 17 |

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
There are <b>11</b> instances (click to show):
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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/bonding/BondingVotes.sol

266:     ) external virtual onlyBondingManager {

303:     function checkpointTotalActiveStake(uint256 _totalStake, uint256 _round) external virtual onlyBondingManager {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol)

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

68:     function __GovernorCountingOverridable_init_unchained(uint256 _quota) internal onlyInitializing {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol)

```solidity
File: contracts/treasury/Treasury.sol

15: contract Treasury is Initializable, TimelockControllerUpgradeable {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingVotes.sol)

</details>

---

<a name="L-4"></a> 
#### [L-4] Using zero as a parameter
Taking `0` as a valid argument in Solidity without checks can lead to severe security issues. A historical example is the infamous `0x0` address bug where numerous tokens were lost. This happens because 0 can be interpreted as an uninitialized `address`, leading to transfers to the 0x0 address, effectively burning tokens. Moreover, `0` as a denominator in division operations would cause a runtime exception. It's also often indicative of a logical error in the caller's code. It's important to always validate input and handle edge cases like `0` appropriately. Use `require()` statements to enforce conditions and provide clear error messages to facilitate debugging and safer code.

<details>
<summary>
There are <b>40</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

199:         transcoderWithHint(_rewardCut, _feeShare, address(0), address(0));

199:         transcoderWithHint(_rewardCut, _feeShare, address(0), address(0));

199:         transcoderWithHint(_rewardCut, _feeShare, address(0), address(0));

199:         transcoderWithHint(_rewardCut, _feeShare, address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

208:         bondWithHint(_amount, _to, address(0), address(0), address(0), address(0));

216:         unbondWithHint(_amount, address(0), address(0));

216:         unbondWithHint(_amount, address(0), address(0));

216:         unbondWithHint(_amount, address(0), address(0));

216:         unbondWithHint(_amount, address(0), address(0));

224:         rebondWithHint(_unbondingLockId, address(0), address(0));

224:         rebondWithHint(_unbondingLockId, address(0), address(0));

224:         rebondWithHint(_unbondingLockId, address(0), address(0));

224:         rebondWithHint(_unbondingLockId, address(0), address(0));

233:         rebondFromUnbondedWithHint(_to, _unbondingLockId, address(0), address(0));

233:         rebondFromUnbondedWithHint(_to, _unbondingLockId, address(0), address(0));

233:         rebondFromUnbondedWithHint(_to, _unbondingLockId, address(0), address(0));

233:         rebondFromUnbondedWithHint(_to, _unbondingLockId, address(0), address(0));

279:         require(_recipient != address(0), "invalid recipient");

294:         rewardWithHint(address(0), address(0));

294:         rewardWithHint(address(0), address(0));

294:         rewardWithHint(address(0), address(0));

294:         rewardWithHint(address(0), address(0));

424:             if (_finder != address(0)) {

436:                 emit TranscoderSlashed(_transcoder, address(0), penalty, 0);

436:                 emit TranscoderSlashed(_transcoder, address(0), penalty, 0);

436:                 emit TranscoderSlashed(_transcoder, address(0), penalty, 0);

439:             emit TranscoderSlashed(_transcoder, _finder, 0, 0);

439:             emit TranscoderSlashed(_transcoder, _finder, 0, 0);

719:         if (newDel.delegateAddress == address(0) && newDel.bondedAmount == 0) {

771:             del.delegateAddress = address(0);

875:                 _setTreasuryRewardCutRate(0);

1512:         if (del.delegateAddress != address(0)) {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/bonding/BondingVotes.sol

484:             0

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol)

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

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/bonding/BondingVotes.sol

107:     constructor(address _controller) Manager(_controller) {}

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol)

```solidity
File: contracts/treasury/Treasury.sol

16:     function initialize(

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol)

```solidity
File: contracts/treasury/Treasury.sol

15: contract Treasury is Initializable, TimelockControllerUpgradeable {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol)

</details>

---


## Non Critical Issues

<a name="NC-1"></a> 
#### [NC-1] Custom errors has no error details
Consider adding parameters to the error to indicate which user or values caused the failure.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

23:     error VoteAlreadyCast();

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol)

</details>

---

<a name="NC-2"></a> 
#### [NC-2] Import declarations should import specific identifiers, rather than the whole file
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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol)

```solidity
File: contracts/bonding/IBondingVotes.sol

4: import "../treasury/IVotes.sol";

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingVotes.sol)

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

4: import "./EarningsPool.sol";

5: import "../../libraries/PreciseMathUtils.sol";

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol)

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

4: import "../../libraries/MathUtils.sol";

6: import "@openzeppelin/contracts/utils/Arrays.sol";

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol)

```solidity
File: contracts/treasury/IVotes.sol

4: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/IVotes.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol)

```solidity
File: contracts/treasury/Treasury.sol

4: import "@openzeppelin/contracts-upgradeable/governance/TimelockControllerUpgradeable.sol";

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol)

</details>

---

<a name="NC-3"></a> 
#### [NC-3] Consider moving `msg.sender` checks to `modifier`s
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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

</details>

---

<a name="NC-4"></a> 
#### [NC-4] Redundant inheritance specifier
The contracts below already extend the specified contract, so there is no need to list it in the inheritance list again.

<details>
<summary>
There are <b>2</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/LivepeerGovernor.sol

26: contract LivepeerGovernor is
        ManagerProxyTarget,
        Initializable,
        GovernorUpgradeable,
        GovernorSettingsUpgradeable,
        GovernorTimelockControlUpgradeable,
        GovernorVotesUpgradeable,
        GovernorVotesQuorumFractionUpgradeable,
        GovernorCountingOverridable

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol)

</details>

---

<a name="NC-5"></a> 
#### [NC-5] Visibility of state variables is not explicitly defined
To avoid misunderstandings and unexpected state accesses, it is recommended to explicitly define the visibility of each state variable.

<details>
<summary>
There is <b>1</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

32:     uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

</details>

---

<a name="NC-6"></a> 
#### [NC-6] Event is missing `indexed` fields
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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/IBondingManager.sol)

</details>

---

<a name="NC-7"></a> 
#### [NC-7] Functions not used internally could be marked external

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/treasury/LivepeerGovernor.sol

54:     function initialize(

114:     function proposalThreshold()

123:     function state(uint256 proposalId)

160:     function supportsInterface(bytes4 interfaceId)

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/LivepeerGovernor.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/Treasury.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/bonding/BondingVotes.sol

167:     function getPastVotes(address _account, uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

194:     function getPastTotalSupply(uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

218:     function delegatedAt(address _account, uint256 _round) external view onlyPastRounds(_round) returns (address) {

303:     function checkpointTotalActiveStake(uint256 _totalStake, uint256 _round) external virtual onlyBondingManager {

553:     function _onlyBondingManager() internal view {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol)

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

68:     function __GovernorCountingOverridable_init_unchained(uint256 _quota) internal onlyInitializing {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/treasury/GovernorCountingOverridable.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/bonding/BondingVotes.sol

316:         return bondingCheckpoints[_account].startRounds.length > 0;

331:         if (exactCheckpoint > 0) {

436:         if (bond.bondedAmount > 0) {

507:         if (rewardRound > 0) {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingManager.sol)

```solidity
File: contracts/bonding/BondingVotes.sol

98:             revert FutureLookup(_round, currentRound == 0 ? 0 : currentRound - 1);

337:         if (upper == 0) {

372:         if (bond.bondedAmount == 0) {

510:             if (pool.cumulativeRewardFactor == 0) {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/BondingVotes.sol)

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

24:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

29:         if (earningsPool.cumulativeFeeFactor == 0) {

52:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

78:         if (_startPool.cumulativeRewardFactor == 0) {

83:         if (_endPool.cumulativeRewardFactor == 0) {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol)

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

30:         if (len == 0) {

49:         if (upperIdx == 0) {

65:         if (array.length == 0) {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol)

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
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/EarningsPoolLIP36.sol)

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

28:     function findLowerBound(uint256[] storage _array, uint256 _val) internal view returns (uint256) {

64:     function pushSorted(uint256[] storage array, uint256 val) internal {

```
[Link to code](https://github.com/code-423n4/2023-08-livepeer/blob/bcf493b98d0ef835e969e637f25ea51ab77fabb6/contracts/bonding/libraries/SortedArrays.sol)

</details>

---

