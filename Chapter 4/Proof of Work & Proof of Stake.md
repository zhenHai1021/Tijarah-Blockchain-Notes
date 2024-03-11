# Consensus Mechanism
## The Need for Consensus Mechanisms in Blockchain
Consensus Mechanisms is vital for blockchain. They are the protocols that ensure all nodes in a blockchain network **agree** on the **validity of transactions**, maintaining the **integrity** and **trust** of distributed ledger. Without consensus mechanisms, blockchain would lack the necessary synchronization and agreement among nodes, leading to potential conflicts and security issues.

Why are Consensus Mechanisms Necessary?
1. **Decentralization**: Enable network participants to agree on the current state of the ledger, eliminate the central authority
2. **Security**: Protect blockchain from fraudulent transactions and malicious actors. By requiring agreement from multiple nodes, consensus mechanisms make it hard for any single entity to manipulate the ledger.
3. **Integrity and Trust**: Ensures that once a transaction is confirmed, it can be trusted as valid. This system’s reliability among users.

Consensus mechanisms are the core of blockchain, ensuring the proper functioning, security and reliability of decentralized digital ledgers. Each mechanism has its unique features, benefits and drawbacks, making it suitable for different types of blockchain applications. The choice of a consensus mechanism depends on the specific requirements of the blockchain, including speed, energy efficiency, security and level of decentralization. 


## Proof of Work
Short:
- Miners use computational power to find a "target hash"/value (nonce) for the next block.
- Puzzle: Involves performing a hash function repeatedly, altering the nonce each time, until the output meets the network criteria (like a leading zeros)
- Miners verify transactions and create new blocks
- Verification process involves solving an algo, that combines previous block hash with new block header hash. Resulting hash must match target value to add block to chain
- The first miner to find the target hash can add the next block then rewarded
- Finding the target hash is difficult (requires computation) but verifying it is easy
- This asymmetry prevents manipulation while allowing decentralized consensus.
- Mining difficulty adjusts to control block time based on computational power.
- Block Reward: Include newly minted coins and transaction fees.

  ![WPoW](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/356f18aa-db4e-444b-aa84-9503c1579157

## Pros and Cons of PoW
| PROS | CONS |
|--- | --- |
|High level of security. To alter any block, the intruders may need to redo the work for the block and the subsequent, which is infeasible due to high computational cost. (No Single Point of Failure)|Inefficient with slow transaction speeds and expensive fees especially the network grows (scalability issues)|
|Provides a decentralized method of verifying transactions. Also allows anyone to participate in the mining process|High energy usage for calculations|
|Allow miners to earn crypto rewards|Mining often requires expensive equipment and high energy consumption, as miners’ electrical power usage to perform necessary calculations.|

---
## REFERENCES
[^1]: https://www.fool.com/terms/p/proof-of-work/#:~:text=The%20proof-of-work%20model%20is%20a%20consensus%20mechanism%20used,transactions%20has%20a%20specific%20hash. 
[^2]: https://www.tryspeed.com/blog/what-is-proof-of-work/ 
