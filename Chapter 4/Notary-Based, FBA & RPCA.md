# Notary-based by CORDA
Consensus that relies on a group of trusted entities (notaries) to validate and confirm transactions or blocks. It introduces a layer of centralization through these trusted notaries to validate and confirm transactions or blocks.

## How Notary-based Work
1. A set of trusted/pre-selected entities for validating transactions.
2. Notaries are often chosen based on reputation, expertise, or trustworthiness
3. When a transaction occurs, it is submitted to the notaries for validation
4. Notaris verify the transaction’s validity and reach consensus.
5. Once the consensus is achieved, the transaction is confirmed.

## Example:
1. Side chains: Use to transfer assets between different blockchains. Notaries validate transactions moving between main and side chains.
2. Cross-Chain Protocols: Some cross-chain protocols involve to ensure secure communication between different blockchain.

|PROS|CONS|
|---|---|
|Interoperability: can facilitate cross-chain by allowing different blockchains to communicate through notaris|Centralization: If notaries collude or compromised, entire system affected|
|Privacy & Confidentiality: Handle confidential transactions without revealing sensitive data to the entire network|Trust: Notaries’ reputations and selection processes are critical|
|Efficiency: Quickly validate transactions, reducing confirmation times|-|

Reference Journal[^1][^2]

# Federated Byzantine Agreement (FBA)[^3]
- Alternative to traditional BFT 
- Federated groups of nodes into smaller network. Nodes in a sub-network communicate with each other to reach consensus on the state of the network, then the sub-networks communicate with each other to agree on global state
- System wide quorums emerge from decisions made by individual nodes

**Quorum slice**
Quorum slices are **subsets of nodes** that can **convince** a specific node to agree. A node can rely on **multiple slices**, with agreement criteria based on factors like **requiring 3/5** selected entities to agree. Nodes can be part of other nodes’ slices, adding complexity. When relying on a slice, it must be **trusted enough** that the node agrees if the slice agrees. QS provides more flexibility compared to requiring full quorum agreement.

<img src="https://miro.medium.com/v2/resize:fit:786/format:webp/1*wNYButkgGK63boJPGz4pvQ.png" width=300px height=100px>

**Quorum Intersections** (Overlapping quorums, where different quorums share some common node)
Nodes can have diff configurations files, leading to dynamic formation of **quorum slices** and **quorums** within the network. It **prevents ‘disjoint quorums’**, quorums that don't overlap and **can independently agree** on transactions. To make sure **quorum intersections**, the system **avoids disjoint** quorums that could **diverge and agree** on **conflict data** to maintain consistency.

<img src="https://miro.medium.com/v2/resize:fit:786/format:webp/1*9GiwaiN0By6HSsDLhQJe0A.png" width=300px height=250px>

**Blocked vs Divergent States**
If nodes get ‘blocked’ from agreement, the blockchain slows down. When nodes present values diff from other nodes, the system is ‘divergent’. A divergent system is more dangerous than block system.
> Blocked system are slow, but divergent system start displaying contradictory data.

<img src="https://miro.medium.com/v2/resize:fit:786/format:webp/1*4NcGc6Gh26kg0MqlI6w-rw.png"  width=300px height=250px>

|PROS|CONS|
|---|---|
|Interoperability: Facilitate cross-chain by allowing diff blockchain communicate through notaries.|Centralization Risk: Rely on fixed set of notaries. Notaries’ selection and behaviour impact the overall system.|
|Privacy: Handle confidential transactions without revealing sensitive data to network.[^4]|Trust: User must trust the integrity and competence of notaries. Critical on notaries’ reputation and selection processes.|

# Ripple Protocol Consensus Algo (RPCA)
- Each node maintains a Unique Node List (UNL) of trusted node
- Try to minimize the probability of collusion (pc) and increase UNL size

## How it works

1. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/faca3b77-e0a6-4080-8afb-da591801d941" width=500px height=500px>

2. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/ead93667-faa4-460b-a9bc-c51fb18f58a2" width=500px height=500px>
<span>A user initiates a transaction and sends it to all the nodes. Then all nodes verify that transaction and add it to their candidates sets</span>

3. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/bcaf3276-dcdb-4d5a-b3e1-ee2e2abdb23a" width=500px height=500px>
<span>More transaction are initiated by different users on the network and all these transactions are verified by all nodes and added to their candidate sets</span>

4. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/cde2ce49-91e4-4ddb-8584-769ebbe1b381" width=500px height=500px>
<span>All the nodes send their candidates sets to other nodes on the network as proposals (arrows are only shown for the proposals received by our node)</span>

5. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/b2b67552-96a3-48bf-a17d-97d0cbd285bf" width=500px height=500px>
<span>Server5 is not in the UNL thus its proposal is rejected and all other proposals are moved forward for voting</span>

6. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/e3b6cd1e-9025-44f1-b6d7-32d9308af833" width=500px height=500px>
<span>Every node conducts a vote based on the proposals received</span>

7. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/08e299c8-09aa-4e10-b1f0-9c12be4db3fb" width=500px height=500px>
<span>The threshold for proposals in this round is 50%. Thus, transactions receiving more than 50% votes are retained and others are dropped from the candidate set (Transaction 4 is being removed as it only received ¼ or 25% votes.</span>

8. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/6c5b58c8-10f7-4dbb-9df8-01393d84d86e" width=500px height=500px>
<span>Voting continues until the threshold reaches 80%. Then all the remaining transactions (that received 80% votes) are added to the ledger. Lets suppose transaction 2 is also receives less than 80% votes upcoming phases, then it is also removed.</span>

9. <img src="https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/2a76b01d-2c6d-42b8-8900-82f7f7c17b86" width=500px height=500px>
<span>Only 2 transactions receive more than 80% votes and they are added to the ledger and a new LCL is generated.</span>

Image sources[^5]

|PROS|CONS|
|---|---|
|Efficiency: Processes transactions swiftly and securely|Centralization: Rely on fixed set of trusted nodes. |
|Decentralization: No single entity controls the network|-|
|Trust Relationship: Nodes form trust relationships through their Unique Node Lists (UNLs)|-|



---
# REFERENCES
[^1]: https://www.mdpi.com/2079-9292/12/13/2804
[^2]: https://www.researchgate.net/publication/349806763_PoNW_A_Secure_and_Scalable_Proof-of-Notarized-Work_Based_Consensus_Mechanism
[^3]: https://medium.com/@learnwithwhiteboard_digest/what-is-byzantine-fault-tolerance-bft-in-blockchain-explained-cb06a12559be
[^4]: https://towardsdatascience.com/federated-byzantine-agreement-24ec57bf36e0
[^5]: https://www.educative.io/answers/how-does-the-ripple-protocol-consensus-algorithm-rpca-work







