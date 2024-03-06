# Merkle Tree & Their Role in Blockchain

KEYWORDS:
Data Integrity, Efficiency, Merkle Data, hahses, data presence

Also known as hash trees, play a crucial role in the efficient and secure functioning of blockchain technology. A Merkle tree is a data structure used to efficiently **summarize** and **verify** the integrity of large sets of data.

![MR](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/8293d183-2bec-45fb-bb2a-2690b89da817)

**What is a Merkle Tree?**
A Merkle tree is a binary tree of hashes. At the **bottom layer (leaf nodes)**, **each node** represents the **hash of a block of data** (eg, a **transaction** in the blockchain). Each **non-leaf node** is a **hash of its two child nodes/previous hash**. This structure continues until there is a single hash at the top of the tree, known as `Merkle Root`.

![BD](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/1272986c-6bde-4c8c-8e57-eca669853e09)

Each **leaf node** is a **hash of transaction data**, and a **non-leaf node** is a **hash of its previous hashes**. 
> [!Tip]
> If transactions are in **odd numbers**, then the last hash will be repeated once to generate an even number of leaf nodes.

Merkle Tree/Hash Tree encodes blockchain data efficiently and securely, which enable quick verification and movement of data in P2P blockchain networks. Transactions on the blockchain have associated hashes. Hashes organized in a tree-like structure with parent-child relations. All **transaction hashes** in a block are hashed to **produce a Merkle Root**. An upside-down binary tree structure, with each node connecting to two nodes below. **Root hash** connects to hashes at level one, each connecting to **two hashes** at **leaf-level**. Structure continues depending on the **no of transactions hashes**.
> [!Tip]
> **Merkle root** is the only **one hash remains** of all the hashes of all the transactions that are part of a block in the blockchain network.

![MRH](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/e2bfe327-52f6-48fa-8fba-f479519f11fc)

**Technical Mechanics**
<ol>
  <li> 
    Creating a Merkle Tree
    <ul type="a">
      <li>
        Hashing Each Piece of Data: Each <strong>piece of data</strong> (like a <strong>transaction</strong> in blockchain) is <strong>hashed</strong> using a <strong>cryptographic hash function</strong> (eg, SHA-256). <strong>Unique hash value</strong> for each <strong>transaction</strong>.
      </li>
      <li>
        Pairing and Hashing Upwards: These hashes are then <strong>paired and hashed</strong> together, and the process continues recursively until a single hash remains - The Merkle Root.
      </li>
      <li>
        Building the Tree: The <strong>pairing and hashing</strong> process follows a hierarchical tree, where each level of the tree represents a round of hashing. At the <strong>bottom level</strong>, the <strong>individual transaction</strong> hashes serve as <strong>leaf nodes</strong>, and as they <strong>move up</strong> the tree, <strong>pairs of hashes</strong> are <strong>combined</strong> until <strong>reaching the root</strong>.
      </li>
    </ul>
  </li>
  <li>
    Verifying Data Using Merkle Trees
    <ul type="a">
      <li>
        To verify the integrity of any single piece of data, the entire blockchain does not need to be downloaded. Instead, the <strong>smallest chain of hashes</strong> is needed to link pieces of data to the Merkle Root.
      </li>
      <li>
        The chain of <strong>hashes</strong>, along with the Merkle Root, represent that the <strong>piece of data is indeed part</strong> of the tree <strong>without revealing</strong> the <strong>entire</strong> dataset.
      </li>
      <li>
        Efficient: Merkle trees enable efficient verification of transactions as the Merkle root needs to be stored in the <strong>block header</strong>. This allows nodes to <strong>quickly verify</strong> the integrity of transactions <strong>without</strong> needing to store the <strong>entire transaction history</strong>.
      </li>
    </ul>
  </li>
</ol>

**Benefits of Merkle Tree in Blockchain**
1. Data integrity: It can used to validate the data’s integrity effectively
2. Disk space: Takes up very **little disk space**. When a block is added to the blockchain, only the Merkle root needs to be stored.
3. Immutability: Ensuring immutability of the blockchain by making it impossible to alter data related to past transactions.
4. Information: Tiny information across networks, such that **MT can be broken down** into **small pieces of data** for verification. Instead of transmitting the entire transaction history.
5. Verification: Verifying the data’s integrity takes only a few moments. It reduces the amount of **memory** for verification. Since **Proof of Verification** does not require transferring **large amounts** of data over the network. Which enables **P2P** by **quickly verifying** transactions.
6. Transparency and traceability: Enhances the overall visibility of data within the network, fostering trust and accountability.
7. Tampering Detection: Check whether any transactions have been tampered with. Since transactions are **stored** in MT, which **stores the hash** of each node in the **top parent node**, any changes to the transaction details will propagate to the hashes in the **upper levels** and finally to the **Merkle root**. A miner can compare the **Merkle root in the header** with the **Merkle root stored in the data part** of the block and easily detect this manipulation.

**Cons of MT in Blockchain** [^1]
1. Overhead: MT require **additional computation** and **storage resource overheads** to create and verify the tree structure
2. Single point of failure: If the root node of the Merkle tree is compromised, the entire tree is compromised too.

**Role in Blockchain**
1. **Efficiency in Data Verification**: Merkle trees allow for efficient and secure verification of **large datasets** common in blockchain. They enable **quick** and lightweight **verification** of whether a **specific transaction** is included **in a block**.
2. **Security and Integrity**: By incorporating cryptographic hashing, MT help ensure the integrity of the blockchain data. Any **alteration** in a transaction would require **recomputation** of all **subsequent hashes up** to the Merkle Root, which is **computational impractical**.
3. Scalability: With enormous transaction amounts, Merkle Tree offers a way to scale efficiently. They reduce the **amount of data** needed to be transmitted, stored, and processed when **verifying transactions**. MT organizes and condenses transaction information, allowing nodes to **verify transactions** selectively **without overwhelming storage requirements**.
4. Proof of data: Providing that **tiny amounts of information** across the network is all that is **required** for a transaction **to be valid**. It enables the **tree** that **both ledger variations** are identical in terms of nominal computer power and network bandwidth.

![MR B](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/b747decf-a581-4c41-9ae3-dd102721ba5d)

**Technical Considerations**
1. Hash Function: The choice of the **hash function** is critical for the security of the Merkle Tree. Functions like **SHA-256** (used in Bitcoin) provide a better balancing speed and security.
2. Tree Structure: While binary trees are common, some implementations may use different structures (Like a Patricia tree in Ethereum) for specific optimization purposes.

![GENB](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/d506664a-ee3c-4c22-b623-90517b0a90f0)

Refer: Website Link [^2]
Each block has its **ID value**, which is the **hash of its header** fields. Another part is the **previous block ID**. Linking with the previous and next block ID, the blocks form a BLOCKCHAIN. By embedding Merkle Root, it makes an **immutable record** of transactions in the block.
Eg, block header contains:
- Merkle Root of all transactions in the block
- Nonce; a value changed in mining to find accepted blocks
- Previous block hash (blockID); linking this block to the previous block in chain (this previous hash is named parent)
- Timestamp; Time of mining (Creating the hash for) the block
- Block version; identifies support features and formats (also used to identify hash function in some blockchains)

These header fields are all **hashed together** to form the **block ID**. Making the block ID a hash of all header data makes it practically impossible to modify. Including Merkle root in the block ID.

---
# Reference
[^1]: https://www.charliedefi.com/dictionary/merkle-tree 
[^2]: https://medium.com/coinmonks/merkle-trees-concepts-and-use-cases-5da873702318
