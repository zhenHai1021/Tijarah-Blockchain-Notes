# Distributed Ledger Technology (DLT)
DLT is the technology infrastructure and protocols that allow simultaneous access, validation, and record updating across a **networked database**/multiple places at the same time. Unlike traditional databases, DLT has **no central data** store or administration functionality. In DLT, **every node** in the network **processes every transaction**, coming to its own **conclusions** and then **voting** on the conclusions to make sure the **majority agree** with the conclusion. This process is known as **consensus**, and it allows for the **recording** of transactions in a decentralized and secure manner.

Key: 
<ul>
   <li>Distributed ledgers are maintained by a network of nodes, each of which has a copy of the ledger, validates the information, and helps reach a consensus about its accuracy.</li>
<li>Distributed ledgers have been around for decades but have become more well-known, researched, used and developed since Bitcoin was introduced</li>
   <li>Distributed ledger can be used in nearly every industry where data is collected and used</li>
   <li>All blockchains are distributed ledgers, but not all distributed ledgers are blockchains</li>
   <li>Though DLT enhances accountability, security, and accessibility, it is still complex, difficult to scale, and not subject to strong regulation.</li>
</ul>

Characteristics:
1. Decentralization: Unlike centralization, a single entity takes control of the entire database. DLTs distribute the control among all participants/nodes in the network. This enhances security and reduces risks of central points of failure.
2. Transparency and Immutability: Transparency transactions on DLT to all nodes, and cannot be altered once recorded. The immutability ensures the integrity of of the ledger and builds trust among users
3. Consensus Mechanisms: DLTs use various consensus mechanisms to validate transactions including Proof of Work, Proof of Stake, and others, depending on the specific implementation. These ensures that all participants agree on the state of the ledger.
4.  Security: The decentralized and immutable DLT, combined with cryptography, makes it secure against tampering and fraud.

Applications of DLT:
1. Cryptocurrencies: Eg. Bitcoin. DLT enables the secure and transparent recording of cryptocurrency transactions.
2. Supply Chain Management: DLT enhances transparency and traceability in the supply chain, allowing all parties to **track the movement of goods**, manufacturing, processing and their authenticity. This enables real-time visibility into supply chain operations, reducing manual work. Eg. a distributed ledger used to track the provenance of goods, ensuring ethical sourcing and enhancing consumer trust.
3. Banking and Financial Services: In banking and finance, DLT can **streamline processes**, **reduce fraud**, and improve compliance through secure and immutable **record-keeping**. One notable use case is the implementation of smart contracts in trade finance. **Smart contracts** facilitate the **execution** and **settlement** of trade transactions, reducing inefficiencies and eliminating the need for intermediaries. Additionally, DLT enables faster cross-border payments, enhances **Know Your Customer (KYC)** processes and provides **secure digital identity** solutions.
4. Identity Verification: DLT provides a secure way of managing **digital identities**, reducing risk of identity theft and fraud.
5. Healthcare: DLT used to improve **patient data** management, streamlining and enhance security. With DLT, medical records can be securely stored and shared, ensuring data privacy and integrity. Additionally, **smart contracts** can **automate insurance claims**, reducing administrative burdens and improving **efficiency**. DLT also enables secure and transparent clinical trials, ensuring the integrity of data and enhancing trust in the research process.
6. Real estate: DLT improves by **simplifying property** transactions, **reducing paperwork** and enhancing security. With the implementation of smart contracts, property transfer can be **automated**, ensuring accurate and tamper-proof records of **ownership**. Blockchain platforms build on distributed ledgers can provide transparent and auditable property registries, reducing the **risk of fraud** and disputes and **removing the need of costly intermediaries**. Furthermore, DLT can enable **fractional ownership** of real estate, unlocking **new investment opportunities** and **increasing liquidity** (asset converted into ready cash without affecting its market price) in the market.
7. Government and Public Records: Governments are adopting DLT to improve the integrity and accessibility of public records. Documents like **birth certificates, land titles,** and **business licenses** can be securely stored on a DLT, making them less susceptible to alteration or loss. This innovation reduces the **red tape** involved in **document retrieval**, **speeding up processes** like **property transfers** and **identity verification**.
8. Education and Credential Verification: DLT in streamlining **credential verification**. Education institutions are leveraging DLT to securely store and share **academic results/records** and **certifications**. Students and employers can easily **verify the authenticity** of these documents, reducing the risk of **forged qualifications** and simplifying the hiring process.
9. Agriculture and Food Safety: DLT is transforming **food safety** and **quality assurance**. DLT solutions enable farmers, distributors, and retailers to **track** the origins of food products from the field to the store shelf. In the event of a **food safety recall**, this technology allows for **pinpointing** the affected products, **reducing waste** and **safeguarding** consumer health.
10. Environmental Sustainability: DLT also employed to promote environmental sustainability. By facilitating the **trading** of **carbon credits** and **monitoring emissions**, DLT in reducing **greenhouse gas emissions**. This encourages companies to take an active role in environmental stewardship and combat climate change.

History of Distributed ledgers
<ul>
   <li>
      In 1990s, it become possible for multiple computers and users in different locations to solve problems and return the solutions to a central location. 
   </li>
   <li>
      The concept of a distributed ledger when cryptographers Stuart Haber and W.Scott Stornetta introduced the idea of a cryptographically secure chain of blocks. Their work laid the foundation for DLT addressing the problem of timestamping digital documents to prevent backdating or tampering.
   </li>
   <li>
      The history of DLT occurred in 2008 when an anonymous individual or group operating under the pseudonym Satoshi Nakamoto published the Bitcoin whitepaper. Nakamoto’s innovation combined the concepts of a decentralized ledger with a new form of digital currency, Bitcoin. This blockchain-based ledger introduced a groundbreaking solution to the problem of trust in digital transactions, allowing peer-to-peer transfers of value without relying on intermediaries.
   </li>
   <li>
      As Bitcoin grained traction, it become evident that the underlying blockchain technology could be adapted for applications beyond cryptocurrency. In 2015, Ethereum, created by Vitalik Buterin, introduced the concept of smart contracts. These self-executing agreements further expanded the scope of DLT, enabling programmable, automated, and trustless interactions. The programs used <strong>automation</strong> and <strong>data encryption</strong> techniques to <strong>verify database transactions</strong> or <strong>changes</strong> in the <strong>database’s state</strong>. This is called <strong>consensus</strong> - the act of <strong>automated majority agreement</strong> on <strong>transaction validity</strong>, where a transaction is simply a change made to a database’s state. 
   </li>
   <li>
      DLT evolved into scalable and programmable platforms, Eg, Ethereum and Hyperledger Fabric, where solutions can be created to use a database, or ledger, for everything from tokenizing physical assets to streamlining manufacturing the business process.
   </li>
</ul>

## How DLT works
DLTs allow **information** to be stored securely and accurately using **cryptography**. The data can be accessed using **“keys”** and **cryptographic signatures**. Once the information is stored, it can become an immutable database; the rules of the network, written into the coding of the database programming, govern the ledger.

As they are decentralized, private, and encrypted, DLTs are less **prone to cybercrime**/cyber attacks, as all the **copies** stored a**cross the network** need to be attacked simultaneously for the attack to be successful. Additionally, the **P2P sharing** and updating of records make the whole process much faster and effective. P2P where multiple nodes store, validate and update the ledger simultaneously. This eliminates the need for a **central authority** and reduces the risk of a **single point of failure**. To give an illustration, when a new transaction is initiated, it is broadcast to all nodes in the network, and each node independently validates and records the transaction. 

The process begins with the replication of **digital data** across the network of nodes. Each node maintains an **identical copy** of the ledger and independently processes new update transactions. To ensure consensus, all participating nodes employ a consensus algorithm that determines the **correct version** of the ledger. Once a consensus is reached, the updated ledger is propagated to all nodes, ensuring **synchronization** and accuracy.

Every device on a distributed ledger network stores a copy of the ledger. These devices are called nodes, a network can have no. of nodes. Any changes to the ledger, such as moving data from one block to another, are recorded across all nodes. Because each node has a copy of the ledger, each one publishes its version with the latest transactions.

If the **network** reaches a consensus about the validity of the **latest ledger**, the transactions are **finalized, encrypted**, and used as a basis for the following transactions. This is how blockchains develop, each block contains **encrypted information** about the proceeding block, which makes them **impossible to change**. Moreover, DLT systems exhibit an i**mmutable nature**, rendering it exceptionally **difficult to modify** or delete data once it has been added to the ledger. 

> Fast Fact: if something is immutable, it is unable to be changed. Distributed ledgers are only immutable if they are programmed to be that way. Blockchains are always immutable because they are decentralized public ledgers.


## Industries using Distributed Ledger Technology 
DLT are created for many different purposes, but one of the most used ways is as a platform for others to scale and use. Eg. Hyperledger Fabric. It a modular and scalable DLT platform that several business have used to create solutions that span many industries. Including aviation, education, healthcare, insurance, manufacturing, transportation, and utilities.

Eg. Fujitsu’s Rice Exchange was created to trade rice, ensuring data regarding sources, prices, insurance, shipping, and settlement are recorded on the ledger. Anyone involved can look at any data and find accurate information regarding the entire process because it cannot be altered. All data is entered and secured automatically by the platform, it will eventually provide tracking information for rice shipping containers as it is shipped to the destination.

### Example 
1. Blockchain. Blockchain, which bundles transactions into blocks that are chained together and then broadcasts them to the nodes in the network. Aka DL.
2. Tangle. Tangle, another type of DLT, is toward internet of things (IoT) ecosystems. Tangle been described as “Permissionless, feeless, scalable distributed ledger, designed to support trustworthy data and value transfer between humans and machines.

## Uses of DLT
1. Record transactions: DLT enables secure, transparent, and decentralized transactions without the need for a central authority. As DLT is a ledger, it records inflows and outflows. Through this naturally lends itself to financial records, DLT can record any type of transaction even without financial undertones (suggested but not direct recommend)
2. Secure identities: DLT can be used to create a secure and tamper-proof digital identity for individuals, as the DLT can provide a reliable way to verify identities and prevent identity theft.
3. Collect votes: DLT can be used to create a secure and transparent voting system that can prevent voter fraud and ensure the integrity of the voting process. The transactions are recorded, a transparent, immutable, open ledger of interactions with users is saved. This enhances the equity and believability of a collection of opinions
4. Enter contracts: DLT allows for smart contracts agreements that automatically execute or complete based on prevailing conditions (existing at a particular time). This limits error, and DLTs make it more difficult for precarious activity by bad actors.
5. Demonstrate ownership: DLT can be used to record property transactions, creating a tamper-proof and transparent record of ownership and transfer of property. Though there are some limitations on translating real-world ownership of physical assets to a distributed ledger, the ledger may be able to convey an unchangeable source of truth regarding ownership.

> Important: DLT may also be referred to as a shared ledger as it requires a ledger to be shared across a peer-to-peer computer network.

## Advantages of DLT
Decentralized: Since there is no **central point of control of failure**. This makes DLT more resilient to attacks and less vulnerable to system-wide failures. Also, DLT uses cryptographic algorithms to secure data, DLT is nearly impossible to tamper with records. This enhances trustworthiness of the data and reduces the risk of fraud. 

Transparency: Allow for data and transactions access, allowing all users of the DLT greater visibility into the operations of the system. This may lead to greater investment from users due to transparency and accountability of records.

Intermediaries: DLT can streamline processes and automating transactions through smart contracts. Because smart contracts may automatically execute when contract conditions are met, there may be less need for human interaction or administration. This can reduce costs and increase efficiency.

Financial: Some people may not have access to traditional banking services. As DLT often relies only on an internet connection, individuals who would be otherwise limited may have access to a greater range of services. This extends to the use of different platforms and networks via interoperability. This lower the overall operational costs from the elimination of a central authority. 

## Disadvantages of DLT
Maintenance: Largely due to the infancy of DLT, there are still large downsides to the technology. DLT is still complex and difficult to implement and maintain. In order for companies or individuals to leverage the solution, it often requires expertise and knowledge to implement.

Scalability: DLT may struggle with scalability as the no. of participants and transactions increases. As a result, DLT processes may lead to slower processing capabilities or higher costs of use. Besides, some DLTs such as Bitcoin require a significant amount of energy to maintain the network and process transactions. This can have negative environmental impacts. Eg consensus mechanisms, such as directed acyclic graph (DAG), are addressing these scalability challenges. 

> DAG - a conceptual representation of a series activities of a data pipeline. Although used in different circles, both terms, DAG and data pipeline. In short, a DAG (or a pipeline) defines a sequence of execution stages in any non-recurring algorithm

>> 1. Directed: In general, if multiple tasks exist, each must have at least one defined upstream (previous) or downstream (subsequent) task, or one or  more of both. It’s important to note, however, that there are also DAGs that have multiple parallel tasks - meaning no dependencies.
>> 2. Acyclic: No task can create data that goes on to reference itself. That could cause an infinite loop, which could give rise to a problem or two. There are no cycles in DAGs.
>> 3. Graph: In mathematics, a graph is finite set of nodes, with vertices connecting the nodes. In the context of data engineering, each node in a graph represents a task. All tasks are laid out in a clear structure, with discrete processes occurring at set points and transparent relationships with other tasks.

Security: Lack of regulation and standardization in the DLT can lead to risk for users and investors. By extension, DLT requires widespread adoption to be effective, and many industries and organizations may be hesitant to adopt new technologies due to these security concerns.

Immutable: All transactions are publicly viewable, it makes it difficult to have privacy for more sensitive types of transactions. It can also be more difficult to correct or reverse transactions in which errors or fraud has occurred.

Interoperability: Interoperability between different distributed ledger system for seamless data exchange and collaboration. However, achieving interoperability remains a complex task due to the lack of standardized protocols and compatibility issues between DLT platforms. Efforts are underway to develop interoperability solutions and bridge the gap between different networks.

Regulatory and legal frameworks: DLT disrupts existing systems and introduces new paradigms, regulatory frameworks must adapt in order to ensure consumer protection, privacy and security.

Complexity: Implementing and maintaining DLT systems can be complex and costly. Organizations may require significant technical expertise to do so effectively.

Privacy Concerns: DLT can provide transparency, it may not be suitable for applications that require complete data privacy. Striking the right balance between transparency and privacy is a challenge.

Initial Implementation Costs: The upfront costs of implementing DLT can be significant, and organizations may not see immediate returns on their investment

| Pros | Cons | 
|---|---|
| Spreads systematic risk around, minimizing the risk of a single point of failure | Is more complex compared to more traditional ledger solutions |
| Has greater security due to cryptographic algorithms | Often requires higher energy consumption for operation |
| Allows for transparency and visibility into operations | May have difficult scaling as more users/transactions occur |
| May prove to be more efficient due to smart contract automation | Still remains risky due to lack of regulation |
| Offers individuals with limited access to traditional systems potentially greater capabilities | May prove to be difficult to reverse fraudulent or erroneous activity. |

## Importance 
DLT is important as it has the potential to transform how information is recorded, stored and distributed. The importance is often cited across three pillars: security, transparency and accessibility

**Security**
Traditional ledger technology often has a central point of control with one single entity often in charge of the ledger. DLT makes the ledger more resilient to attacks and less vulnerable to system-wide failures. As DLT uses cryptographic algorithms to secure data, it also makes it more difficult to tamper with or forge records. DLT solution built on a consensus mechanism where all distributed ledgers must be in agreement about how a transaction is recorded. This validation of transactions allows greater trust among users and relinquishes power from any single individual.

**Transparency**
Centralized, traditional ledgers often restrict access to certain individual. Though this still holds value for **sensitive information**, there are many use cases where is is more beneficial for all when data and information is **broadly distributed** and **transparent**. Consider the example above of voting; having **digitally distributed, undisputable (un-disagreement)**, **verifiable** records of voting may enhance the believability of results. DLT is vital as it holds the theory of **reducing fraud** and **increasing accountability** in the long-term. Note how all transactions within a DLT system are able to be **viewed** by anyone with access to the DLT. The information may be “audited” by anyone any time, potentially demotivating bad actors from entering into nefarious activities in such a public sphere.

**Accessibility**
DLT offers the ability to store and **record transitions** using only a network connection as opposed to a very expensive connection such as bank account. Presents opportunities for **innovation** and the creation of new applications and use cases. In general, because of the ease of being to access DLT solutions, there are many positive implications on the broad public being able to communally access a shared network with often few complicated rules that cause long delays to meet prior to access.

## Differences between Distributed Ledgers and Blockchains
DLTs may take various forms, while a blockchain uses one specific infrastructure that uses a linear system of blocks to record and verify information.

| Distributed Ledger | Blockchain |
|:---|:----|
| Data can be chained, but not using “blocks” | Data is stored in chained “blocks” |
|Can be encrypted|Always encrypted|
|Private and permissioned, but can be permissionless|Generally public and permissionless, but some are permissioned|
|Can be immutable|Always immutable|

## Types of Distributed Ledgers
1. Private/Permissioned: There is no decentralization. Both the applications and the network nodes that operate them must **receive invitations** based on specific criteria or identification requirements. Any participant can be **expelled** from the network **without prior** notice.
2. Private/Permissionless: Involves **inviting applications** to join the network, with the possibility of removal at any time without notice. However, the **network nodes**, responsible for running these applications, can **join** and **contribute anonymously** and freely, often in exchange for the network’s native cryptocurrency.
3. Public//Permissioned: **Applications** can be** deployed **or removed from the network **without** the need to **notify** anyone, **disclose** their **identity**, or **meet specific application** criteria. The network nodes that operate these applications must be invited to participate.
4. Public/Permissionless: Highest degree of **decentralization**. Applications can be deployed or removed from the network without any notification, identity disclosure, or application criteria requirements. Similarly, network nodes can join and contribute freely and anonymously, typically in exchange for the network’s native cryptocurrency

## FAQ
1. What is Distributed Ledger Technology Used For?
Distributed ledger technology is used to securely store data so that is is unaltered, transparent, synchronized, and accurate. This can be extended to counting votes, recording transactions (financial or non-financial), or reporting activity across all users of a single DLT solution.
2. Is DLT better than blockchain
Each has a different purpose. Eg, blockchain is designed to be pubic and permissionless, while DLT is intended for private uses and can be permissioned or permissionless.
3. Do Banks Use DLT?
Banking ledgers have historically been centralized. However, DLT solutions allow for banking practices (ie, saving value, entering into transactions). If a financial institution has implemented a cryptocurrency, digital currency, or other means of recording on a digital ledger, that financial institution can theoretically enter into all of the same transactions as a traditional bank through the use of smart contracts. This can range from recording transactions, KYC information, or settling securities.
4. What is the difference between DLT and DeFi?
Decentralized Finance (DeFi) builds off of DLT solutions. DeFi allows for users to enter into familiar transactions offered by traditional banking solutions. However, these trades, loans or investments are made without a centralized intermediary.
