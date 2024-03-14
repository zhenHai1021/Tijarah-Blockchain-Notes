# Byzantine Fault Tolerance (BFT)
System ability to continue operating even if some of its nodes fail or act maliciously

## Problem with Byzantine Generals' Problem[^1]:
- Has an army surrounding a fortress, decide to attack or retreat **TOGETHER**
- Same decision = they are successful
- Each general stayed with their armies. They can communicate with one another via messengers
- If miscommunication or 'traitors' causing some generals to attack while the others retreat, then the battle is lost.

<img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/aef22bf9-425a-41d1-b239-d6594e245786" width="100px" height="100px"> 

 ## How BFT work[^2]
1. The client makes a request to the primary node
2. The primary node sends the request on to secondary nodes
3. The nodes process the request, provide the service, and respond to the client
4. The client waits until it has received the same response from m+1 nodes, with m being the max no of malicious/faulty nodes the system allows
5. In short, the max no of malicious nodes cannot be equal or greater than one-third (33%) of the system total nodes

| PROS | CONS |
|--- | --- |
|Less computing power: No need any miners to solve the complex equation|Vulnerable to Sybil Attacks where one party is able to control large portion of nodes. |
|Transactions confirmation: if the nodes are in agreement about a block of transaction, then it is confirmed immediately|Requires communication between nodes at every step of the process. Takes time for scalability standpoint|
|Nodes can share in the rewards|-|
> [!Tip]
> Sybil Attacks (named after a book about a woman with multiple personality disorder)

# Practical Byzantine Fault Tolerance (PBFT)
- Address the cons of traditional BFT
- BFT is inefficient and unscalable
- Relise on direct communication between each pair of nodes in network
- Nodes spinning up and going down unexpectedly, nearly impossible to maintain an update list for direct communication

## Improve on BFT
1. Make for Large network: By eliminating the communication between every node in the network
2. Efficiency: Define order for the nodes in network with primary and backup nodes. Broken innto few phases in which a leader proposes a block, and each node validates it and approves. Once the nodes accomplished this, considered finalized.

| PROS | CONS |
|--- | --- |
|Fault Tolerance: Deal with node failure|Centralization: Leader node to define the content of next block and process of getting it approved|
|Transaction Finality: accepted block may be removed from the ledger after a reorganization|Scalability: Requires messages from some % of the nodes in the network to finalize block’s content. No of message scale with size of the network|
|BFT: Can handle no of malicious nodes in the network|Network overhead: The more nodes need to communicate, the more bandwidth it consumes|
> [!NOTE]
> Sybil Attack: pBFT decision on receiving msg from certain nodes. If an attacker controls many diff nodes, having outsized votes and may approve malicious blocks.

<img src="https://assets-global.website-files.com/6433e6f821ae13dd37394322/6439167c0f24b24248245731_syb1a.png" width=400px height=400px>

# Istanbul Byzantine Fault Tolerance (IBFT)
Ensure single, agreed-upon ordering transactions in blockchain, aims for high throughput and low latency optimizing communication and consensus process. 
- Well-suited for consortium and private where participants are trusted.
- Designed to work in Ethereum-based
- Remove some overhead and redundant message present in pBFT, improving performance
- Designed to scale better than PBFT for permissioend network with a known set of validators.
- Validators node responsible in proposing and validating, even diff role in each round, such as proposer, committer, and message relayer.
- Can tolerate up (N-1)/3 faulty nodes in a network of N validators

## Key advantage[^3]
Block Producer = BP
1. Immediate block finality: Allow one block for each block height (h) by elected BP. Provides immediate confirmation of executed transactions.
2. Reduced time between blocks: Every BP get its chance to add block, the effort required to READ/WRITE and validate is reduced, inc the throughput of the chain
3. High data integrity and fault tolerance: Ensure data integrity as only trusted BPs contribute to blocks
4. Operationable flexible: Consortium of BPs can be updated, ensure trustworthy BPs remain member of consortium.

## How IBFT Work[^3]
1. Uses a pool of BP nodes in a permissioned blockchain network. Once BP is selected as the Proposer to propose a block. The other BPs validate and sign the block.
2. Once a supermajority (around 66%) of BPs sign, the block is added to the blockchain.
3. The proposer role then moves to the next BP in line. If not enough BP reject the block. The Proposer moves to the next BP to start a new round.
4. "Block Locking" where added blocks are finalized and cannot be altered. IBFT tolerants up 1/3 of faulty nodes while ensure consensus as long as over 2/3 BPs are honest.
> Ensure system integrity and fault tolerance in the permissioned network.


---
# REFERENCE
[^1]: https://www.youtube.com/watch?v=_fgW2IM6ctM 
[^2]: https://www.fool.com/terms/b/byzantine-fault-tolerance/#:~:text=Byzantine%20Fault%20Tolerance%20is%20a,a%20group%20of%20Byzantine%20generals. 
[^3]: https://medium.com/ledgerium-io/ledgerium-blockchain-ibft-consensus-a596b3403bb1 
