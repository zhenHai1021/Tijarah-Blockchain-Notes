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
 
---
[^1]: https://www.youtube.com/watch?v=_fgW2IM6ctM 
[^2]: https://www.fool.com/terms/b/byzantine-fault-tolerance/#:~:text=Byzantine%20Fault%20Tolerance%20is%20a,a%20group%20of%20Byzantine%20generals. 
