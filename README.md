# 20-Solidity

#### Unit 20 Solidity Smart Contracts Homework - Dan Smith  
* Associate Profit Splitter : [AssociateProfitSplitter.sol](./AssociateProfitSplitter.sol)

##### Motivation
This code and contract shows a proof of concept for even profit sharing amongst associates.

##### Summary
This basic contract accepts ETH and will divide the ETH evenly among three specified addresses, or "associates."
The contract will takes _one, _two, and _three constructor addresses, representing employees to share ETH with, along with the amount of wei to distribute.
Only the contract owner may deposit or distribute ETH.
When dividing equally among the three addresses, any remainder is transferred back to the msg.sender, which is required to be the contract owner address.
If the contract receives ETH directly, it will in turn call the deposit function, which will include the requirement of only allowing the contract owner address to deposit ETH.
