# Proof of Elapsed Time (PoET) {Permissioned blockchain}
- Used in Intel's Sawtooth platform (Intel Corporation)
- Randomizes the process of electing block creators using a fair lottery system
- Generates a random wait time for each node in blockchain network; each node must sleep for that duration
- Node with the shortest wait time will wake up first to win the block
> Enerfy-efficient and suitable for permissioned

<img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/9aa25f6e-3394-4a19-983f-8d174af2a52c" width=400px height=300px>

## Rules[^1][^2]
1. Ensure the participating nodes genuinely select a time that is indeed random and not a shorter duration chosen.
2. Check if the nodes are not choosing the shortest wait time on purpose.
3. Establishes that the winner has completed the waiting time.
Fast Fact:
Uses much less energy than PoW since randomly selects a node instead using all miners on a network in a competition.

## How PoET Work[^3]
1. Fair lottery system where every node is equally chosen, spreads the chances of winning across the largest possible no of network participants
2. Each node in the network must wait for a random chosen time. The node can sleep or do another task for the random chosen time.
3. First to wake up/complete the waiting time wins the block, broadcasting the info to the whole network. Process repeats of the next block.

## PoET vs PoW[^2]
|-|PoET|PoW|
|---|---|---|
|Blockchain Type|Permissioned|Permissionless|
|Transaction Rate|Medium|Low|
|Token Needed|No|Yes|
|Energy Efficiency|More Energy Efficient|Less Energy Efficient|
|Power Consumption|Less Power Consumption|More Power Consumption|
|Network Efficiency|Increased Network Efficiency|Less Efficient Network|
|Environment|Random selection environment|Competitive work environment|

## Phases
1. Selection Process: Ensure the validity of the node to generate new block. Then the node is eligible to get a timer object. The numbers are assigned to each node as a timer object by Intel's RAND, random number generator. It generates difficult-to-detect random no.
2. Generate Process: After timer object expires, the node wakes up, eligble to forge new block to network. The active node generates the hash of its block of transactions and submits it for the acceptance. 

|PROS|CONS|
|---|---|
|Less power consumption: nodes can "Sleep" or switcch to other tasks while waiting|Compatibility issues: High depends on tools by Intel might raise issue with others|
|Less resource intensive: RAND without being resource-intensive/complex mechanism|-|
|High transaction rate: Up a Million transactions/s, faster transaction processing|Specialized hardware required: specialized hardware for PoET, cannot be used by most people|
|Permissioned: Ensure network security against cyberattacks|-|

# Proof of Burn (PoB)[^4]
- PoW without energy waste
- Mechanism to promote periodic burning to maintain mining power
- Burnt coin power "Decays" partially with each new block
- Encourages regular minig activity instead of one-time investment
- Miners may need upgrade equipment as tech advances

![PoB](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/36567de3-21cc-44b3-8d19-d85033630b7e)


## How PoB work
1. Miners “burns” (send to an unspendable address) virtual currency tokens to mine/add new blocks. Granted right to write blocks proportional to coins burnt
> [!NOTE]
> Burnt coins are liking ming rigs, more coins burnt=bigger rig
> burning: miners send tokens to verifiable addresses from which the tokens can never be spent/retrieved.
2. Burning process consumes minimal resources to keep network active & agile
> [!Tip]
> Native/alternate chain currency (BTC) can be burnt
3. Transactions to burn own coins or include others’ burnt coins in blocks
4. Rewards given in native currency for burning activity

## Example of PoB
1. Slimcoin (SLM): First cryptocurrency to implement PoB. Miners burn SLM coins to compete for mining the next blocks and receive additional blocks. It combines PoB with PoS & PoW to increase security. 
2. Counterparty (XCP): Participants burnt bitcoin during a one-time burn period and automatically received XCP proportional to the amount burnt. This ensured equitable distribution of the fixed supply of XCP tokens.

|PROS|CONS|
|---|---|
|Minimal Energy Consumption: Economical and requires minimal hardware setup.|Initial Coin Loss: Burning coins means user lose the coins permanently.|
|Sustainable: Miners burn a portion of their coins to generate new blocks. This keep system security.|Centralization: Exploited in more coins can be burned to earn more rewards. Lead to increased centralization.|
|Market: Coins burnt reduce the circulating supply, potentially increasing the value of remaining coins.|Lack of incentives: PoB don’t provide block rewards. Miners rely on transaction fees.|
|Long term commitment: Demonstrate commitment to the network by burning coins.|Complexity: Complex than PoW or PoS|
Reference[^5][^6][^7]

---
# REFERENCE
[^1]: https://www.investopedia.com/terms/p/proof-elapsed-time-cryptocurrency.asp#:~:text=Proof%20of%20elapsed%20time%20(PoET)%20is%20a%20consensus%20mechanism%20often,they%20are%20allowed%20to%20join. 
[^2]: https://www.geeksforgeeks.org/proof-of-elapsed-time-poet-in-blockchain/ 
[^3]: https://www.investopedia.com/terms/p/proof-elapsed-time-cryptocurrency.asp#:~:text=Proof%20of%20elapsed%20time%20(PoET)%20is%20a%20consensus%20mechanism%20often,they%20are%20allowed%20to%20join. 
[^4]: https://www.investopedia.com/terms/p/proof-burn-cryptocurrency.asp#:~:text=Proof%20of%20burn%20is%20one,any%20cryptocurrency%20coin%20double-spending. 
[^5]: Proof of Burn Consensus Algorithm in Blockchain - GeeksforGeeks 
[^6]: Proof of Burn (PoB) | Learn Crypto | Coinmerce
[^7]: What are proof-of-burn (PoB) and proof-of-weight (PoWeight)? - AAG (saakuru.com)
