## Impact
A malicious MEV bot can prevent others from participating in the auction and they always get a revert (DoS on other participants).

## Proof of Concept
Let's describe this in the following scenario:
- MEV bot tracks the mempool and see there is submitted a transaction with value `x` (let's say this transaction is submitted by actor `Alice`).
- It front-runs the Alice transaction and submits a transaction with higher value (`x` + 1) and higher gas price.
- Transaction of MEV bot will be executed first, and now `returnHighestBid` returns (`x` + 1)
- Transaction of Alice will be reverted, because of this line:
```solidity
require(msg.value > returnHighestBid(_tokenid) && block.timestamp <= minter.getAuctionEndTime(_tokenid) && minter.getAuctionStatus(_tokenid) == true);
```
(The above condition is checking `x` > (`x` + 1) ? No, so the transaction will be reverted. In other words, participants should always offer a higher price than the previous highest price, otherwise the transaction will be reverted)
- Now MEV bot cancels its bid (it gets-back its funds) and repeats this act until the auction ends and prevents others from participating in auction. (Auction may ends without any winner)

## Tools Used
Manual Review
## Recommended Mitigation Steps
Consider some solutions that prevents against this attack.








