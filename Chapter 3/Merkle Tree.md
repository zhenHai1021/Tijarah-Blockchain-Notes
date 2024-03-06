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
        Hashing Each Piece of Data: Each **piece of data** (like a **transaction** in blockchain) is **hashed** using a **cryptographic hash function** (eg, SHA-256). **Unique hash value** for each **transaction**.
      </li>
      <li>
        Pairing and Hashing Upwards: These hashes are then **paired and hashed** together, and the process continues recursively until a single hash remains - The Merkle Root.
      </li>
      <li>
        Building the Tree: The **pairing and hashing** process follows a hierarchical tree, where each level of the tree represents a round of hashing. At the **bottom level**, the **individual transaction** hashes serve as **leaf nodes**, and as they **move up** the tree, **pairs of hashes** are **combined** until **reaching the root**.
      </li>
    </ul>
  </li>
  <li>
    Verifying Data Using Merkle Trees
    <ul type="a">
      <li>
        To verify the integrity of any single piece of data, the entire blockchain does not need to be downloaded. Instead, the **smallest chain of hashes** is needed to link pieces of data to the Merkle Root.
      </li>
      <li>
        The chain of **hashes**, along with the Merkle Root, represent that the **piece of data is indeed part** of the tree **without revealing** the **entire** dataset.
      </li>
    </ul>
  </li>
</ol>

