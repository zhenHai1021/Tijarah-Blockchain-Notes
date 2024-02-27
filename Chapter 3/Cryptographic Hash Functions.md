# Cryptography for Blockchain
A cryptographic hash function is a foundational element in the realm of **digital security** and blockchain technology. It is a special class of hash function designed to **secure** and manage **data integrity** in various cryptographic applications. 
A **CHF** is an algorithm that takes an input (or message) and return a **fixed-size** string of bytes. A CHF is a **single direction work**, making it extraordinary difficult to reverse in order to recreate the information used to make it. The output is typically a **‘hash’** or **‘digest’** that represents the input data. Key properties of these functions:

1. Deterministic: The same input will always produce the same hash output, meaning it wil produce the **same result** each time the **same input** is used. Eg, SHA-256 can generate a hashed output in **ms** with little computing power, but it also makes determining input difficult.
2. Quick computation: The hash function can process any size of data quickly and return a hash value in a consistent time frame
3. Preimage resistance: Given a hash value, it should be computationally infeasible to reconstruct the original input data (also known as one-way property) h = hash(m).
4. Second Preimage resistance: Weak collision resistance {hash(m1) = hash(m2)}
5. Small changes lead to significant differences: Even a tiny change in input data should produce an entirely different hash (avalanche effect)
> [!NOTE]
> AE: The desirable property of cryp algo, typically block ciphers and cryp hash functions, wherein if an input is changed slightly (eg, flipping a single bit), the output changes significantly (eg, half the output bits flip)
6. Collision Resistance: It should be extremely difficult to find two different inputs that produce the same hash output.

## Technical Details
1. **Hash Size**: The length of the hash output is critical. Eg, SHA-256, a commonly used cryptographic hash function in blockchain technology, produces a 256-bit (32-byte) output. This size ensures a vast range of possible hash values, contributing to collision resistance.
2. **Hash Functions**:  The most common hash function used in blockchain is SHA-256. SHA-256 is a secure hash function that is resistant to collision attacks.
3. **Digital Signatures**: The most common digital signature algorithm used in blockchain is ECDSA (Elliptic Curve Digital Signature Algorithm). ECDSA is a secure digital signature algorithm that is based on ECC (Elliptic Curve Cryptography).
4. **Algorithm Structure**: Most cryptographic hash functions follow a series of well-defined steps: message padding (to ensure that the input data is of a certain length), breaking the input into blocks, and processing these blocks through a series of mathematical operations.
5. **Public-key cryptography**: The most common public-key cryptography algorithm used in blockchain is RSA (Rivest-Shamir-Adleman). RSA is a secure public key cryptography algorithm that is based on the difficulty of factoring large numbers.
6. **Symmetric-key cryptography**: The most common symmetric-key cryptography algorithm used in blockchain is AES (Advanced Encryption Standard). AES is a secure symmetric-key cryptography used by US government.
7. **Merkle tree**: Merkle trees are constructed by hashing the data in a block and then hashing the resulting hash values, and so on, until a single hash value is obtained. This single hash value is called Merkle root. The Merkle root can be used to efficiently verify the integrity of all of the data in the block.
8. **Zero-knowledge proofs**: Zero-knowledge proofs are used in blockchain to create privacy-preserving transactions. Eg, zero-knowledge proofs can be used to allow a user to prove that they have a certain amount of money in account without revealing the account balance.

## Application in Blockchain
1. **Creating Block Hashes**: Each block in a blockchain has a unique hash, created from the block’s data (including the previous block’s hash). Any alteration in the block data changes its hash, affecting the entire chain, to ensure data integrity.
2. **Mining and Proof of Work**: Cryptographic hashes are central to mining in Proof of Work-based blockchains like Bitcoin.
> [!Tip]
> Miners must find a hash that is below a certain target, which requires computational work, thereby securing the network through energy and computational commitment.
4. **Securing transactions**: Hash functions are used to create digital signatures, which are used to authenticate the identity of a sender and to ensure the integrity of a message. Digital signatures are used secure transactions on the blockchain.
5. **Verifying the integrity of data**: Hash functions are used to create Merkle trees, which are used to efficiently verify the integrity of a large amount of data. 
6. **Creating unique identifiers**: Hash functions are used to create unique identifiers for blocks, transactions, and other data structures on the blockchain. These **Unique ID** are used to track and reference data on the blockchain.
7. **Creating privacy-preserving applications**: Hash functions are used to create privacy-preserving applications on the blockchain.
> [!Tip]
> Eg, hash functions can be used to create zk-proofs, which allow one party to prove to another party that they know a certain piece of information without revealing that information. Zk-proofs can be used to create privacy-preserving transactions on blockchain.
8. **Data Extraction and Retrieval**: Hashing converts object data into a integer value by using algorithms or functions. Once these items are located on such an object data map, queries can be filtered using a hash.
> [!Tip]
> Eg, developers or miners use hash tables to store data such as customer records and transitions as key and value pairs. Hash codes are then converted to integers of a specific size, whereas keys are used to identify data and are fed into the hash function.

## Example of Application Uses Hash Functions:
1. Bitcoin: Uses hash functions to secure transactions, verify the integrity of data, and create proof-of-work.
2. Ethereum: Ethereum uses hash functions to secure transactions, verify the integrity of data, and create unique identifiers for blocks and transactions.
3. Zcash: Zcash is a privacy-focused cryptocurrency that uses hash functions to create zk-proofs. Zero-knowledge proofs allow users to send and receive transactions without revealing their identity or the amount of money they are sending.
4. Filecoin: Filecoin is a decentralized file storage network that uses hash functions to create unique ID for files. UID are used to track and reference files on the Filecoin network.

## Resistance
<ol>
  <li>
    Collision Resistance = Second Preimage resistance: A good cryptographic hash function makes it nearly impossible to find <strong>two different inputs that produce the same output. </strong>The property is crucial for data integrity. 
    <ol>
      <li>
        Means it should be hard to find two different inputs of any length that result in the same hash. This property is also referred to as collision free hash function.
      </li>
      <li>
        If a hash function h, it is hard to find any two different inputs x and y such that h(x) = h(y).
      </li>
      <li>
        Since, hash function is compressed with fixed hash length, it is impossible for a hash function not to have collisions. This property of collision free only confirms that these collisions should be hard to find.
      </li>
      <li>
        This makes it very difficult for an attacker to find two input values with the same hash.
      </li>
      <li>
        Also, if a hash function is collision-resistant then it is second preimage resistant.
      </li>
    </ol>
  </li>
  <li>
    Preimage resistance: It is computationally unfeasilbe to reverse-engineer the original input from its hash output. This property is important for securing data and making it tamper-evident.
    <ol>
      <li>
        Means that it should be computationally hard to reverse a hash function
      </li>
      <li>
        If a hash function h produced a hash value z, then it should be a difficult process to find any input value x that hashes to z.
      </li>
      <li>
        Protects against an attacker that has a hash value and is trying to find the input
      </li>
    </ol>
  </li>
  <li>
    Second Preimage resistance = weak collision resistance: Property of a hash function that it is infeasible to find any second input that has the same output as a given input.
    <ol>
      <li>
        Means that given an input and its hash, it should be hard to find a different input with the same hash. 
      </li>
      <li>
        If a hash function h for an input x produces hash value h(x), then it should be difficult to find any other input value y such that h(y) = h(x)
      </li>
      <li>
        Protects against an attacker who has an input value and its hash, and wants to substitute different value as legitimate value in place of original input value
      </li>
    </ol>
  </li>
</ol>

## Benefirs of Hashing
1. Equality: Check the equality of two files. Without having to open two document files and compare them word for word, then calculated hash values of these files will tell the owner right away if they are different.
2. Validation: Used to validate the integrity of a file after it has been transferred from one location to another, most commonly in a file backup program such as SyncBack. A user can compare the hash values of both files to ensure that the transferred file is not corrupted. If they are the same, the transferred file is a duplicate.
3. 
