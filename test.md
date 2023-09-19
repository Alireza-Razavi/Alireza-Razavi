# Report


## Gas Optimizations


| |Issue|Instances|
|-|:-|:-:|
| [GAS-1](#GAS-1) | Use calldata instead of memory for function arguments that do not get mutated | 2 |
| [GAS-2](#GAS-2) | Use Custom Errors | 25 |
| [GAS-3](#GAS-3) | Don't use `SafeMath` once the solidity version is 0.8.0 or greater | 2 |
| [GAS-4](#GAS-4) | Long revert strings | 10 |
| [GAS-5](#GAS-5) | Functions guaranteed to revert when called by normal users can be marked `payable` | 15 |
| [GAS-6](#GAS-6) | Use != 0 instead of > 0 for unsigned integer comparison | 14 |
| [GAS-7](#GAS-7) | Using assembly to check for zero can save gas | 26 |
| [GAS-8](#GAS-8) | `internal` functions not called by the contract should be removed | 5 |


## Non Critical Issues


| |Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Custom errors has no error details | 1 |
| [NC-2](#NC-2) | Import declarations should import specific identifiers, rather than the whole file | 52 |
| [NC-3](#NC-3) | Consider moving `msg.sender` checks to `modifier`s | 9 |
| [NC-4](#NC-4) | Visibility of state variables is not explicitly defined | 299 |
| [NC-5](#NC-5) | Event is missing `indexed` fields | 12 |
| [NC-6](#NC-6) | Functions not used internally could be marked external | 17 |


## Low Issues


| |Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Governance functions should be controlled by time locks | 4 |
| [L-2](#L-2) | Missing storage gap for upgradable contracts | 2 |
| [L-3](#L-3) | Solidity version 0.8.20 or above may not work on other chains due to PUSH0 | 1 |
| [L-4](#L-4) | Using zero as a parameter | 40 |
| [L-5](#L-5) | Zero address check in initializer | 4 |
| [L-6](#L-6) | Empty Function Body - Consider commenting why | 2 |
| [L-7](#L-7) | Initializers could be front-run | 2 |
| [L-8](#L-8) | Functions calling contracts/addresses with transfer hooks should be protected by reentrancy guard | 1 |
| [L-9](#L-9) | Unsafe ERC20 operation(s) | 1 |
| [L-10](#L-10) | Upgradable contracts need a constructor to lock the implementation contract when it is deployed | 2 |


## Medium Issues


| |Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | Centralization Risk for trusted owners | 11 |



## Gas Optimizations


<a name="GAS-1"></a> 
#### [GAS-1] Use calldata instead of memory for function arguments that do not get mutated
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

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```


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

```solidity
File: contracts/bonding/BondingVotes.sol

167:     function getPastVotes(address _account, uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

194:     function getPastTotalSupply(uint256 _round) external view onlyPastRounds(_round) returns (uint256) {

218:     function delegatedAt(address _account, uint256 _round) external view onlyPastRounds(_round) returns (address) {

303:     function checkpointTotalActiveStake(uint256 _totalStake, uint256 _round) external virtual onlyBondingManager {

553:     function _onlyBondingManager() internal view {

```

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

68:     function __GovernorCountingOverridable_init_unchained(uint256 _quota) internal onlyInitializing {

```


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

```solidity
File: contracts/bonding/BondingVotes.sol

316:         return bondingCheckpoints[_account].startRounds.length > 0;

331:         if (exactCheckpoint > 0) {

436:         if (bond.bondedAmount > 0) {

507:         if (rewardRound > 0) {

```


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

```solidity
File: contracts/bonding/BondingVotes.sol

98:             revert FutureLookup(_round, currentRound == 0 ? 0 : currentRound - 1);

337:         if (upper == 0) {

372:         if (bond.bondedAmount == 0) {

510:             if (pool.cumulativeRewardFactor == 0) {

```

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

24:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

29:         if (earningsPool.cumulativeFeeFactor == 0) {

52:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

78:         if (_startPool.cumulativeRewardFactor == 0) {

83:         if (_endPool.cumulativeRewardFactor == 0) {

```

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

30:         if (len == 0) {

49:         if (upperIdx == 0) {

65:         if (array.length == 0) {

```


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

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

28:     function findLowerBound(uint256[] storage _array, uint256 _val) internal view returns (uint256) {

64:     function pushSorted(uint256[] storage array, uint256 val) internal {

```


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

```solidity
File: contracts/bonding/IBondingVotes.sol

4: import "../treasury/IVotes.sol";

```

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

4: import "./EarningsPool.sol";

5: import "../../libraries/PreciseMathUtils.sol";

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

4: import "../../libraries/MathUtils.sol";

6: import "@openzeppelin/contracts/utils/Arrays.sol";

```

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

```solidity
File: contracts/treasury/IVotes.sol

4: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

```

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

```solidity
File: contracts/treasury/Treasury.sol

4: import "@openzeppelin/contracts-upgradeable/governance/TimelockControllerUpgradeable.sol";

```


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


</details>

---

<a name="NC-4"></a> 
#### [NC-4] Visibility of state variables is not explicitly defined
To avoid misunderstandings and unexpected state accesses, it is recommended to explicitly define the visibility of each state variable.

<details>

<summary>
There are <b>299</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

32:     uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

39:         uint256 lastRewardRound; // Last round that the transcoder called reward

40:         uint256 rewardCut; // % of reward paid to transcoder by a delegator

41:         uint256 feeShare; // % of fees paid to delegators by transcoder

43:         uint256 lastActiveStakeUpdateRound; // Round for which the stake was last updated while the transcoder is active

44:         uint256 activationRound; // Round in which the transcoder became active - 0 if inactive

45:         uint256 deactivationRound; // Round in which the transcoder will become inactive

46:         uint256 activeCumulativeRewards; // The transcoder's cumulative rewards that are active in the current round

47:         uint256 cumulativeRewards; // The transcoder's cumulative rewards (earned via the its active staked rewards and its reward cut).

48:         uint256 cumulativeFees; // The transcoder's cumulative fees (earned via the its active staked rewards and its fee share)

49:         uint256 lastFeeRound; // Latest round in which the transcoder received fees

60:         uint256 bondedAmount; // The amount of bonded tokens

61:         uint256 fees; // The amount of fees collected

62:         address delegateAddress; // The address delegated to

63:         uint256 delegatedAmount; // The amount of tokens delegated to the delegator

64:         uint256 startRound; // The round the delegator transitions to bonded phase and is delegated to someone

65:         uint256 lastClaimRound; // The last round during which the delegator claimed its earnings

66:         uint256 nextUnbondingLockId; // ID for the next unbonding lock created

79:         uint256 amount; // Amount of tokens being unbonded

80:         uint256 withdrawRound; // Round at which unbonding period is over and tokens can be withdrawn

259:         uint256 amount = lock.amount;

260:         uint256 withdrawRound = lock.withdrawRound;

280:         uint256 fees = delegators[msg.sender].fees;

303:         address _transcoder,

304:         uint256 _fees,

305:         uint256 _round

312:         uint256 currentRound = roundsManager().currentRound();

316:         uint256 lastRewardRound = t.lastRewardRound;

317:         uint256 activeCumulativeRewards = t.activeCumulativeRewards;

330:             uint256 lastUpdateRound = t.lastActiveStakeUpdateRound;

342:         uint256 totalStake = earningsPool.totalStake;

348:             uint256 rewards = PreciseMathUtils.percOf(

355:             uint256 treasuryRewards = MathUtils.percOf(rewards, treasuryRewardCutRate);

358:             uint256 transcoderCommissionRewards = MathUtils.percOf(rewards, earningsPool.transcoderRewardCut);

359:             uint256 delegatorsRewards = rewards.sub(transcoderCommissionRewards);

368:         uint256 delegatorsFees = MathUtils.percOf(_fees, earningsPool.transcoderFeeShare);

369:         uint256 transcoderCommissionFees = _fees.sub(delegatorsFees);

371:         uint256 transcoderRewardStakeFees = PreciseMathUtils.percOf(

395:         address _transcoder,

396:         address _finder,

397:         uint256 _slashAmount,

398:         uint256 _finderFee

403:             uint256 penalty = MathUtils.percOf(delegators[_transcoder].bondedAmount, _slashAmount);

421:             uint256 burnAmount = penalty;

425:                 uint256 finderAmount = MathUtils.percOf(penalty, _finderFee);

486:         uint256 _rewardCut,

487:         uint256 _feeShare,

488:         address _newPosPrev,

489:         address _newPosNext

497:         uint256 currentRound = roundsManager().currentRound();

538:         uint256 _amount,

539:         address _owner,

540:         address _to,

541:         address _oldDelegateNewPosPrev,

542:         address _oldDelegateNewPosNext,

543:         address _currDelegateNewPosPrev,

544:         address _currDelegateNewPosNext

550:         uint256 currentRound = roundsManager().currentRound();

552:         uint256 delegationAmount = _amount;

554:         address currentDelegate = del.delegateAddress;

556:         uint256 currentBondedAmount = del.bondedAmount;

641:         uint256 _amount,

642:         address _to,

643:         address _oldDelegateNewPosPrev,

644:         address _oldDelegateNewPosNext,

645:         address _currDelegateNewPosPrev,

646:         address _currDelegateNewPosNext

680:         address _delegator,

681:         uint256 _amount,

682:         address _oldDelegateNewPosPrev,

683:         address _oldDelegateNewPosNext,

684:         address _newDelegateNewPosPrev,

685:         address _newDelegateNewPosNext

693:         address oldDelDelegate = oldDel.delegateAddress;

697:         uint256 oldDelUnbondingLockId = oldDel.nextUnbondingLockId.sub(1);

698:         uint256 withdrawRound = oldDel.unbondingLocks[oldDelUnbondingLockId].withdrawRound;

704:         uint256 newDelUnbondingLockId = newDel.nextUnbondingLockId;

712:         uint256 currentRound = roundsManager().currentRound();

713:         uint256 lastClaimRound = newDel.lastClaimRound;

746:         uint256 _amount,

747:         address _newPosPrev,

748:         address _newPosNext

757:         address currentDelegate = del.delegateAddress;

758:         uint256 currentRound = roundsManager().currentRound();

759:         uint256 withdrawRound = currentRound.add(unbondingPeriod);

760:         uint256 unbondingLockId = del.nextUnbondingLockId;

797:         uint256 _unbondingLockId,

798:         address _newPosPrev,

799:         address _newPosNext

819:         address _to,

820:         uint256 _unbondingLockId,

821:         address _newPosPrev,

822:         address _newPosNext

848:         uint256 currentRound = roundsManager().currentRound();

866:         uint256 lastUpdateRound = t.lastActiveStakeUpdateRound;

872:             uint256 treasuryBalance = livepeerToken().balanceOf(treasury());

882:         uint256 totalRewardTokens = mtr.createReward(earningsPool.totalStake, currentRoundTotalActiveStake);

883:         uint256 treasuryRewards = PreciseMathUtils.percOf(totalRewardTokens, treasuryRewardCutRate);

885:             address trsry = treasury();

892:         uint256 transcoderRewards = totalRewardTokens.sub(treasuryRewards);

912:         uint256 endRound = roundsManager().currentRound();

927:         uint256 endRound = roundsManager().currentRound();

991:             uint256 lastRewardRound,

992:             uint256 rewardCut,

993:             uint256 feeShare,

994:             uint256 lastActiveStakeUpdateRound,

995:             uint256 activationRound,

996:             uint256 deactivationRound,

997:             uint256 activeCumulativeRewards,

998:             uint256 cumulativeRewards,

999:             uint256 cumulativeFees,

1000:             uint256 lastFeeRound

1031:             uint256 totalStake,

1032:             uint256 transcoderRewardCut,

1033:             uint256 transcoderFeeShare,

1034:             uint256 cumulativeRewardFactor,

1035:             uint256 cumulativeFeeFactor

1062:             uint256 bondedAmount,

1063:             uint256 fees,

1064:             address delegateAddress,

1065:             uint256 delegatedAmount,

1066:             uint256 startRound,

1067:             uint256 lastClaimRound,

1068:             uint256 nextUnbondingLockId

1147:         uint256 currentRound = roundsManager().currentRound();

1213:         uint256 lastRewardRound = _transcoder.lastRewardRound;

1219:         uint256 lastFeeRound = _transcoder.lastFeeRound;

1240:         uint256 _startRound,

1241:         uint256 _endRound,

1242:         uint256 _stake,

1243:         uint256 _fees

1270:         uint256 startRound = del.lastClaimRound.add(1);

1271:         address delegateAddr = del.delegateAddress;

1295:         address _delegate,

1296:         uint256 _amount,

1297:         address _newPosPrev,

1298:         address _newPosNext

1308:         address _delegate,

1309:         uint256 _amount,

1310:         address _newPosPrev,

1311:         address _newPosNext

1315:         uint256 currStake = transcoderTotalStake(_delegate);

1316:         uint256 newStake = currStake.add(_amount);

1319:             uint256 currRound = roundsManager().currentRound();

1320:             uint256 nextRound = currRound.add(1);

1353:         address _delegate,

1354:         uint256 _amount,

1355:         address _newPosPrev,

1356:         address _newPosNext

1360:         uint256 currStake = transcoderTotalStake(_delegate);

1361:         uint256 newStake = currStake.sub(_amount);

1364:             uint256 currRound = roundsManager().currentRound();

1365:             uint256 nextRound = currRound.add(1);

1393:         address _transcoder,

1394:         uint256 _totalStake,

1395:         uint256 _activationRound,

1396:         address _newPosPrev,

1397:         address _newPosNext

1399:         uint256 pendingNextRoundTotalActiveStake = nextRoundTotalActiveStake;

1402:             address lastTranscoder = transcoderPool.getLast();

1403:             uint256 lastStake = transcoderTotalStake(lastTranscoder);

1444:         uint256 deactivationRound = roundsManager().currentRound().add(1);

1460:         address _transcoder,

1461:         uint256 _rewards,

1462:         uint256 _round,

1463:         address _newPosPrev,

1464:         address _newPosNext

1472:         uint256 transcoderCommissionRewards = MathUtils.percOf(_rewards, earningsPool.transcoderRewardCut);

1473:         uint256 delegatorsRewards = _rewards.sub(transcoderCommissionRewards);

1475:         uint256 transcoderRewardStakeRewards = PreciseMathUtils.percOf(

1501:         address _delegator,

1502:         uint256 _endRound,

1503:         uint256 _lastClaimRound

1506:         uint256 startRound = _lastClaimRound.add(1);

1507:         uint256 currentBondedAmount = del.bondedAmount;

1508:         uint256 currentFees = del.fees;

1521:                 uint256 lastRewardRound = t.lastRewardRound;

1528:                 uint256 lastFeeRound = t.lastFeeRound;

1565:         address _delegator,

1566:         uint256 _unbondingLockId,

1567:         address _newPosPrev,

1568:         address _newPosNext

1575:         uint256 amount = lock.amount;

1592:         address _owner,

1599:         uint256 startRound = roundsManager().currentRound() + 1;

1668:         uint256 currentRound = roundsManager().currentRound();

1669:         uint256 lastClaimRound = delegators[_delegator].lastClaimRound;

```

```solidity
File: contracts/bonding/BondingVotes.sol

28:         uint256 bondedAmount;

32:         address delegateAddress;

37:         uint256 delegatedAmount;

42:         uint256 lastClaimRound;

51:         uint256 lastRewardRound;

60:         uint256[] startRounds;

71:         uint256[] rounds;

96:         uint256 currentRound = clock();

234:         address,

235:         uint256,

236:         uint256,

237:         uint8,

238:         bytes32,

239:         bytes32

259:         address _account,

260:         uint256 _startRound,

261:         uint256 _bondedAmount,

262:         address _delegateAddress,

263:         uint256 _delegatedAmount,

264:         uint256 _lastClaimRound,

265:         uint256 _lastRewardRound

330:         uint256 exactCheckpoint = totalStakeCheckpoints.data[_round];

335:         uint256[] storage initializedRounds = totalStakeCheckpoints.rounds;

336:         uint256 upper = initializedRounds.findUpperBound(_round);

343:             uint256 nextInitedRound = initializedRounds[upper];

388:         address _account,

392:         address previousDelegate = previous.delegateAddress;

393:         address newDelegate = current.delegateAddress;

401:         uint256 previousDelegateVotes = wasTranscoder ? previous.delegatedAmount : 0;

402:         uint256 currentDelegateVotes = isTranscoder ? current.delegatedAmount : 0;

440:         uint256 startRoundIdx = checkpoints.startRounds.findLowerBound(_round);

447:         uint256 startRound = checkpoints.startRounds[startRoundIdx];

```

```solidity
File: contracts/bonding/IBondingManager.sol

16:         address indexed newDelegate,

17:         address indexed oldDelegate,

18:         address indexed delegator,

19:         uint256 additionalAmount,

20:         uint256 bondedAmount

23:         address indexed delegate,

24:         address indexed delegator,

25:         uint256 unbondingLockId,

26:         uint256 amount,

27:         uint256 withdrawRound

31:         address indexed oldDelegator,

32:         address indexed newDelegator,

33:         uint256 oldUnbondingLockId,

34:         uint256 newUnbondingLockId,

35:         uint256 amount

40:         address indexed delegate,

41:         address indexed delegator,

42:         uint256 rewards,

43:         uint256 fees,

44:         uint256 startRound,

45:         uint256 endRound

60:         address _transcoder,

61:         uint256 _fees,

62:         uint256 _round

66:         address _transcoder,

67:         address _finder,

68:         uint256 _slashAmount,

69:         uint256 _finderFee

89:             uint256 totalStake,

90:             uint256 transcoderRewardCut,

91:             uint256 transcoderFeeShare,

92:             uint256 cumulativeRewardFactor,

93:             uint256 cumulativeFeeFactor

```

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

21:         uint256 _fees

23:         uint256 prevCumulativeFeeFactor = _prevEarningsPool.cumulativeFeeFactor;

24:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

50:         uint256 _rewards

52:         uint256 prevCumulativeRewardFactor = _prevEarningsPool.cumulativeRewardFactor != 0

74:         uint256 _stake,

75:         uint256 _fees

```

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

29:         uint256 len = _array.length;

38:         uint256 upperIdx = _array.findUpperBound(_val);

68:             uint256 last = array[array.length - 1];

```

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

42:         uint256 deductions;

49:         uint256 againstVotes;

50:         uint256 forVotes;

51:         uint256 abstainVotes;

95:             uint256 againstVotes,

96:             uint256 forVotes,

97:             uint256 abstainVotes

110:         uint256 totalVotes = againstVotes + forVotes + abstainVotes;

122:         uint256 opinionatedVotes = againstVotes + forVotes;

131:         uint256 _proposalId,

132:         address _account,

133:         uint8 _supportInt,

134:         uint256 _weight,

135:         bytes memory // params

175:         uint256 _proposalId,

178:         address _account,

179:         uint256 _weight

181:         uint256 timepoint = proposalSnapshot(_proposalId);

182:         address delegate = votes().delegatedAt(_account, timepoint);

```

```solidity
File: contracts/treasury/LivepeerGovernor.sol

55:         uint256 initialVotingDelay,

56:         uint256 initialVotingPeriod,

57:         uint256 initialProposalThreshold,

58:         uint256 initialQuorum,

59:         uint256 quota

133:         uint256 proposalId,

134:         address[] memory targets,

135:         uint256[] memory values,

136:         bytes[] memory calldatas,

137:         bytes32 descriptionHash

143:         address[] memory targets,

144:         uint256[] memory values,

145:         bytes[] memory calldatas,

146:         bytes32 descriptionHash

```

```solidity
File: contracts/treasury/Treasury.sol

17:         uint256 minDelay,

18:         address[] memory proposers,

19:         address[] memory executors,

20:         address admin

```


</details>

---

<a name="NC-5"></a> 
#### [NC-5] Event is missing `indexed` fields
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


</details>

---

<a name="NC-6"></a> 
#### [NC-6] Functions not used internally could be marked external

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

```solidity
File: contracts/treasury/LivepeerGovernor.sol

54:     function initialize(

114:     function proposalThreshold()

123:     function state(uint256 proposalId)

160:     function supportsInterface(bytes4 interfaceId)

```


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

```solidity
File: contracts/treasury/Treasury.sol

15: contract Treasury is Initializable, TimelockControllerUpgradeable {

```


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

```solidity
File: contracts/bonding/BondingVotes.sol

484:             0

```


</details>

---

<a name="L-5"></a> 
#### [L-5] Zero address check in initializer

<details>

<summary>
There are <b>4</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/Treasury.sol

16:     function initialize(

18:         address[] memory proposers,

19:         address[] memory executors,

20:         address admin

```


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

```solidity
File: contracts/bonding/BondingVotes.sol

107:     constructor(address _controller) Manager(_controller) {}

```


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

```solidity
File: contracts/treasury/Treasury.sol

16:     function initialize(

```


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

```solidity
File: contracts/treasury/Treasury.sol

15: contract Treasury is Initializable, TimelockControllerUpgradeable {

```


</details>

---


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

```solidity
File: contracts/bonding/BondingVotes.sol

266:     ) external virtual onlyBondingManager {

303:     function checkpointTotalActiveStake(uint256 _totalStake, uint256 _round) external virtual onlyBondingManager {

```

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

68:     function __GovernorCountingOverridable_init_unchained(uint256 _quota) internal onlyInitializing {

```


</details>

---
