# Differences between Bitcoin and Ethereum
|Platform|Consensus Mechanism|Scalability|Programming Language|Use Cases|
|--|--|--|--|--|
|Ethereum|PoW (Transitioning to PoS)|Working on Ethereum 2.0 for improved scalability|Solidity|General-purpose blockchain, decentralized applications|
|Quorum (ConsenSys)|Raft of Istanbul BFT|Focus on privacy and performance|Solidity|Enterprise solutions, finance|
|Hyperledger Fabric|Pluggable, supports various mechanisms|Modular architecture for scalability|Go, Java, Node.js|Supply chain, finance, enterprise solutions|
|Corda|Notary-based consensus|Designed for privacy and scalability|Kotlin, Java|Financial services, legal, supply chain|
|IBM Blockchain|Supports multiple mechanisms|Modular for different business needs|Go, Java|Supply chain, finance, healthcare|
|Bitcoin|PoW|Limited scalability, slower transaction processing|Bitcoin Script|Peer-to-peer digital currency|
|Hyperledger Sawtooth|PoET (Pluggable)|Modular design for flexibility|Python, Go|Supply chain, finance|
|Stellar|Federated Byzantine Agreement (FBA)|High throughput and fast settlement|Stellar (custom language)|Cross-border payments, remittances|
|Ripple|Ripple Protocol Consensus Algorithm (RCPA)|Fast and low-cost transactions|Ripple Transaction Protocol (custom)|Cross-border payments, remittances|
|EOSIO|Delegated Proof of Stake (DPoS)|High throughput and low latency|C++|Decentralized applications, social media|
|MaalChain|Maal Validator DAO (PoA)|High TPS (UpTo 4000)|Go|Decentralized Applications, Concept of Identity based Private dApps|

## Hyperledger Sawtooth
![PoET](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/4020103b-4fb6-41bf-bcd2-19dfa23b8f55)

Consensus Mechanism Proof of Elapsed Time (PoET)
- Follows a lottery system that spread the chances of winning equally across network participants, giving each node the same chance (probability)
- PoET generates a random wait time for each node in the blockchain; each node must sleep for that duration
- Node with the shortest wait time will wake up first and win the block, thus being allowed to commit a new block to the blockchain.
- The PoET workflow is similar to PoW but consumes less power bcs it allow a node to sleep and switch to other tasks for the specific time, thereby increasing network energy efficiency.

## Understanding Bitcoin
Launched in 2009 by the pseudonymous Satoshi Nakamoto, Bitcoin (BTC) stands as the pioneering cryptocurrency, dominating the digital currency landscape. It was conceived as a decentralized alternative to traditional currencies, facilitating **peer-to-peer value transfers**. Bitcoin transactions undergo **verification** by a **network of nodes **using **cryptography** and are **recorded** on a **transparent ledger** known as the blockchain. This blockchain is distributed among multiple nodes to prevent **tampering**; any attempt at altering the blockchain is swiftly detected and rejected by the network, known as tampering. Tampering is detected in the Bitcoin network through hashes, long strings of numbers that must match across all nodes. The **SHA-256 hash** function turns data into these unique strings, which are then **broadcasted** and **added** to new blocks once **validated**. This safeguarding process relies on **cryptographic hashes**, **unique strings** of numbers ensuring **consistency** across all nodes. Miners, employing proof-of-work, validate and add transactions to new blocks, ensuring consensus and thwarting malicious alterations. 

## Understanding Ethereum
Ethereum (ETH) was proposed in late 2013 and brought to life in 2015 by Vitalik Buterin. Ethereum’s primary purpose extends beyond the simple transfer of value. Instead, Ethereum is designed to be a platform that allows **P2P contracts** and applications to be built and run without control, permission, or interference from **third parties**. These decentralized apps (DApps), are powered by Ethereum’s own **cryptographic token**, Ether (ETH). Ether is used to interact with applications on the Ethereum network. Paying for transactions, creating smart contracts and using DApps all require users to pay fees in Ether. As the value of Ether went up, it also started being used as a store of value. Decentralized applications (DApps) on Ethereum enable the utilization of Ether and other cryptocurrencies in various ways, such as **collateral** for loans or earning interest by lending them out. Collateral is assets offered as security against loan repayment. For instance, users can deposit $1,000 worth of ETH into a DApp, securing a $750 loan while earning interest on their deposited funds.

|Aspect|Bitcoin|Ethereum|
|:---|:---|:---|
|Purpose|Decentralized and digital cash system|Cryptocurrency. Open-source platform for DApps and smart contracts. Directly without middleman|
|Technology|Consensus mechanism. Proof-of-Work (PoW), where miners solve mathematical problems to validate transactions and add to the blockchain. High consumption computational power and energy.|Transition with PoW to Proof-of-Stake (PoS) with Ethereum 2.0 upgrade. In PoS, validators are chosen to create a new block holding the amount of cryptocurrency & willing to “stake” as collateral. Efficient > PoW|
|Scalability|PoW is not scalable. Only handle a limited no. of transactions per second, a max of around 7 per second.|PoS is scalable. Processes up to 30 transactions/second, still face scalability issues. Through upgrades such as transitioning to PoS and an upgrade called sharding.|
|Supply (total no. of coins created)|Capped supply of 21 million coins|Has no maximum supply limit, which means unlimited no. of Ether can be created. However, the inflation rate is low to negative.|
|Use Cases|Digital money/digital gold - digital currency or a store of value|Smart contracts & DeFi, without third intermediaries. Ethereum platform for most NFT, unique digital assets that can represent ownership or proof of authenticity for everything from digital art to virtual real estate|
|Price|Like most cyptoassets. Primary drive of the crypto market, given its larger market cap. When bitcoin’s price rises, it often pulls up the price of other cryptocurrencies, including ETH. Usually influenced by a number of factors which include: supply and demand, market sentiment, regulatory news and events.|Impacted by Bitcoin’s, influenced by factors unique to Ethereum such as updates to is platform, its usage in DeFi, and demand for blockspace. Ethereum’s price, in turn, influences the price of smaller cryptoassets especially those that use Ethereum’s blockspace such as DeFI, NFT and DAO projects.|
|Block Time|10 minutes on avr|10-15 seconds on avr|
|Transaction throughput|7 transaction per second|30 transaction per second|
|Supply|Finite supply-capped at 21 million BTC|Infinite supply|
|Address|Star with a 1, a 3, “bc1”|Start with “0x”|

## What gives Bitcoin value?
1. It's features
2. It's network effects

## Characteristics
1. It has a limited supply: There will only ever be 21 million bitcoins.
2. Rarity: When the things are not rare, they have less value over time. And if that is used as money, it leads to less purchasing power, which is the amount of goods and services that can be purchased with amounts of money
3. It's easily divisible: One bitcoin can divided into 100 mil pieces, whereas 1 US Dollar can be broken into 100 pieces. Means that the world will never "run out" of Bitcoin. It can always be divided into smaller and smaller pieces.
   ![1 us d 100 cent](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/f5dd8797-2779-44f8-ad5a-a33ab26b0db0)

4. It's durable: The internet is durable as it is made up of a global network of computer systems. Similarly, a huge globally distributed network of independently operated computers track, Bitcoin ownership. This ensure that no bitcoin is lost.
5. It's more portable: Sending any amount of bitcoin to anyone globally in minutes
6. It's more easily verified: Easy to verify the authenticity of bitcoin.
7. Stronger network effects. Bitcoin's network effects benefit from the scale and internet speed. Bitcoin is a digital asset whose proponents (Promoters) are digital natives.

How does Bitcoin work?
1. Transactions are initiated by people
2. Transactions are broadcast to the network, verified by the nodes, and collect in a "pool"
3. Miners complete a math problem. Whoever (one) solve the first wins the right to make the next block
4. The winning miner takes transcations from the pool to build a new blcok. The new block includes a set reward of new Bitcoin for the miner.
5. The new block is verified, added to the chain, and broadcast to the network.

## ETH Characteristics
1. Open and permissionless access: anyone is free to create, run and use applications on the Ethereum network. The network doesn’t pick which applications to run, no account deed to use/deploy. Instead, the shared computer’s resources are delegated purely by market forces. In other words, anyone willing to pay will have access the network’s processing power - **gas fee**. Anyone in the world can use, eg, the finance protocols like lending and borrowing that are built on Ethereum. Means that anyone can build an application on Ethereum, and have it be accessible to anyone without having rely on approval from intermediaries.
2. Transparency: Anyone can see how the the applications run on it work, since there are no hidden algorithm, so participants can evaluate the minutest details of applications before deciding whether to interact with them. Anyone can see, eg, exactly how much collateral has been help in a lending protocol - from the protocol’s inception right up to the present.
3. Immutability: The immutability of current and historical states, in combination with the above-described transparency, gives all participants a high degree of assurance that fraud is not being committed.
4. Durability: The shared computer’s components - it’s **processing power** and memory are spread out around the world. **Decentralized** = no single entity is in control. No even governments can ban Ethereum and possibly even target well-known people associated with it, it is hard to prevent average people from using it, and even shut it down completely.
5. Neutrality: Ethereum may adapt to the needs of participants in a way that would appear **different** from **legacy computing models**. Specifically, participants are endowed (provided) with a **higher degree **of assurance that they always have fair **access** to the **network’s resources** and that the network will not evolve in a way that prioritized the needs of one group over the needs of another.

## Ethereum and the Web 3.0
The concept of Ethereum as a platform and its potential towards Web3. Currently, the internet operates on Web2, characterized by centralized entities like Facebook, Google, and Uber, which exert full control over users' access to products and services. These intermediaries often leverage users' personal information for profit and maintain closed-source systems, limiting users' ability to influence the products they use.

Web3 social network where users own their data and can choose to monetize it. Advertisers could transact directly with users, rewarding them for their attention, thus eliminating the need for intermediaries. Users, who are also stakeholders in the network, could actively participate in its evolution by voting on upgrade proposals and deciding how to allocate funds. This model incentivizes participation and innovation, potentially leading to rapid growth and dynamic evolution of the network in the users' interests.

## What is ETH used for?
ETH is also the currency used to pay for the resources of the Ethereum network. To send one ETH to another, you must attach a fee which is paid in ETH. The fees goes to validators, who are network participants that ensure transactions are processed in accordance with rules of the protocol. However, the Ethereum network can do more than just move ETH around. As Ethereum is designed to be a type of shared computer that is capable of. Thus, ETH is the fuel needed to power the computer. Means that, whenever you want to use applications built on Ethereum, you’ll need to pay fees in ETH.

1. Smart contracts and DApps
Smart contracts are self-executing contracts with the terms of the agreement between buyer and seller being directly written into lines of code. They run on the Ethereum blockchain, automatically executing transactions and **enforcing agreements **when prefined conditions are met, without any need for intermediaries. This enable the creation of DApps, which operate on a P2P network of computers rather than a single centralized server. DApps built on Ethereum can serve a wide range of purposes, from **financial tools** and games to **complex data management system**s. Use of ETH as a form of payment for executing these smart contracts ensures that developers and users can transact and interact with DApps in a secure and decentralized manner.

2. DeFi (Decentralized Finance)
Represents a shift from traditional financial systems to P2P enabled by decentralized technologies built on the Ethereum blockchain. DeFi platforms allow users to lend, borrow, trade and earn interest on their crypto assets without third intermediaries. These services are accessible to anyone, anywhere as long as they have access to the internet and ETH to pay for transaction fees. The openness and accessibility of DeFi could potentially democratize access to financial services, offering greater inclusivity compared to conventional financial systems. ETH vital in this ecosystem by facilitating transactions, executing smart contracts, and serving as collateral for various DeFi protocols.

3. NFT
Unique digital assets that represents ownership or proof of authenticity of a wide range of tangible and intangible assets from arts, music to virtual real estate and collectibles. Unlike cryptocurrencies such as Bitcoin or even ETH, which are fungible and can be exchanged on a one to one basis, each NFT has a distinct value and cannot be exchanged on a like for like basis. Ethereum’s blockchain supports the creation and trading of NFTs through its smart contract, with ETH being used to buy, sell these digital assets. The NFT market has exploded in popularity, highlighting Ethereum’s role in pioneering new forms of digital ownership and the monetization of digital content.

4. Staking and Ethereum 2.0
Transition to Ethereum 2.0 shift from Proof of Work (PoW) to PoS, staking has become a central element of the network’s security and consensus mechanism. In PoS, ETH holders can **lock up** a portion of their **tokens** as a **stake** in the network, essentially acting as **validators** who propose and **validate** blocks of transactions. **Staking ETH** not only helps **secure** the network, but also allow **stakeholders** to **earn** rewards in proportion to their staked amount. This shift aims to **reduce** the **network energy consumptio**n significantly, making Ethereum more sustainable while increasing its scalability and security. 

### Layer 2 Scaling Solutions
Too many demands on its capacity, leading to higher gas fee and slower transaction time during peak periods. Layer 2 scaling solutions, such as rollups and state channels, offer a way to handle transactions off the main Blockchain (layer 1), while still ensuring the security and decentralization of the network. These solutions allow for faster and cheaper transactions by batching or processing them on a separate layer, then recording the final state on the main blockchain. ETH remains integral to these operations as transactions within Layer 2 solutions often require ETH for fees or collateral. By leveraging these technologies, Ethereum aims to significantly increase its transaction throughput without trade off security or decentralization, making it more accessible and usable for everyday applications.

### The Ethereum Virtual Machine (EVM)
EVM is the heart of the Ethereum network. EVM interprets and executes the smart contracts written in Ethereum’s programming language, such as Solidity. It ensures that every Ethereum node runs the same instructions, maintaining the blockchain’s integrity and consensus. ETH is used as “gas” to power these operations, compensating (repay) for the computational resources required to execute transactions and smart contracts. This mechanism prevents spam on the network and allocates resources efficiently. The flexibility and power of the EVM have enable developers to build a wide array of decentralized applications, pushing the boundaries of what can be achieved with blockchain technology.

### Token Standards and ERC-20 Tokens

Token standards on the Ethereum blockchain, particularly the ERC-20 standard, have been instrumental in the widespread adoption of Ethereum for creating digital assets. ERC-20 defines a common list of rules that Ethereum tokens must adhere to, allowing for seamless interaction with smart contracts, decentralized applications, and other tokens. This standardization has facilitated the growth of a vibrant ecosystem of tokens serving various purposes, from representing digital currencies and assets to governance tokens that grant holders voting rights in decentralized protocols. ETH itself is used for transaction fees and gas costs when interacting with these tokens, reinforcing its position as the foundational currency of the Ethereum ecosystem.

### History of Ethereum’s Monetary Policy
On 15 sep 2022, Ethereum shift from PoW to Pos. This marked a major turning point in Ethereum’s monetary policy. Ethereum used to employ a PoW consensus mechanism, which the miners who succeeded in extending the Ethereum blockchain by applying computing power to the hashing algorithm were rewarded in ETH, and new blocks where added approximately every 10-15 seconds.

When the Ethereum network launched in 2015, the block reward was initially set to 5 ETH. In other words, 5 ETH were added to the total supply every 10-15 seconds. Considering that the total circulating supply of ETH (eg. the “stock”) at that point was relatively small, and the issuance rate (eg, the “flow”) was high, Ethereum started off with a low stock-to-flow ratio. This meant that the out-of-the gate inflation rate was above 20% on an annual basis. However, as the total supply (stock) expanded, any additional supply would have diminishing impact. The stock-to-flow ratio increased. One year later, Ethereum’s inflation rate had been reduced to the low teens (on an annual basis).

At block 4,370,000 in October 2017, Ethereum implemented EIP-649, reducing the block reward to 3 ETH and lowering annual inflation to less than 10%. Another reduction occurred at block 7,280,000 in February 2019, with EIP-1234 lowering the reward to 2 ETH, resulting in an annual inflation rate of 4.5%. EIP-1559, introduced in August 2021, allows for the burning of ETH based on network demand, potentially leading to periods of deflation during high transaction activity. Ethereum's transition to Proof-of-Stake under "Ethereum 2.0" drastically reduced issuance by around 90%, enabling the possibility of total supply contraction over time in combination with EIP-1559 adjustments.
