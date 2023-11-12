## Impact
Participant calls `participateToAuction` and winner calls `claimAuction`, if both transactions are executed at `auctionEndTime` (in same block where block.timestamp = auctionEndTime), if the transaction of winner is executed earlier, the participant will lost their funds and the funds will be locked in contract for ever.

## Proof of Concept
Let's take a look at `participateToAuction`:
```solidity
// @audit `participateToAuction` doesn't check if the auction is already claimed or not
function participateToAuction(uint256 _tokenid) public payable {
        require(msg.value > returnHighestBid(_tokenid) && block.timestamp <= minter.getAuctionEndTime(_tokenid) && minter.getAuctionStatus(_tokenid) == true);
        // ...
}
```
**1. The above condition lets Participant's transaction to be executed at `auctionEndTime` (because it checks block.timestamp `<=` auctionEndTime and not `<` )**
And look at `claimAuction`:
```solidity
    function claimAuction(uint256 _tokenid) public WinnerOrAdminRequired(_tokenid,this.claimAuction.selector){
        require(block.timestamp >= minter.getAuctionEndTime(_tokenid) && auctionClaim[_tokenid] == false && minter.getAuctionStatus(_tokenid) == true);
        // ...
```
**2. The above condition lets Winner's claim transaction to be executed at `auctionEndTime` (because it checks block.timestamp `>=` auctionEndTime and not `>` )**

So what we get from 1 and 2 ? if the transaction of a participant and the transaction of winner are executed in same block (for example block `N` where timestamp of block `N` is equal to `auctionEndTime`) -> then if transaction of winner executes earlier, the participant has lost their funds forever. (In other words, Winner transaction can be executed at `x` and Participate transaction can be executed at `x`, so if Winner claim transaction is executed earlier, it means auction is claimed, so which auction does the participant participate in? While the auction has been claimed by the winner)

Scenario:
- There is a block called `N` and timestamp for block `N` is 123456
- Assume the auction ends at `123456` in block `N` (it means, auctionEndTime = 123456 = block.timestamp)
- Winner calls `claimAuction` and Alice (a participant) calls `participateToAuction`.
- If both transactions are executed in same block (block `N`) and transaction of Winner executes earlier, Alice funds will be lost forever (because the both transactions are allowed to be executed at exactly `auctionEndTime`) and there is no way for Alice for get their funds back (because the auction is already claimed and there is no any function to cancel the bid after auction ends).


## Tools Used
Manual Review

## Recommended Mitigation Steps
Add the following line in `participateToAuction`:
```diff
diff --git a/smart-contracts/AuctionDemo.sol b/smart-contracts/AuctionDemo.sol
index 95533fb..435c0cd 100644
--- a/smart-contracts/AuctionDemo.sol
+++ b/smart-contracts/AuctionDemo.sol
@@ -55,6 +55,7 @@ contract auctionDemo is Ownable {
     // participate to auction

     function participateToAuction(uint256 _tokenid) public payable {
+               require(auctionClaim[_tokenid] == false, "It's too late");
         require(msg.value > returnHighestBid(_tokenid) && block.timestamp <= minter.getAuctionEndTime(_tokenid) && minter.getAuctionStatus(_tokenid) == true);
         auctionInfoStru memory newBid = auctionInfoStru(msg.sender, msg.value, true);
         auctionInfoData[_tokenid].push(newBid);

```























