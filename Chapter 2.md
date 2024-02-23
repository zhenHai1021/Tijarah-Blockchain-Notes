# Blockchain Architecture
## 1. What is A Private Blockchain?

**Permission** and **restrictive** Blockchain that operates in a **closed network**. Such blockchain is often generally used within an organization where only particular members are **participants** of a Blockchain network. A private blockchain network requires an **invitation** or **set of rules** established, which must be **approved** by the network founder. This limits who is authorized to engage in the network, by condition participants must get an **invitation or authorization**. Private blockchain is suitable for **enterprises** and businesses that aim for internal uses, when a company wants to benefit from blockchain qualities without exposing its network to the public. Sector including Digital identification, supply chain, banking sector or, healthcare data cases. 

Pros </br>
**Enhanced privacy and confidentiality**: Restrict access to authorized participants, ensuring sensitive information is not visible to the public.

**Greater control**: Participants in a private sector have more control over the consensus mechanism, governance, and the overall rules of the network. This allows for faster decision making and adaption to specific business requirements.

**Scalable and Efficiency**: More easily scaled to meet specific business needs. Especially growing transaction volumes throughput and faster confirmation compared to the public. It is beneficial for businesses that require rapid and enormous volume transactions.

**Reduced Energy consumption and Low Cost**: Use consensus mechanisms that are less energy-intensive compared to the Proof-of-Work that is often used by public Blockchain. Advantageous for the organization aiming to minimize the environmental impact. Fewer participants, transaction costs can be lower compared to public Blockchains, dealing with high volume of transactions.

**Compliance with Regulations**: Designed to comply with specific regulations. Sectors such as finance and healthcare, where strict adherence to rules is essential.

**Customization and faster adoption**: Flexible to customize according to their specific needs. More palatable (acceptable) for traditional businesses as allow to experiment with Blockchain technology without fully exposing their operations to the public, with unique requirements that may not be met by public Blockchains. Seamlessly integrate with existing system and databases as well. Smoother transition for business incorporating Blockchain technology into their operations.

Cons </br>
**Centralization Concerns**: Limited number of participants controlling the network, potentially leading to concentration of power.

**Limited Transparency**: Restrict access to certain information, reducing the transparency compared to public Blockchains, where stakeholders require visibility into all transactions and activities.

**Security Risks**: private B heavily relies on the trustworthiness of the participating entities, if a participant is compromised, it can jeopardize the overall security of the network.

**Interoperability**: May face issues in interoperability with other blockchain networks, therefore it may hinder seamless communication and data exchange between different networks.

**Dependency Single Entity**: often depend on a single organization to maintain/operate the network. May face entity single point of failure from the entire blockchain network. Thus, collusion could lead to manipulative practices or biased decision making within the network. 

**Cost and Resources**: setting up and maintaining a private Blockchain can be costful for smaller organizations

**Limited Tokenization Opportunities**: Limitations in creating and managing tokens or cryptocurrencies. Potential for developing and implementing tokenization-based applications and business models.

**Governance**: Private blockchains may be controlled by a select group, leading to potential conflicts of interest. It may hinder decision-making processes and result in suboptimal outcomes for the networks.

Private blockchain is more **centralized** due to a single authority maintaining the network. Means that private blockchain provide **greater control** and **privacy to the network’s owners** since only authorized parties can access and participate in them. These networks are **faster** than public since they do not require solving complex algorithms before adding new transactions.

## 2. What is A Public Blockchain?
**Permissionless, non-restrictive, distributed ledger** system, anyone who is connected to the internet can join the network. The basic use is for exchanging cryptocurrencies and mining. It also maintains trust among the whole **community** of users in the network and feels incentivized to work towards the **public network**. Eg, Bitcoin, Ethereum and Solana.

Pros </br>
**Decentralization and Transparency**: Decentralized network of nodes, resistant to censorship or control by a single entity. Ensuring a more democratic and inclusive system. All transactions on a public Blockchain are visible to anyone in the network. Foster trust among participants from verifying transactions and the overall state of the network.

**Security**: Often use consensus mechanisms such as Proof of Work or Proof of Stake, which is difficult for hackers to alter transactions history or compromise the security of a network.

**Immutability**: Once a block is added to the Blockchain, it is practically impossible to alter its content. This ensures the integrity of transaction history and builds trust among users.

**Interoperability and Accessible**: Can be accessed and used by anyone across different platforms and applications. Accessible to anyone with an internet connection, providing financial services and opportunities to anyone may be excluded from the financial institutions.

**Tokenization**: Allows for the representation of various assets on the Blockchain, enabling efficient and secure transfer of ownership. Token rewards to encourage participants (miners/validators) to contribute to the network’s security.

**Trustless transactions**: Trust the underlying protocol and the consensus mechanism, ensure the validity of transactions without the need for intermediaries or government control.

Cons </br>
**Scalability**: Large no. of transactions to be handled, result in slower transaction processing times and higher fees during network congestion.

**Energy Consumption and Unpredictable cost**: Proof-of-work consensus, requires significant computational power, leading to higher energy consumption, not only raises environmental concerns but also makes the operation of the network expensive. Unpredictable transaction fees. Hard to estimate cost of transaction accurately, leading to unpredictability in expenses.

**Privacy Concerns**: Public blockchain are transparent, since all the transactions are visible to anyone. Lack of privacy can be a burden for users who want to keep confidential their financial activities.

**Regulatory**: Governments and regulators may find it hard to monitor and control activities on public blockchain. This may lead to legal uncertainties, hindering broader adoption and acceptance.

**Immutability dilemma**: Once a transaction is recorded, posing challenges in correcting mistakes. 

**Lack of Governance**: Often lack formal governance structures. Therefore, decision-making process and protocol upgrades may become contentious (heated argument), potentially leading to forks and divisions in the community.

**User-friendly**: Complex for non-technical users or non-knowledge blockchain users. This limits the widespread adoption of Blockchain technology.

**Smart contract risks**: Smart contracts are not immune to bugs or vulnerabilities. Flaws in smart contracts can lead to significant financial losses. 

Anyone can join and participate in a public blockchain network. To attract more participants to join the network, the network usually has an incentive system. One of the cons, is the amount of **computational/processing power** required to keep a distributed ledger running at a wide scale. To obtain consensus, each node in a network must solve a **sophisticated**, resource-intensive cryptographic challenge known as proof-of-work (PoW) to ensure everyone is on the same page. Another problem arise, from its openness, which implies minor to zero transaction privacy and only supports a fundamental of security.

## 3. What is the difference between private vs public blockchain vs consortium?
| Aspect | Private| Public | Consortium |
|---|---|---|--|
| Access Control | Restricted access | Open to Anyone | Limited Access |
||Access is restricted to a specific group of participants who are typically known and permissioned by a central authority. This ensures a higher level of trust among participants. The permissioned nature allows for faster transactions and lower latency.|Open to anyone without permission. Participants can join the network pseudonymously, and transactions are validated by a consensus mechanism that doesn’t rely on trust among participants. This openness promotes decentralization but lead to slower transaction speeds.| Access is limited to a predefined group of participants. While not entirely open, it is more inclusive than a private Blockchain. The consortium determines and manages permissions.|
| Participants | Known and permissioned | Anonymous and open |Known and permissioned |
||Known as entities, mostly verified. This identity verification enhances trust and allows for more straightforward governance. |Participants are pseudonymous, identified by cryptographic addresses. Anyone can participate, and trust is established through the consensus mechanism and transparency.|Participants are known and permissioned by the consortium. Similar to private Blockchain.|
|Permissionless?|No. Invited users to read/write only|Yes. Anyone |No. Approved participants|
|Consensus Mechanism|Faster, less energy-intensive|Slower, energy-intensive|Variable, depends on consensus model|
|||Relies on more time-consuming and energy-intensive consensus mechanisms such as Proof-of-Work (Bitcoin) or Proof of Stake (Ethereum). Designed to achieve decentralized consensus in an open network.|Vary based on the specific needs and goals of the consortium. |
|Decentralization|More centralized|Fully decentralized|Intermediate level|
||More centralized, as control as is often central authority or a limited number of trusted participants.|Fully decentralized, with no central authority. Decision-making and validation of transactions are distributed across a network of nodes, providing high level of trust and censorship resistance.|More decentralized than private blockchain, still less decentralized than public blockchains|
|Ownership|Single Entity|Nobody|Multiple entities|
|Speed and Scalability|Faster and scalable|Slower and less scalable|Moderate speed and scalability|
||Faster and more scalable due to the known participants. Limited of nodes facilitates quicker consensus and validation.|Slower and less scalable from increasing number of participants. Therefore, adding more complex in achieving consensus, leading to longer transaction times. |Moderate speed and scalability. Not as fast as private blockchain. More efficient than a fully public Blockchain.|
|Example|Hyperledger Fabric, Corda|Bitcoin, Ethereum|Quorum, R3 Corda|

##  4. What is A Consortium Blockchain?
Consortium blockchains (Federated Blockchains) are the union of a **public and private** blockchain that is partly decentralized. ==There are some **controlling nodes** to verify and validate transactions or blocks. The **miner blocks** are valid only when approved and signed by these controlling nodes. The data or transaction details can be **open source**, like public blockchains, but the nodes can **verify** and validate transactions instead of a specific individual or a single company==. In the consortium blockchain, there is **more than one** central in-charge, which means that one organization is involved who provides access to pre-selected nodes for reading, writing and auditing the Blockchain. Since there is no single authority governing the control, it maintains decentralized nature. 

Pros </br>
**Shared control bring Resilience**: Multiple organizations/entities control the network. This shared control fosters collaboration and allows for collective decision making, suitable for industries where multiple stakeholders ask for collaboration. The shared control enhances the network. Even if one participant experiences issues, the overall integrity of Blockchain can be maintained through the consensus of the remaining members

**Enhanced privacy and Trust**: Not fully private as private Blockchains, offer a higher level of privacy compared to public Blockchains. Participants have a degree of control over who can join the network, ensuring a level of confidentiality. Trustworthiness leverage a shared and distributed ledger, promoting trust among participants. Where transparency and accountability in supply chain traceability or collaborative research.

**Efficiency and Speed**: Higher efficiency and faster transaction processing compared to public Blockchains. Where a moderate level of decentralization is desired without used up performance.

**Cost Savings**: Cost for infrastructure and maintenance are shared, participants can save up cost compared to private. 

**Interoperability**: Facilitate interoperability between different organizations within the network. This can streamline processes, improve communication among the consortium members. 

**Customization and flexibility**: Allow for customization to meet the specific needs of participants. Aid in industries with diverse requirements such as supply chain management or healthcare.

**Compliance with Regulations**: Comply with industry standards, providing a balance between regulatory requirements and the benefits of technology. 

**Gradual Adoption**: Allows them to collaborate with selected partners or stakeholders before consideration.

Cons </br>
**Limited decentralization**: More decentralized than private blockchains, still involve a restricted group of participants. 

**Complex governance structures**: Require complex governance structures to manage decision making among the participating organizations. Therefore developing and maintaining effective governance can be challenging, potentially leading to conflicts and delays in decision-making.

**Interoperability**: Similar to private blockchains, face difficulties in interoperability with other Blockchain networks. Limited interoperability can hinder the exchange of data and assets between consortiums of networks.

**Security risks from member actions**: Security relies on the trustworthiness of its members. 

**Scalability**: Might encounter scalability issues, from the increasing number of participants and transactions. Results in slower transaction processing times and increased costs during high period activity.

**Complex integration processes**: Integrating existing systems and processes into a consortium Blockchain can be challenging. The complexity of integration may slow down adoption and implementation.

**Cost sharing and funding issues**: Allocating sharing costs among consortium members can be a complex task. 

A consortium blockchain is a hybrid form of **public and private blockchains**. Instead of an open system in which anybody can validate blocks or a close system in which only a single part selects block producers, a consortium chain employs a small number of equally powerful parties as validators. A consortium blockchain would be useful where several companies operate in the same industry and need a single platform to conduct transactions or transmit information. Compared to a public blockchain network, consortium is more secure, scalable and efficient. It provides access controls, like private blockchain. However, consortium blockchain is less transparent, and the member node still can be compromised, and the blockchain’s own rules can make the network unusable.

## 5. Is Bitcoin/Ethereum a Public or a Private Blockchain?
**Bitcoin** is a public blockchain that anyone can observe and use as it is built with open source computing codes.
While private blockchain do not allow for **anonymity**, the Bitcoin blockchain does. Anyone, Eg, can purchase and trade Bitcoin without revealing their **identity**. Ensuring everyone is treated equally. Because of Bitcoin’s **decentralized** nature, all transactions can be monitored **transparently** via personal nodes or blockchain explorers, which allow anyone to witness transactions in real time. Each node maintains its copy of the chain, which is updated as new blocks are confirmed. 

**Ethereum** is a public blockchain that anyone can add, but not altered. 
Anyone can join the network, read data, perform transactions, and participate in the consensus process. If someone wanted to alter any of the information or cheat the system, they need to perform so on the majority of computers on the network. Ethereum operates without a central authority, secured by **mechanisms** such as Proof-of-Work or Proof-of-Stake. Same as Bitcoins, Ethereum’s decentralized nature, all transactions can be **visible** to anyone on the networks. Besides, Ethereum supports decentralized execution of smart contracts.

## 6. How does a private blockchain work?
A private blockchain is a sort of blockchain technology in which a **single entity** controls the network. The entire network is shared by the coalition (partnership) of organizations in a private permissioned blockchain. The **network operator** can set up user and node permissions and roles, such as who can participate in the consensus process, who can read and write to the ledger and how blockchain nodes are distributed around the network.

Steps involved in the working of a private blockchain network include:

1. Users of the network and their rights are not equal and are determined by their role in the consortium.

2. Different categories of data can only be accessed by users who have been granted authorization.

3. The technique of access is determined by the network participants’ regulations.

## 7. How does a public blockchain work?
The public blockchain network is a blockchain network that **anybody** can **join** at any time. Anyone with internet connectivity can join a blockchain platform and become an authorized node, making public blockchain **non-restrictive and permissionless**. This user has access to current and **historical records** and the ability to perform **mining operations**, which are sophisticated calculations required to **verify** transactions and add them to the ledger. No valid record or transaction **altered/modified** on the network, and because the source code is usually **open-source**, anyone can **verify/witness** the transaction, uncover errors and other fixes. To engage with the public blockchain, each participant creates an account and connects it to a node. Consider it a bank account for sending and receiving transactions. The decision to add a transaction to the chain on a public blockchain is decided by consensus. This means that the transaction must be accepted by the **majority of “nodes”** (or computers in the network). The people who own the machines in the network are rewarded for confirming transactions. “Proof-of-work (PoW)” is the term for this procedure.

## 8. How does a consortium blockchain work?
The consortium blockchain network is a blockchain network in which numerous organizations manage the platform. Instead of starting from scratch, newcomers might join a consortium and help to **manage** the developed structure and **shared data**. At the same time, by working together to solve **shared puzzles/challenges**, businesses can save money and time on development. Finally, the **coordination** of actions and the **sharing of expertise** helps to avoid duplication by allowing **diverse subjects** to **share duties** rather than **duplicate labor**. In a consortium blockchain, there are fewer known participants. It ensures **low latency** and **excellent performance** as it is frequently a voting-based system. Every node can **write and read** transactions, but neither may **add** a block. Every node (or supermajority) must confirm that block to do so. The block cannot be added if this rule is not met.

## 9. What is the key difference between Private and Public Blockchain?
**Public** blockchains are decentralized and rely on **consensus** mechanisms such as Proof-of-work (PoW) or Proof-of-Stake (PoS) to validate transactions and add new blocks to the chain. Private blockchains, on the other hand, can be **centralized or decentralized**, depending on the design and use case. In some cases, private blockchains may have a **central authority** that controls the network, which can limit the benefits of decentralization. On the other hand, private blockchain are designed for **closed networks** where participants are **pre-approved** and require **permission** to access the network. Private blockchain are typically used by enterprises and organizations that want to keep their data and transactions private and secure. 

From the perspective of the level of **transparency**. Public blockchains are designed to be fully **transparent**, meaning that anyone can **view** the data and transactions on the blockchain. Private blockchain, on the other hand, can be designed with **varying levels** of transparency, **depending** on the **use case** and requirements of the participants. Same as their **openness and accessibility**. Public blockchains are **open to anyone** and are fully transparent, while private blockchains are **restricted** to **approved participants** and may have varying levels of transparency.

## 10. Ethereum on differences public, private and consortium.
Instead of having a fully public and uncontrolled network and state machine secured by cryptoeconomics (eg. PoW, PoS), it is also possible to create a system where access permissions are more tightly controlled, with rights to modify or even read the blockchain state restricted to a few users, while still maintaining many kinds of partial guarantees of authenticity and decentralization that blockchains provide. 

Public Blockchain </br>
Anyone in the world can **read, send and see** the transactions if they are valid, and anyone legible to participate in the **consensus process**, the process for determining what blocks get **added** to the chain and what the **current state** is. As a substitute for centralized or quasi-centralized trust, public blockchain are secured by **cryptoeconomics**, the combination of **economic incentives** and **cryptographic verification** using **mechanisms **such as PoW or PoS, following a ==general principle that the degree to which someone can have an influence in the consensus process is proportional to the quantity of economic resources that are bearable==. These blockchain are called “Fully Blockchain”.

Fully Private Blockchain </br>
A fully private blockchain where permissions are kept **centralized** to one organization. **Read** permissions may be **public or restricted**. Likely applications include **database management**, auditing, etc internal to a **single company**, and so public readability may not be necessary in many cases at all, though in other cases public auditability is desired.

Consortium Blockchain </br>
A consortium blockchain is a blockchain where the consensus process is controlled by a pre-selected set of nodes. Eg, imagine a consortium of 15 financial institutions, each of which operates a node and of which 10 must sign every block in order for the block to be valid. The right to read the blockchain may be public, or restricted to the participants, and there are also hybrid routes such as the root hashes of the blocks being public together with an API that allows members of the public to make a limited number of queries and get back cryptographic proofs of some parts of the blockchain state. These blockchains are called “Partially Decentralized”.
</br>
In general, the former provides a hybrid between the **“low-trust”** provided by **public blockchains** and the **“single highly-trusted entity”** model of **private blockchain**, whereas the latter can be more accurately described as a traditional centralized system with a degree of cryptographic auditability attached. However, to some degree there is good reason for the **focus** on **consortium over private**: the fundamental value of blockchain in a fully private context, aside from the replicated state machine functionality, is cryptographic authentication, and there is no reason to believe that the optimal format of such authentication provision should consist of a series of hash-linked data packets containing Merkle tree roots; generalized zero knowledge proof technology provides a much broader array of possibilities about the kinds of cryptographic assurances that applications can provide their users. 

## 11. Ethereum on Public vs Private
### a. Private
### i. 
The consortium running a private blockchain can easily change the rules of a blockchain, revert transactions, modify balance. In some cases, eg. national land registries, this functionality is necessary; there is no way a system would be allowed exist where `Pirate Robert` can have legal ownership rights over a plainly visible piece of land, and so an attempt to create government-uncontrollable land registry would in practice devolve (pass down) into one that is not recognized by the government itself. Of course, one can argue that one can do this on public blockchain by the government a backdoor key to a contract; the counter-argument to that is that such an approach is essentially Rube alternative to the more efficient route of having a private blockchain, although there is in turn a partial counter-argument to that later on
### ii.
The validators are known, so any risk of 51% attack arising from some miner collusion in China does not apply.
### iii. 
Transactions are cheaper, since they only need to be verified by a few nodes that can be trusted to have very high processing power, and do not need to be verified by 10k laptops. This is vital, as public blockchains tend to have transaction fees >$0.01 per tax, yet to not that in may change in the long term with scalable blockchain that promises to bring public-blockchain cost down to within 1 or 2 orders of magnitude of an optimally efficient private blockchain.
### iv. 
Nodes can be trusted to be very well-connected, and faults can quickly fixed by manual intervention, allowing the use of consensus algo which offer finality after much shorter block times. Improvements like Ethereum 1.0’s uncle concept and later PoS, can bring public blockchain much closer to the “instant confirmation” ideal (eg. offering total finality after 15 seconds, rather than 99.999% finality after two hours as does Bitcoin), but even still private blockchain faster and the latency difference will never disappear as unfortunately the speed of light does not increase by 2x every 2 years by Moore’s law.
### v. 
If read permissions are restricted, private blockchain can provide a greater level of, well, privacy.

### b. Public
### i.
Provide a way to protect the users of an application from the developers, establishing that there are certain things that even the developers of an application have no authority to do. A major category of pressure that application developers are at risk of is that by governments, so “censorship resistance” ties strongly into this kind of argument.
### ii. 
Public blockchains are open, and therefore are likely to be used by very many entities and gain some network effects. Eg, consider the case of domain name. If A wants to sell a domain to B, there is the standard conterparty risk problem that needs to be solved; Is A sends first, B may not sending money, and if B sends first then A might not send the domain. To solve this problem, Ethereum have centralized escrow intermediaries, but these charge fees of 3 - 6%. However, if we have a domain name system on a blockchain, and a currency on the same blockchain, then we can cut costs to near-zero with smart contract: A can send the domain to a program which immediately sends it to the first person to send the program money, and the program is trusted because it runs on a public blockchain. Note that in order for this to work efficiently, two completely heterogeneous asset classes from completely different industries must be on the same database, not a situation which can be easily happen with private ledgers. Another similar example in this category is land registries and title insurance, although it is important to note that another route to interoperability is to have private chain that the public chain can verify, btcrelay-style and perform transactions cross chain.

## FAQ
1. What is the common type of Blockchain?
   - The most common type of Blockchain is the public Blockchain.
   - It is widely recognized, open to anyone, and exemplified by cryptocurrencies like Bitcoin and Ethereum.
     
2. What are the 3 most important components for a Blockchain?
   - Decentralized Network: Operating without a central authority, ensuring a democratic and inclusive system
   - Consensus Mechanism: A method for nodes to agree on the state of the Blockchain, such as Proof of Work or Proof of Stake
   - Distributed Ledger: A ledger that is duplicated across the entire network, ensuring transparency and security
     
3. What is the best type of Blockchain?
   - Determining the “best” type of Blockchain depends on specific needs and use cases
   - Public Blockchains offer global accessibility, transparency, and trustless transactions but face challenges like scalability and energy consumption
   - Private Blockchain provide enhanced privacy, control, and efficiency but may have issues like centralization and limited transparency.
   - Consortium Blockchains offer shared control, improved privacy, and efficiency, balancing characteristics of both public and private Blockchains.
     
4. What are some examples of places where a private blockchain could be implemented? Wide-ranging applications across industries such as supply chain management, healthcare, finance, and government.
   - In supply chain management, they enhance transparency, traceability, and collaboration among participants, ensuring authenticity and reducing delays. Participants, such as manufacturers, suppliers, and distributors, can securely share information, track inventory, verify suppliers authenticity, and streamline processes through a private blockchain network.
   - In healthcare, private blockchains securely store and share patient records, improving data integrity and facilitating interoperability. Medical institutions, insurance providers, and patients can securely share and access sensitive patient records, ensure data integrity and streamline processes like insurance claims and medical research.
   - In financial industry, private blockchains expedite cross-border transactions, streamline settlements, and enhance regulatory compliance. Governments can leverage private blockchains for secure voting systems, transparent land registries, voting system,and efficient public service delivery.
     
5. What are some examples of places where consortium blockchain exist.
   
XRP, Ripple’s native token, is among the cryptocurrencies. Notable companies using Ripple include Bank of America, PNC Bank, Santander, American Express, and etc

Hyperledger is another notable consortium blockchain launched by the Linux Foundation in 2015. The project aims to unite companies to develop blockchains and other distributed ledgers to benefits multiple industries, including fintech and supply chains. Additionally, Hyperledger serve as an incubator of codebases from companies like Intel, Digital Asset, and Blockstream. Companies leveraging Hyperledger include Cisco, Fujitsu, Hitachi and more

Another example is the Energy Web Foundation (EWF), a non-profit organization dedicated to providing blockchain-based solutions for the international energy industry. These solutions are intended to enhance company performance, harness clean energy, improve inter-company cooperation, secure stakeholders’ data, and reduce costs. The foundation introduced the open-source decentralized platform Energy Web Chain in 2017.

6. What is a private token from a private blockchain?

A private token is a type of cryptocurrency or digital asset that is issued and managed on a private blockchain. Unlike public cryptocurrencies, which can be bought, sold, and traded freely, private tokens are usually restricted to a close network or participants, such as a company or consortium, and are often used for specific business purposes, like tracking supply chain data or rewarding customer loyalty. PTs are often used in enterprise, where organizations want to benefit from the security and transparency while retaining control over who can access and transact with the tokens.

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
      As Bitcoin grained traction, it become evident that the underlying blockchain technology could be adapted for applications beyond cryptocurrency. In 2015, Ethereum, created by Vitalik Buterin, introduced the concept of smart contracts. These self-executing agreements further expanded the scope of DLT, enabling programmable, automated, and trustless interactions. The programs used **automation** and **data encryption** techniques to **verify database transactions** or **changes** in the **database’s state**. This is called **consensus** - the act of **automated majority agreement** on **transaction validity**, where a transaction is simply a change made to a database’s state. 
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
| ====| ====|
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
|==|==|
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

# Differences between Bitcoin and Ethereum
![Differences between Bitcoin and Etherem](/assets/images/Diff BNE (1).png "Diff Bitcoin and Ether")

