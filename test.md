# Report


## Gas Optimizations


| |Issue|Instances|
|-|:-|:-:|
| [GAS-1](#GAS-1) | Use calldata instead of memory for function arguments that do not get mutated | 2 |
| [GAS-2](#GAS-2) | For Operations that will not overflow, you could use unchecked | 210 |
| [GAS-3](#GAS-3) | Use Custom Errors | 25 |
| [GAS-4](#GAS-4) | Don't use `SafeMath` once the solidity version is 0.8.0 or greater | 2 |
| [GAS-5](#GAS-5) | Long revert strings | 10 |
| [GAS-6](#GAS-6) | Functions guaranteed to revert when called by normal users can be marked `payable` | 15 |
| [GAS-7](#GAS-7) | Use != 0 instead of > 0 for unsigned integer comparison | 14 |
| [GAS-8](#GAS-8) | Using assembly to check for zero can save gas | 26 |
| [GAS-9](#GAS-9) | `internal` functions not called by the contract should be removed | 5 |


## Non Critical Issues


| |Issue|Instances|
|-|:-|:-:|
| [NC-1](#NC-1) | Event is missing `indexed` fields | 12 |
| [NC-2](#NC-2) | Functions not used internally could be marked external | 17 |


## Low Issues


| |Issue|Instances|
|-|:-|:-:|
| [L-1](#L-1) | Empty Function Body - Consider commenting why | 2 |
| [L-2](#L-2) | Initializers could be front-run | 12 |
| [L-3](#L-3) | Unsafe ERC20 operation(s) | 1 |


## Medium Issues


| |Issue|Instances|
|-|:-|:-:|
| [M-1](#M-1) | Centralization Risk for trusted owners | 11 |



## Gas Optimizations

<a name="GAS-1"></a> 
### [GAS-1] Use calldata instead of memory for function arguments that do not get mutated
Mark data types as `calldata` instead of `memory` where possible. This makes it so that the data is not automatically loaded into memory. If the data passed into the function does not need to be changed (like updating values in an array), it can be passed in as `calldata`. The one exception to this is if the argument must later be passed into another function that takes an argument that specifies `memory` storage.

<details>

<summary>
There are <b>(2)</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/Treasury.sol

18:         address[] memory proposers,

19:         address[] memory executors,

```

</details>

<a name="GAS-2"></a> 
### [GAS-2] For Operations that will not overflow, you could use unchecked

<details>

<summary>
There are <b>(210)</b> instances (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

4: import "../ManagerProxyTarget.sol";

5: import "./IBondingManager.sol";

6: import "../libraries/SortedDoublyLL.sol";

6: import "../libraries/SortedDoublyLL.sol";

7: import "../libraries/MathUtils.sol";

7: import "../libraries/MathUtils.sol";

8: import "../libraries/PreciseMathUtils.sol";

8: import "../libraries/PreciseMathUtils.sol";

9: import "./libraries/EarningsPool.sol";

9: import "./libraries/EarningsPool.sol";

10: import "./libraries/EarningsPoolLIP36.sol";

10: import "./libraries/EarningsPoolLIP36.sol";

11: import "../token/ILivepeerToken.sol";

11: import "../token/ILivepeerToken.sol";

12: import "../token/IMinter.sol";

12: import "../token/IMinter.sol";

13: import "../rounds/IRoundsManager.sol";

13: import "../rounds/IRoundsManager.sol";

14: import "../snapshots/IMerkleSnapshot.sol";

14: import "../snapshots/IMerkleSnapshot.sol";

15: import "./IBondingVotes.sol";

17: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

17: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

17: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

17: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

32:     uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

32:     uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

32:     uint256 constant MAX_FUTURE_ROUND = 2**256 - 1;

39:         uint256 lastRewardRound; // Last round that the transcoder called reward

39:         uint256 lastRewardRound; // Last round that the transcoder called reward

40:         uint256 rewardCut; // % of reward paid to transcoder by a delegator

40:         uint256 rewardCut; // % of reward paid to transcoder by a delegator

41:         uint256 feeShare; // % of fees paid to delegators by transcoder

41:         uint256 feeShare; // % of fees paid to delegators by transcoder

42:         mapping(uint256 => EarningsPool.Data) earningsPoolPerRound; // Mapping of round => earnings pool for the round

42:         mapping(uint256 => EarningsPool.Data) earningsPoolPerRound; // Mapping of round => earnings pool for the round

43:         uint256 lastActiveStakeUpdateRound; // Round for which the stake was last updated while the transcoder is active

43:         uint256 lastActiveStakeUpdateRound; // Round for which the stake was last updated while the transcoder is active

44:         uint256 activationRound; // Round in which the transcoder became active - 0 if inactive

44:         uint256 activationRound; // Round in which the transcoder became active - 0 if inactive

44:         uint256 activationRound; // Round in which the transcoder became active - 0 if inactive

45:         uint256 deactivationRound; // Round in which the transcoder will become inactive

45:         uint256 deactivationRound; // Round in which the transcoder will become inactive

46:         uint256 activeCumulativeRewards; // The transcoder's cumulative rewards that are active in the current round

46:         uint256 activeCumulativeRewards; // The transcoder's cumulative rewards that are active in the current round

47:         uint256 cumulativeRewards; // The transcoder's cumulative rewards (earned via the its active staked rewards and its reward cut).

47:         uint256 cumulativeRewards; // The transcoder's cumulative rewards (earned via the its active staked rewards and its reward cut).

48:         uint256 cumulativeFees; // The transcoder's cumulative fees (earned via the its active staked rewards and its fee share)

48:         uint256 cumulativeFees; // The transcoder's cumulative fees (earned via the its active staked rewards and its fee share)

49:         uint256 lastFeeRound; // Latest round in which the transcoder received fees

49:         uint256 lastFeeRound; // Latest round in which the transcoder received fees

60:         uint256 bondedAmount; // The amount of bonded tokens

60:         uint256 bondedAmount; // The amount of bonded tokens

61:         uint256 fees; // The amount of fees collected

61:         uint256 fees; // The amount of fees collected

62:         address delegateAddress; // The address delegated to

62:         address delegateAddress; // The address delegated to

63:         uint256 delegatedAmount; // The amount of tokens delegated to the delegator

63:         uint256 delegatedAmount; // The amount of tokens delegated to the delegator

64:         uint256 startRound; // The round the delegator transitions to bonded phase and is delegated to someone

64:         uint256 startRound; // The round the delegator transitions to bonded phase and is delegated to someone

65:         uint256 lastClaimRound; // The last round during which the delegator claimed its earnings

65:         uint256 lastClaimRound; // The last round during which the delegator claimed its earnings

66:         uint256 nextUnbondingLockId; // ID for the next unbonding lock created

66:         uint256 nextUnbondingLockId; // ID for the next unbonding lock created

67:         mapping(uint256 => UnbondingLock) unbondingLocks; // Mapping of unbonding lock ID => unbonding lock

67:         mapping(uint256 => UnbondingLock) unbondingLocks; // Mapping of unbonding lock ID => unbonding lock

79:         uint256 amount; // Amount of tokens being unbonded

79:         uint256 amount; // Amount of tokens being unbonded

80:         uint256 withdrawRound; // Round at which unbonding period is over and tokens can be withdrawn

80:         uint256 withdrawRound; // Round at which unbonding period is over and tokens can be withdrawn

1599:         uint256 startRound = roundsManager().currentRound() + 1;

```

```solidity
File: contracts/bonding/BondingVotes.sol

4: import "@openzeppelin/contracts/utils/Arrays.sol";

4: import "@openzeppelin/contracts/utils/Arrays.sol";

4: import "@openzeppelin/contracts/utils/Arrays.sol";

5: import "@openzeppelin/contracts/utils/math/SafeCast.sol";

5: import "@openzeppelin/contracts/utils/math/SafeCast.sol";

5: import "@openzeppelin/contracts/utils/math/SafeCast.sol";

5: import "@openzeppelin/contracts/utils/math/SafeCast.sol";

7: import "./libraries/EarningsPool.sol";

7: import "./libraries/EarningsPool.sol";

8: import "./libraries/EarningsPoolLIP36.sol";

8: import "./libraries/EarningsPoolLIP36.sol";

9: import "./libraries/SortedArrays.sol";

9: import "./libraries/SortedArrays.sol";

11: import "../ManagerProxyTarget.sol";

12: import "./IBondingVotes.sol";

13: import "./IBondingManager.sol";

14: import "../rounds/IRoundsManager.sol";

14: import "../rounds/IRoundsManager.sol";

98:             revert FutureLookup(_round, currentRound == 0 ? 0 : currentRound - 1);

156:         (uint256 amount, ) = getBondingStateAt(_account, clock() + 1);

168:         (uint256 amount, ) = getBondingStateAt(_account, _round + 1);

182:         return getTotalActiveStakeAt(clock() + 1);

195:         return getTotalActiveStakeAt(_round + 1);

206:         (, address delegateAddress) = getBondingStateAt(_account, clock() + 1);

219:         (, address delegateAddress) = getBondingStateAt(_account, _round + 1);

267:         if (_startRound != clock() + 1) {

268:             revert InvalidStartRound(_startRound, clock() + 1);

270:             revert FutureLastClaimRound(_lastClaimRound, _startRound - 1);

326:         if (_round > clock() + 1) {

327:             revert FutureLookup(_round, clock() + 1);

427:         if (_round > clock() + 1) {

428:             revert FutureLookup(_round, clock() + 1);

```

```solidity
File: contracts/bonding/IBondingVotes.sol

4: import "../treasury/IVotes.sol";

4: import "../treasury/IVotes.sol";

```

```solidity
File: contracts/bonding/libraries/EarningsPoolLIP36.sol

4: import "./EarningsPool.sol";

5: import "../../libraries/PreciseMathUtils.sol";

5: import "../../libraries/PreciseMathUtils.sol";

5: import "../../libraries/PreciseMathUtils.sol";

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

7: import "@openzeppelin/contracts/utils/math/SafeMath.sol";

```

```solidity
File: contracts/bonding/libraries/SortedArrays.sol

4: import "../../libraries/MathUtils.sol";

4: import "../../libraries/MathUtils.sol";

4: import "../../libraries/MathUtils.sol";

6: import "@openzeppelin/contracts/utils/Arrays.sol";

6: import "@openzeppelin/contracts/utils/Arrays.sol";

6: import "@openzeppelin/contracts/utils/Arrays.sol";

34:         if (_array[len - 1] <= _val) {

35:             return len - 1;

54:         return upperIdx - 1;

68:             uint256 last = array[array.length - 1];

```

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

8: import "../bonding/libraries/EarningsPool.sol";

8: import "../bonding/libraries/EarningsPool.sol";

8: import "../bonding/libraries/EarningsPool.sol";

9: import "../bonding/libraries/EarningsPoolLIP36.sol";

9: import "../bonding/libraries/EarningsPoolLIP36.sol";

9: import "../bonding/libraries/EarningsPoolLIP36.sol";

11: import "../Manager.sol";

12: import "../IController.sol";

13: import "../rounds/IRoundsManager.sol";

13: import "../rounds/IRoundsManager.sol";

14: import "./IVotes.sol";

110:         uint256 totalVotes = againstVotes + forVotes + abstainVotes;

110:         uint256 totalVotes = againstVotes + forVotes + abstainVotes;

122:         uint256 opinionatedVotes = againstVotes + forVotes;

135:         bytes memory // params

135:         bytes memory // params

154:             tally.againstVotes += _weight;

156:             tally.forVotes += _weight;

158:             tally.abstainVotes += _weight;

188:             return _weight - _voter.deductions;

193:         delegateVoter.deductions += _weight;

202:                 _tally.againstVotes -= _weight;

204:                 _tally.forVotes -= _weight;

207:                 _tally.abstainVotes -= _weight;

```

```solidity
File: contracts/treasury/IVotes.sol

4: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

4: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

4: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

4: import "@openzeppelin/contracts-upgradeable/interfaces/IERC5805Upgradeable.sol";

```

```solidity
File: contracts/treasury/LivepeerGovernor.sol

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

4: import "@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

5: import "@openzeppelin/contracts-upgradeable/governance/GovernorUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesUpgradeable.sol";

6: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesUpgradeable.sol";

7: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesQuorumFractionUpgradeable.sol";

7: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesQuorumFractionUpgradeable.sol";

7: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesQuorumFractionUpgradeable.sol";

7: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesQuorumFractionUpgradeable.sol";

7: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorVotesQuorumFractionUpgradeable.sol";

8: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorSettingsUpgradeable.sol";

8: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorSettingsUpgradeable.sol";

8: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorSettingsUpgradeable.sol";

8: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorSettingsUpgradeable.sol";

8: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorSettingsUpgradeable.sol";

9: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorTimelockControlUpgradeable.sol";

9: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorTimelockControlUpgradeable.sol";

9: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorTimelockControlUpgradeable.sol";

9: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorTimelockControlUpgradeable.sol";

9: import "@openzeppelin/contracts-upgradeable/governance/extensions/GovernorTimelockControlUpgradeable.sol";

11: import "../bonding/libraries/EarningsPool.sol";

11: import "../bonding/libraries/EarningsPool.sol";

11: import "../bonding/libraries/EarningsPool.sol";

12: import "../bonding/libraries/EarningsPoolLIP36.sol";

12: import "../bonding/libraries/EarningsPoolLIP36.sol";

12: import "../bonding/libraries/EarningsPoolLIP36.sol";

14: import "../ManagerProxyTarget.sol";

15: import "../IController.sol";

16: import "../rounds/IRoundsManager.sol";

16: import "../rounds/IRoundsManager.sol";

17: import "./GovernorCountingOverridable.sol";

18: import "./Treasury.sol";

```

```solidity
File: contracts/treasury/Treasury.sol

4: import "@openzeppelin/contracts-upgradeable/governance/TimelockControllerUpgradeable.sol";

4: import "@openzeppelin/contracts-upgradeable/governance/TimelockControllerUpgradeable.sol";

4: import "@openzeppelin/contracts-upgradeable/governance/TimelockControllerUpgradeable.sol";

4: import "@openzeppelin/contracts-upgradeable/governance/TimelockControllerUpgradeable.sol";

```

</details>

<a name="GAS-3"></a> 
### [GAS-3] Use Custom Errors
[Source](https://blog.soliditylang.org/2021/04/21/custom-errors/)
Instead of using error strings, to reduce deployment and runtime cost, you should use Custom Errors. This would save both deployment and runtime cost.

<details>

<summary>
There are <b>(25)</b> instances (click to show):
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

<a name="GAS-4"></a> 
### [GAS-4] Don't use `SafeMath` once the solidity version is 0.8.0 or greater
Solidity 0.8.0 introduces internal overflow checks, so using SafeMath is redundant and adds overhead.

<details>

<summary>
There are <b>(2)</b> instances (click to show):
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

<a name="GAS-5"></a> 
### [GAS-5] Long revert strings

<details>

<summary>
There are <b>(10)</b> instances (click to show):
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

<a name="GAS-6"></a> 
### [GAS-6] Functions guaranteed to revert when called by normal users can be marked `payable`
If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function. Marking the function as `payable` will lower the gas cost for legitimate callers because the compiler will not include checks for whether a payment was provided.

<details>

<summary>
There are <b>(15)</b> instances (click to show):
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

<a name="GAS-7"></a> 
### [GAS-7] Use != 0 instead of > 0 for unsigned integer comparison

<details>

<summary>
There are <b>(14)</b> instances (click to show):
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

<a name="GAS-8"></a> 
### [GAS-8] Using assembly to check for zero can save gas
Using assembly to check for zero can save gas by allowing more direct access to the evm and reducing some of the overhead associated with high-level operations in solidity.

<details>

<summary>
There are <b>(26)</b> instances (click to show):
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

<a name="GAS-9"></a> 
### [GAS-9] `internal` functions not called by the contract should be removed
If the functions are required by an interface, the contract should inherit from that interface and use the `override` keyword

<details>

<summary>
There are <b>(5)</b> instances (click to show):
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



## Non Critical Issues

<a name="NC-1"></a> 
### [NC-1] Event is missing `indexed` fields
Index event fields make the field more quickly accessible to off-chain tools that parse events. However, note that each index field costs extra gas during emission, so it's not necessarily best to index the maximum allowed per event (three fields). Each event should use three indexed fields if there are three or more fields, and gas usage is not particularly of concern for the events in question. If there are fewer than three fields, all of the fields should be indexed.

<details>

<summary>
There are <b>(12)</b> instances (click to show):
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

<a name="NC-2"></a> 
### [NC-2] Functions not used internally could be marked external

<details>

<summary>
There are <b>(17)</b> instances (click to show):
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



## Low Issues

<a name="L-1"></a> 
### [L-1] Empty Function Body - Consider commenting why

<details>

<summary>
There are <b>(2)</b> instances (click to show):
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

<a name="L-2"></a> 
### [L-2] Initializers could be front-run
Initializers could be front-run, allowing an attacker to either set their own values, take ownership of the contract, and in the best case forcing a re-deployment

<details>

<summary>
There are <b>(12)</b> instances (click to show):
</summary>

```solidity
File: contracts/treasury/GovernorCountingOverridable.sol

64:     function __GovernorCountingOverridable_init(uint256 _quota) internal onlyInitializing {

```

```solidity
File: contracts/treasury/LivepeerGovernor.sol

54:     function initialize(

60:     ) public initializer {

61:         __Governor_init("LivepeerGovernor");

62:         __GovernorSettings_init(initialVotingDelay, initialVotingPeriod, initialProposalThreshold);

63:         __GovernorTimelockControl_init(treasury());

67:         __GovernorVotes_init(votes());

69:         __GovernorVotesQuorumFraction_init(initialQuorum);

71:         __GovernorCountingOverridable_init(quota);

```

```solidity
File: contracts/treasury/Treasury.sol

16:     function initialize(

21:     ) external initializer {

22:         __TimelockController_init(minDelay, proposers, executors, admin);

```

</details>

<a name="L-3"></a> 
### [L-3] Unsafe ERC20 operation(s)

<details>

<summary>
There is <b>(1)</b> instance (click to show):
</summary>

```solidity
File: contracts/bonding/BondingManager.sol

616:             livepeerToken().transferFrom(msg.sender, address(minter()), _amount);

```

</details>



## Medium Issues

<a name="M-1"></a> 
### [M-1] Centralization Risk for trusted owners
Contracts have owners with privileged rights to perform admin tasks and need to be trusted to not perform malicious updates or drain funds.

<details>

<summary>
There are <b>(11)</b> instances (click to show):
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

