# Consensus Mechanism
## The Need for Consensus Mechanisms in Blockchain
Consensus Mechanisms is vital for blockchain. They are the protocols that ensure all nodes in a blockchain network **agree** on the **validity of transactions**, maintaining the **integrity** and **trust** of distributed ledger. Without consensus mechanisms, blockchain would lack the necessary synchronization and agreement among nodes, leading to potential conflicts and security issues.

Why are Consensus Mechanisms Necessary?
1. **Decentralization**: Enable network participants to agree on the current state of the ledger, eliminate the central authority
2. **Security**: Protect blockchain from fraudulent transactions and malicious actors. By requiring agreement from multiple nodes, consensus mechanisms make it hard for any single entity to manipulate the ledger.
3. **Integrity and Trust**: Ensures that once a transaction is confirmed, it can be trusted as valid. This system’s reliability among users.

Consensus mechanisms has its unique features, benefits and drawbacks, making it suitable for different types of blockchain applications. The choice of a consensus mechanism depends on the specific requirements of the blockchain, including speed, energy efficiency, security and level of decentralization. 

# Proof of Work
Short:
- Miners use **computational power** to find a "target hash"/value (**nonce**) for the next block.
- **Puzzle**: Involves performing a hash function repeatedly, altering the nonce each time, until the output meets the network criteria (like a leading zeros)
- Miners **verify** transactions and **create** new blocks
- Verification process involves **solving** an algo, that combines previous block hash with new block header hash. Resulting hash must match target value to add block to chain
- The **first miner** to find the target hash can **add the next block** then **rewarded**
- Finding the target hash is difficult (requires computation) but verifying it is easy
- This asymmetry prevents manipulation while allowing decentralized consensus.
- Mining difficulty adjusts to control block time based on computational power.
- Block Reward: Include newly minted coins and transaction fees.

![WPoW](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/e0f0eb71-8e50-45d1-9064-f4e6e33bb229)
Idea Refer [^2]

## Pros and Cons of PoW
| PROS | CONS |
|--- | --- |
|High level of security. To alter any block, the intruders may need to redo the work for the block and the subsequent, which is infeasible due to high computational cost. (No Single Point of Failure)|Inefficient with slow transaction speeds and expensive fees especially the network grows (scalability issues)|
|Provides a decentralized method of verifying transactions. Also allows anyone to participate in the mining process|High energy usage for calculations|
|Allow miners to earn crypto rewards|Mining often requires expensive equipment and high energy consumption, as miners’ electrical power usage to perform necessary calculations.|

## Example how Bitcoin uses proof of work to maintain the integrity of its blockchain [^1]
When Bitcoin transactions occur, they go through a security verification and are grouped into a block to be mined. Bitcoin’s PoW algo then generates a hash of the block. The SHA-256 algo generates a 64 character hash for each block. Miners compete to find a hash value below the target block hash. The first miner to find a valid hash gets to add the new block to the blockchain. They receive Bitcoin rewards in the form of newly minted coins and transaction fees. Bitcoin has a fixed maximum supply of 21 million coins, after that, miners will continue receiving transaction fees for their service. The PoW aims to add a new block every 10 min. Mining difficulty automatically adjusts to account for changes in total mining power. If blocks are computed too quickly, the difficulty increases to slow it down. If too slowly, the difficulty decreases to speed up the 10 minute block time.

# Proof of Stake

---
## REFERENCES
[^1]: https://www.fool.com/terms/p/proof-of-work/#:~:text=The%20proof-of-work%20model%20is%20a%20consensus%20mechanism%20used,transactions%20has%20a%20specific%20hash. 
[^2]: https://www.tryspeed.com/blog/what-is-proof-of-work/ 
