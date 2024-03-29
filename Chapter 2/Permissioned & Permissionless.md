## Permissioned vs Permissionless Networks
Eg, a bank may be running a permissioned blockchain operated through a designated number of nodes internal to the bank to track money transfers.You cannot access this blockchain because you do not have the permissions required. In contrast, you could join a permissionless blockchain like a cryptocurrency mining network once you have established a semi-anonymous account in that network.

||Permissionless|Permissioned|
|-|-|-|
|Overview| - Open network available for anyone to interact and participate in consensus validation. - Fully decentralized across unknown parties| Closed network. Designated parties interact and participate in consensus validation. Partially decentralized (eg. distributed across known parties)|
|AKA| Public, Trustless| Private, permissioned sandbox|
|Attribute| <ul><li>Full transparency of transactions, based on open source protocols</li><li>Development via open source</li><li>Mostly anonymous, with some exceptions</li><li>Privacy depends on technological limitation or innovations</li><li>No central authority</li><li>Often involves digital asset or token for incentive</li></ul>|<li>Controlled transparency, based on organizations’ goals</li><li>Development via private entities</li><li>Not anonymous</li><li>Privacy depends on governance decisions</li><li>No single authority, but private group authority decisions</li><li>May or may not involve digital assets or tokens</li></ul>|
|Benefits|<li>Broader decentralization, extending access across more network participants</li><li>Highly transparent, which is beneficial for speed and reconciliation across unknown parties</li><li>Censorship resistant, due to accessibility and participation across locations and nationalities</li><li>Security resilience, since attackers cannot target a single repository, and it is costly and difficult to corrupt 51% of the network</li><li>Less energy efficient because network-wide transactions verification is resource-intensive</li><li>Slower and difficult to scale, as high volume can strain network-wide transaction verifications</li><li>Less user privacy and information control</li>|<li>Incremental decentralization, but participation from multiple business helps mitigate risks of highly centralized models</li><li>Stronger information privacy because transaction information is only available based on permissions</li><li>Highly customizable to specific use cases through diverse configurations, modular components and hybrid integrations</li><li>Faster and more scalable, since fewer nodes manage transaction verification and consensus</li><li>Limited decentralization because a network with fewer participants increase risk of corruption or collusion</li><li>Risk of override, since owners and operations can control or change the rules of consensus, immutability or mining</li><li>Less transparent to outside oversight, since participants are limited and operators determine privacy requirements</li>|

## 1. What is permissionless blockchain and what are its key characteristics? (Bitcoin & Ethereum)
Permissionless blockchains, also aka **trustless** or **public blockchains**, open networks available to everyone to participate in the consensus process blockchain use to **validate** **transactions** and **data**. In a permissionless blockchain, users typically create a personal address which can be usernames or account profile attached to email addresses. Permissionless blockchain are fully **decentralized** across unknown parties. The key characteristics of permissionless blockchain are:

- **full transparency** of transactions
- **Open source development**: the chain’s nodes and features are documented or recorded as publicly accessible information. They also allow developers to study their characteristics and develop compatible **open-source** software like **crypto wallets**, NFT, and other DeFi resources, such as digital asset exchanges.
- **Anonymity**, with some exceptions participating in network activities: mining, validating transactions: Demand a little user data because they have no identity verification or access control layers. It enables users to transact while remaining anonymous. These chains enforce verification procedures like **Know Your Customer (KYC)** and **Anti Money Laundering (AML)**. However, these processes only limit the ability to transact on the network. They do not affect the blockchain’s anonymity.
- **Heavy use** of **tokens** and other **digital assets** as **incentives** to **participate**

Pros
**Decentralization**: Broader decentralization that extends access across **more/much** network participants than in permissioned blockchain, **no central** authority controlling the network, making it **resilient** to **censorship** and **central points of failure**

**Transparency**: A high degree of transparency, which is **verifiable** by **all network** participants. **Wallet addresses** cannot generally be **tracked** back to the blockchain users, and **transactions** are **encrypted** using various **cryptography** methods.

**Accessibility**: **Resistance** to **censorship**, and **participation** across locations

**Security**: since intruders can’t target a **single repository**, and it’s **difficult** to corrupt 15% of the network to **disrupt** consensus mechanisms

**Immutability**: Data stored is **immutable**, which cannot be **altered/modified** or deleted. Also, these blockchains are **tamper-proof**, providing **long-term capacity** to **retrieve** and verify the information

**Censorship Resistance**: From decentralized nature, these chains are **tamper-proof**; all their nodes **see each other’s** transactions and avail (help) their information to public users, ensuring nothing is **concealed** or manipulated

**Ease of use**: **Zero authentication** procedures. These chains are **accessible** from anywhere **worldwide** through the **internet**

Cons
**Efficiency**: Poor energy efficiency due to the **resource-intensiveness** of network-wide verification of transactions

**Performance and scalability**: From the **verification process** on computing **resources**

**Privacy**: **less privacy** and user control over information

**Scalability**: Offer nearly everyone that requires **higher computing resources** to sustain their networks. Thus, it needs **more nodes**; each node **consumes high power** for verifying transactions. This results in **difficulty to scale up**.

**Security**: Allowing **all traffic** into a blockchain **without authorization** compromises security.

Use Case
Tend to be used in applications with a **strong financial** component or that require highly decentralized blockchain. Ideal for applications where **trust** among participants is **minimal**, and a **high degree of transparency** and **security** is required, such as in public cryptocurrencies
- Digital asset trading: For permitting as many users to acquire and trade digital assets
- Crowdfunding and donations: to allows as many people to access the contribution feature and monitor the funds
- Distributed file storage, Eg. Blockchain storage: As a storage layer for publicly accessible information

## 2. What is permissioned blockchain and what are its key characteristics?  (Hyperledger Fabric and R3’s Corda)
In contrast, permissioned blockchains, as **private blockchain** or permissioned, are **closed networks** in which previously **designated parties**, who are sometimes members of a consortium, interact and participate in consensus and data validation. They are **partially decentralized** in the sense of being distributed across known participants rather than unknown participants. Participation in these networks requires **authorization** from the network’s governing entity or consortium. Tokens and digital assets are possible but less common than in permissionless blockchains. This structure allows for **more control** over the network activities. Key characteristics of permissioned blockchain include:

- **Controlled transparency** based on the goals of participating organizations
- Development by **private entities**
- **Lack of a central authority/anonymity**, but a **private group authorizes decisions**
- Only verified and **authorized entities** can **participate** in network: transaction validation, governance, and access to certain information
- **Access control layer** designed with an **extra security** layer that strictly assigns **different permissions** to **different users**. The layer limits users based on their roles. Certain role allowed access to certain information.

Pros
Decentralization: Decentralization can be incremental, which allows **multiple business** to **participate** without all the risks of **highly centralized** models

Privacy: Strong privacy because **permission** is needed to **access** transaction information and **visible** and **restricted** to certain network participants

Customization: **customizable** for specific uses, since it enable **diverse configurations**, modular components and hybrid integrations

Performance and Scalability: Fewer nodes manage transaction: verification and consensus

Transparency: Nodes, or the users and their connections, are known and their **transactions** are **visible**. This can defend a company against **double invoicing (duplicate invoice)**, spending, paying or any other number of errors that can be made using enterprise management programs.

Proper governance structure: **Clear governance structure**. A hierarchical system that makes **updating** and **implementing changes** and effect rules on the chain easier.

Cost effective: Permissioned blockchains are **highly cost-effective**. They require **few nodes**, **reducing** operational **costs**. They also have a **limited no. of users, scaling down** infrastructure **req and costs**.

Cons
Corruption and Collusion: Risky, because of **fewer participants** than in a permissionless blockchain

Overridden consensus: Consensus is more **easily overridden** because the **owners** and **operators** can **change the rules** of consensus, immutability and mining

Transparency: **Less transparency** to outside oversight because the number of participants is **limited** and the **network’s operators** determine privacy requirements.

Centralization: **Negating** the blockchain **decentralized aspect**.

Power to censorship: **Privately regulated**, there is much **human influence** on the **chain’s performance**. Increase the likelihood of administrators **withholding information** from users or **micromanaging** transactions in their favor.

Security: Although these blockchains are often safe from external attacks, the integrity relies heavily on the administrators. If the administrators or private entities on the network are being compromised or manipulated the data in the blockchain. It then compromises the protection of the chain.

Use Case
Suitable for **enterprise and business** applications where **privacy compliance**, and **fast transaction processing**. Permissioned blockchain have enabled new applications that depend on privacy and security include:
- Supply chain provenance tracking: for storing data on circulating and stored goods or available services
- Banking and financial: To store client transaction data and verification
- Manufacturing: For documenting manufacturing processes, ingredients and workflows
Claims settlement
- Healthcare and Life Science: To store patient medical records and health research data
- Consumer packaged goods: for maintaining inventory

## Key Differences of Permissioned and Permissionless Blockchains
### 1. Accessiblity and Privacy
<ol type="a"><li>Permissioned chains limit access to authorized users while maintaining **high privacy standards**</li><li>Permissionless blockchain grant accessibility to all interested users, making them publicly accessible chains.</li></ol>

### 2. Scalability and Efficiency
<ol type="a"><li>Permissioned requires fewer nodes, translating to lower costs and ease of network growth.</li><li>Permissionless are power and resources intensive as the growth of users, making scaling more complex.</li></ol>

### 3. Transaction speeds
<ol type="a"><li>Private’s transaction speeds are higher</li><li>Public have slower speeds of their traffic and the no of computations needed for validating transactions.</li></ol>

### 4. Decentralization and trustlessness
<ol type="a"><li>Private are more centralized and distrusted since few participants managing</li><li>Public are fully decentralized, fostering trustworthy</li></ol>

### 5. Full transparency
<ol type="a"><li>Private have less transparency (limited decentralization)</li><li>Public all information is publicly accessible</li></ol>

## Similarities of Permissioned and Permissionless Blockchains
1. **Decentralization**: **Both** run on **Decentralized Ledger Technology (DLT)** even though they have a **centralization aspect**. Running on DLT gives both chains the capabilities of **decentralized networks**.
2. **Transaction speed per second (TPS)**: **Permissionless network** may be **slower** at **processing transactions** than a **permissioned** one, but both chains have impressive speeds. Eg. Solana, one of the fastest permissionless chains, can run 65k TPS.
3. **Scalability**: Since **permissionless** chains started **using Proof-of-stake** consensus algorithms, they have drastically **lowered** the **computational power** needed to run transactions. This has made them almost as **scalable** as **permissioned chains**. Also, the existence of **layer 2 networks** that run on top layer 1 blockchain platforms helps boost the **scalability**

## How to choose the right blockchain
### 1. Use case
<ol type="a"><li>Permissioned chain are optionally the best option for industries that handle many private data and processes. Or the private administrator decide own resources distribution.
</li><li>Permissionless are more convenient for shared resources and publicly accessible information.</li></ol>

### 2. The number of users
<ol type="a"><li>Its crucial to consider the number of users accessing it, and the limited user base for the permissioned blockchains.</li><li>More people are better on permissionless</li></ol>

### 3. Accessibility and Efficiency
<ol type="a"><li>Permissioned chain have more complex accessibility features but are highly efficient</li><li>Permissionless ones are easy to explore but less effective</li></ol>

