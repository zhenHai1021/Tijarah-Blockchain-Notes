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
Short:
- Used by Ethereum (upcoming Ethereum 2.0)
- Nodes **stake crypto**currency to become **validators**. Pool of validator candidates created.
- Algo select validator node from pool. Validators are **chosen** to **create a new blocks** based on the **no of coins** to stake as **collateral**.
> [!NOTE]
>  selection based on amount of cryptocurrency staked, coin age(how long validator node remains a validator) and randomization process (lowest hash value, highest staked = best-weighted)
- A block created by validator, other validators will **verify** the transactions. The valid block will be **added** to the blockchain.
- More energy-efficient than PoW and offers faster transaction processing
- However, it might favor wealthier nodes with more significant stakes
- Rewards: Validators are rewarded for their efforts in validating transactions, transaction fees

## Workflow of PoS based mechanism [^3]
1. Nodes perform transactions. The PoS algorithm puts all these transactions into a pool
2. Pool of nodes compete to become validator for the next block raise the stake. This stake is combined with other factors such as “coin age” or “random selection” to select a validator.
3. The validator verifies all transactions and publishes the block. His bet remains locked, and the reward has not been rewarded yet, so that the nodes in the network agree on a VALID new block.
4. The validator will get the stake back the reward if the block is VALID. Algoi uses coin age to select validators, then the validator of the current block reset to 0, makes low prior for the next validator election.
5. If other nodes in the network do not validate the block, the validator loses his stake and is marked as “BAD” from the algo. Start over from step 1
> [!NOTE]
>  Slashing. Penalty against validator who act maliciously, jeopardizing the network security.

![WPoS](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/23a8df9f-ca35-4e5f-890e-92ea1025435a)

## Pros and Cons of PoS
| PROS | CONS |
|--- | --- |
|Energy Efficient|-|
|Decentralization|Group of validators own total cryptocurrency, better chance becoming validators. Increasing chances, therefore centralized |
|Safety|“Noting At Stake”. Each fork will lead to multiple blockchains, and validators will work, and the nodes in the network will never reach a consensus[^4].

## Comparison PoW & PoS[^5]
| PoW | PoS |
|--- | --- |
|Mining Capacity depends on computational power|Validating capacity depends on the stake in the network|
|Miners receive block rewards to solve a cryptographic puzzle|Validators do not receive a block reward, instead, collect transaction fees as reward|
|Hackers would have a pc powerful than 51% of the network to add a malicious block, leading to 51% attack|Hacker would need to own 51% of all the cryptocurrency on the network, which is practically impossible.|
|Requires hardwares and energy, as mining depends heavily on computational power|No need to purchase specialized equipments or to solve complex equation|

## Consequences/Repercussions for Validators
Found violation of the protocol rules
1. Loss of Staked assets: Primary penalty faced by validators is the loss of a portion or the entirely of staked assets.
2. Ejection from Validator Set: Ejected from the pool, losing privilege to participate in the consensus process and reward.
3. Reputation Damage: Reputation damaged, dissuading/discourage other participants from delegating the assets to the slashed validator in future
> [!Note]
> Reduced Earning: Even if x rejected, slashed validators may face earning reduction due to the delegated assets loss & lower ranking within validator set [^6] 

## Conclusion
In PoS, Crypto owners can stake (pledge and lock up) their coins to be validators. When a new block needs validation, the PoS protocol selects a validator node from the staker’s pool, based on their staked amount and randomization. The chosen validator proposes  the block, the validators verifies the transaction. If VALID, the block is added to the chain and hence transaction fee as rewards. If INVALID, penalties by losing a portion of the staked holdings.
Stakers can unstake their coins to stop being validators but lose the role until re-staking. PoS replaces PoW computationally-intensive mining, enabling distributed consensus, security and validation through staking instead of mining.

---
## REFERENCES
[^1]: https://www.fool.com/terms/p/proof-of-work/#:~:text=The%20proof-of-work%20model%20is%20a%20consensus%20mechanism%20used,transactions%20has%20a%20specific%20hash. 
[^2]: https://www.tryspeed.com/blog/what-is-proof-of-work/ 
[^3]: https://www.analyticsvidhya.com/blog/2022/09/blockchain-proof-of-stake-pos/#commentModule 
[^4]: https://www.analyticsvidhya.com/blog/2022/09/blockchain-proof-of-stake-pos/#commentModule
[^5]: https://medium.com/@aurangzaib.khalid/what-is-meant-by-proof-of-work-pow-and-proof-of-stake-pos-in-blockchain-2138887a2167 
[^6]: https://www.nervos.org/knowledge-base/slashing_in_PoS_(explainCKBot) 
