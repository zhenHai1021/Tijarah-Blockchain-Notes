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


---
# REFERENCE
[^1]: https://www.investopedia.com/terms/p/proof-elapsed-time-cryptocurrency.asp#:~:text=Proof%20of%20elapsed%20time%20(PoET)%20is%20a%20consensus%20mechanism%20often,they%20are%20allowed%20to%20join. 
[^2]: https://www.geeksforgeeks.org/proof-of-elapsed-time-poet-in-blockchain/ 
[^3]: https://www.investopedia.com/terms/p/proof-elapsed-time-cryptocurrency.asp#:~:text=Proof%20of%20elapsed%20time%20(PoET)%20is%20a%20consensus%20mechanism%20often,they%20are%20allowed%20to%20join. 
