# Delegated Proof of Stake (DPoS)
- Implemented in EOS, Tron and others
- A variant of PoS where stakeholders vote for a few delegates who manage the blockchain on their behalf
- Offers scalability and efficiency but less decentralized
- Representative democracy where stakeholders delegate voting power to trusted entities

How DPoS work[^1]
1. Election of Delegates: Network participants **vote** using **tokens/coins** for their **trusted delegates** in the network. Chooses a number of delegates from the election.
2. Role of Delegates (**witnesses**): **Elected** delegates **validates** the transaction block.
> [!NOTE]
> Strong reputation are usually elected as witnesses
3. Block Creation and Validation: Delegates **takes turn** to create new block to network, round-robin. **Other** delegates **validate** the blocks.
4. Rewards: Delegates are incentivized through block rewards, which are distributed among contributions. Some systems also reward voters.

![WDPoS](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/d6052866-d8a8-4e09-a932-63372d90f452)

| PROS | CONS |
|--- | --- |
|Increased Transaction Throughput: handle a higher volume of transactions per second, suitable for scalability, as less confirmation time | Centralization: limited no of delegates could lead to centralization, vulnerable to collusion (illegal agreement) |
|User participation: Encourage broader community involvement | Voter Apathy: If token holders not participating in voting process, lead to lack of representation in the delegate selection.|
|Democratic: More power in the hands of network participants.|Hard to find and struggles with the risk of discrepancy (inconsistent logic)|
|There is no need for specialized and expensive equipment to be delegate|Dissuade beginner network participants with lower coins during voting|

Consideration[^2]
1. **Malicious Delegates**: Risk of a 51% attack where **majority of delegates** act maliciously to do **as they want** with the network.
By allowing **token holders** to **delegate the voting power**, DPoS can have **malicious actors** delegates to **gain control** of the **majority** of the network and manipulate for their own advantage, including updates to the network.
> [!Tip]
> Sorely penalize validators
2. **Dependent on Delegators**: Requires numerous delegators **remain active**. Any vote for dividing delegation among several delegates to distribute the risks. Users with smaller stake may **refuse** to **take part** in voting.

## Comparison PoS & DPoS
| PoS | DPoS |
|--- | --- |
|randomly selects the block producer among validators.|choose delegates by the voting system. Each delegate get them turn in the process of submitting their translation blocks, also role in verifying other blocks added to the network.|
|Transaction volume lower than DPoS|Has a higher transaction volume than PoS. Faster process than PoS.|

# Nominated Proof of Stake (NPoS) {Polkadot}
- Allows **token holders** to **nominate validators** to represent them in block validation process
- Only **nominated validators** can participate in block formation, each nominator can nominate a **sepcific no of validators** (16)
- These networks automatically distribute the stake among the participating validators evenly and penalize both validators and nominators if they act maliciously

![NPoS](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/f0033402-524c-41ec-8890-b1834738a317)

> Splitting the nominators' stake into validators' backing of roughly equal size. Provide fair representation and a high security level

## How Nominatted Proof of Stake work (Nominators and validators)[^3]
1. Validator: Verify transactions for the next block, not chosen randomly, but nominated by other Nodes.
2. Voting Mechanism: Follow sequential Phragmen election technique for fair representation. Active validator set chosen by nominators for each block.
3. Nomination Process: Nominators can nominate a specific no of validator nodes (16). Validators receive slots in validator set relative to stake backing them. Nominators can evaluate validators based on metrics.
4. Validator Selection: Validators with most nominations and higher stake backing = validator set of the block. Network distributes stake among chosen validators for fairness.
> [!NOTE]
>  Validator set changes every “era” (4-24 hours)

| PROS | CONS |
|--- | --- |
|Democratic: Allow nominators to select trusted validators. Distributing all stakes evenly.|Nominating Malicious Validators: Losing part of your stake for choosing malicious validators. Rewards even. *Both nominators and validators.|
|Fair Punishment: Punishments for both validators and nominators. Slashes the stake of the nominator who vouched (confirm) for the validator too.|Active Validator Selection: Can endorse multiple validators, not all the validators nominated might be active. If fraction of nominated validators are accepted, the stake associated is divided among the successful nominees.|
> [!NOTE]
> The stake from nominators remains, does not contribute to the rewards earned by validators

# Proof of Authority (PoA) {Permissioned blockchain}
- Nodes are validated and selected as trustworthy entities
- Used in private or consortium blockchains where high throughput and scalability are needed
- Less decentralized, relying on the reputation of the validators.

## How Proof of Authority [^4]
1. In PoA, rights to generate new blocks are awarded to authorized nodes/”Validators”
2. Validators run software to put transactions in blocks. The process is automated, less constant monitoring from validators.
3. Validators ensure their computers uncompromised.
4. PoA suits for both public and private where trust is distributed. 
5. Leverage the identities value. Block validators stake their reputation instead of coins
6. PoA is secured by trust in selected identities/validators

Conditions for PoA consensus:
- Validators confirmed with real identities.
- Willing to invest coins and reputation at stake. 

| PROS | CONS |
|--- | --- |
|High tolerance, secure since trusting a set of pre-approved validators.|Not decentralized. Lead to lesser accountability and transparency.|
|Predictable new blocks of time of interval.|Validators are visible, could lead to 3rd party manipulation.|
|High transaction rate, less computational resources, hence reducing operational costs.|Limited scalability, limited no of validators, thereby limiting the no of transactions. Restricts access, thereby making unsuitable public networks.|

## Common Attack
1. Distributed Denial of Service Attack (DDoS): Aim to spam traffic to make it unavailable. 
2. 51% attack: Attacker require to control over 51% of network nodes. PoA allow non-consecutive block approval from any one validator, meaning the risk of damage is centralized to the authority node.

---
# References
[^1]: https://www.shiksha.com/online-courses/articles/delegated-proof-of-stake-dpos/  
[^2]: https://www.ledger.com/academy/what-is-delegated-proof-of-stake-dpos#:~:text=Delegated%20Proof%20of%20Stake%20is,designed%20to%20address%20POS%27s%20limitations.
[^3]: https://medium.com/web3foundation/how-nominated-proof-of-stake-will-work-in-polkadot-377d70c6bd43 
[^4]: https://www.geeksforgeeks.org/proof-of-authority-consensus/ 
