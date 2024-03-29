
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
