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
2. Validation: Used to validate the integrity of a file after it has been transferred from one location to another, most commonly in a file backup program such as SyncBack.
> [!Tip]
> A user can compare the hash values of both files to ensure that the transferred file is not corrupted. If they are the same, the transferred file is a duplicate.
4. Immutable: An encrypted file may sometimes be configured never to change the file size or the latest update data and time (Eg, virtual driver container files).
> [!Tip]
> It would be impossible to distinguish if two similar files are distinct or not at first glance (first look), but the hash values would easily distinguish these files apart if they are.

## Hash Function
Hash function is a mathematical function that converts a numerical input value into another compressed numerical value. The input to the hash function of arbitrary length but output is always of fixed length. Moreover, hashes cannot be used to “reverse-engineer” the input from the hashed output since hash functions are “One Way”.
> Values returned by a hash function are called message digest or simply hash values.

![hash_functions](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/d93db65d-4265-4826-ab61-465bf299ae2c)

**Fixed Length Output (Hash Value)**
- Hash function converts data of arbitrary length to a fixed length. Process refer to as “hashing the data”
- Hash is much smaller than input data, hence hash function refer "compression functions"
- Since a hash is a smaller representation of a larger data, refer to "digest"
- Hash function with n bit output is referred to as n-bit hash function. Popular hash functions generate values between 160 and 512 bits.

**Efficiency of Operation**
- Computationally hash functions are much faster than a symmetric encryption


## How Hashes Work
A cryptographic hash function combines the message-passing capabilities of hash functions with security properties. Hash functions are algorithms that determine how information is encrypted. If one bit anywhere in the original data been changed, the entire hash value changes.
> [!Tip]
> Eg, Secure Hashing Algorithm 256 (SHA-256) goes through a process to encrypt the input it receives by:
- Converting it to binary
- Creating hash values
- Initializing constants
- Chunking data into bits
- Creating a message schedule
- Running a compression loop
- Modifying the final values
> [!IMPORTANT]
> Using SHA-256, the word “Hello” will produce an output that is the same number of characters (64) as “Hello World” and “Hellos”. The hash will be significantly different for all three.

## Hashing and Cryptocurrencies
The backbone of a cryptocurrency is the blockchain, which is a globally distributed ledger formed by linked together individual blocks of transaction data through hashing. The blockchain only contains validated transactions, which prevents **fraudulent transactions** and **double spending** of the currency such as **Cryptocurrency mining** and validation involves working with this hash.

Solving a cryptocurrency hash **starts** by using the **block header** from the **previous block** as **input** and generating a **hash**. Each block header contains a **version number**, **a timestamp**, the hash used in the previous block, the hash of the Merkle root, the nonce, and the target hash.

The goal is to generate **a HASH** that is **equal to or less** than the **network’s target hash**. In the hash is a sequence of numbers called the **nonce**, or number **used once**. The mining program focuses on the nonce, which starts at zero in the first attempt. If the attempt fails, the program adds 1 to the nonce, and generates the hash again. It adds 1 to each failed attempt **until** generating a hash **less than or equal** to the **target hash**, then is the solution.

The miner may potentially test a **large number of nonce** options before getting it right. **The greater the difficulty**, a measure of **how hard it is to create a hash** that meets the requirement of the target hash, the longer to take to generate a solution.

## Design of Hashing Algorithms
At the heart of a hashing is a mathematical function that operates on two fixed-size blocks of data to create a hash code. This hash function forms the part of the hashing algorithm.
The size of each data block varies depending on the algorithm. Typically the block sizes are from **128 bits to 512 bits**.

![Hash algorithm](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/659a1153-9c3f-4af1-b2df-2dac2ad6812b)

Hashing also involves round of aboce hash f(x) like a block cipher. Each round takes an input of a fixed size, typically a combincation of the most recent message block and the output of the last round.

This process is repeated for as many rounds as are required to hash the entire message.
Schematic of hashing algo as example below:
![Hash algorithm (1)](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/ae08715d-352c-4412-a3de-e8e9795557c1)

Since, The hash value of first message block becomes an input to the second hash operation, output of which alters the result of the third operation. This effect is called "Avalanche Effect" of hashing.
> [!Note]
> *Avalanche effect results in different hash values for two messages that differ by even a single bit of data.
> [!WARNING]
> **Hash function** generates a hash code by operating on two blocks or fixed-length binary data.
> **Hashing algorithm** is a process for using the hash function, specifying how the message will be broken up and how the results from previous message blocks are chained together.

## Popular Hash Functions
**Message Digest (MD)**: Message Digest is used to ensure the integrity of a message transmitted over an insecure channel. MD5 was the most popular and widely used hash function for quite some years.
- The MD family comprises of hash functions MD2, MD4, MD5 and MD6. That was adopted as Internet Standard RFC 1321. It is a **128-bit** hash function
- MD5 digests have been widely used in the software world to provide assurance about **integrity of transferred file**.
> [!Tip]
> Eg, file servers often provide a pre-computed MD5 checksum for the files, so that a user can compare the checksum of the downloaded file to it.
- In 2004, collisions were found in MD5. An **analytical attack** was reported to be successful only in an hour using **computer cluster**. This collision attack resulted in compromised MD5 and hence it is no longer recommended for use.

![DM](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/72ed613d-7dfa-490e-a14d-e2225717b667)

Assume, Alice sent a message and digest pair to Bob. To check the integrity of message Bob runs the cryptographic hash function on the received message and gets a new digest. Now, Bob will comparer the new digest and the digest sent by Alice. If both are the same then Bob is sure that the ori message is not changed.
- The digest should be **unchanged** during the **transmission**
- **One way function**, which is practically infeasible to invert. This cryp hash function takes a **message** of variable length as **input** and creates  a **digest/hash/fingerprint** of fixed length, which is used to verify the integrity of the message.
- Digest is **encrypted** with the **sender's private key**. Now this digest is called **digital signature**. Which can be only **decrypted** by the **receiver** who **has** the **sender's public key**. Now the receiver can authenticate the sender and also verify the integrity of the sent message.

**Secure Hash Function (SHA)**: Family of SHA comprise of four algorithms; SHA-0, SHA-1, SHA-2, and SHA-3. Though from same family, but there are structurally different.
- The original version is SHA-0, a **160-bit** hash function. Few weaknesses and not popular. Later in 1995, SHA-1 was designed to correct alleged weaknesses of SHA-0.
- SHA-1 is the most widely used of the existing SHA hash functions. It is employed in several widely used applications and protocols including **Secure Socket Layer (SSL)** security.
- In 2005, a method was found for uncovering collisions for SHA-1 within practical time frame making long-term employability of SHA-1.
- SHA-2 family has four SHA variants, SHA-224, SHA-256, SHA-384, and SHA-512, SHA-512/224, and SHA-512//256 depending up on **number of bits** in their **hash value**. No successful attacks reported on SHA-2 hash function.
- Though SHA-2 is a strong hash function. Though significantly different, its basic design is still follows design of SHA-1. Hence, NIST called for new competitive hash function designs.
- In OCT 2012, the NIST chose **Keccak algorithm** as the **new SHA-3** standard. Keccak offers many benefits, such as **efficient performance** and **better resistance **for attack.

> [!Note]
> *Keccak is a sponge function, means that it takes an **input message** of **arbitrary length** and produces a **fixed-length output**. It is resistant to collision attack, means that it is **difficult** to find **two different messages** that produce the **same hash** value. Also resistant to **Preimage attacks**, which means that it is **difficult** to find a **message** that produces a **given hash value**.
The sponge function consists of two parts: The absorber and the squeezer.
>> The absorber takes the **input message** and **absorbs** it into a **state**, which is represented as a **5x5 matrix** of 64-bit words. The absorber is designed to be highly efficient and can process large amounts of data quickly.
>> Once the absorber has **finished processing** the **input message**, the squeezer is used to **extract the output hash**. **The squeezer** is used to extract the **output hash**. The squeezer takes the **state and outputs** a **fixed-length bit string**. The length of the output hash can be varied, depends on the desired security level.

**Characteristic of the SHA-256**
![SHA-256](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/dfe8f895-c2ae-47c2-a41a-c19d8ad362a2)
- Message Length: The length of the cleartext should be **< 264bits**. The size needs to be in the **comparison area** to keep the **digest** as **random** as possible.
- Digest Length: The length of the hash digest should be 256bits in SHA-256 algo, 512bits in the SHA-512. Bigger digests usually suggest **more calculations** at the **cost of speed** and **space**.
- Irreversible: All hash functions such as SHA-256 are irreversible. Should neither get a **plaintext** when u have the **digest** beforehand nor should the **digest** provide its **original value** when u pass it **through the hash function** again. *Digest should not be able to produce the original message.

**Application of SHA algo**
![apps_Sha](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/60050235-03dd-4c17-81e2-a135826ab2b8)
- Digital Signature Verification: DS follow **asymmetric encryption** to verify the authenticity of a document/file. Hash algo like SHA-256 go a long way in ensuring the verificaiton of the signature
- Password Hashing: Website store user passwords in a hased format for 2 benefits. It helps foster a sense of privacy, and it lessens the load on the central database since all the digests area of similar size.
- SSL Handshake: Crucial for **web browsing sessions**. Consist of the web browsers and the web servers agreeing on encryption keys and hashing authenticiation to prepare a secure connections.

**RIPEMD**: The RIPEMD is an acronym for RACE Integrity Primitives Evaluation Message Digest.
- The set includes RIPEMD, RIPEMD-128, and RIPEMD-160 (most common). There also exist **256**, and **320-bit** versions of this algorithm
- Original RIPEMD (128 bit) is based upon the design principles used in MD4 and found to provide questionable security. RIPEMD 128-bit version came as a quick fix replacement to overcome vulnerabilities on the original RIPEMD.
- RIPEMD-160 is an improved version and the most widely used version among family. The 256 and 320-bit versions reduce the chance of accidental collision, but do not have higher levels of security as compared to RIPEMD-128 and RIPEMD-160 respectively.

**BLAKE2**: Designed to **replaced MD5 and SHA-1** algorithms in applications requiring **high performance** in software, It provides **better security** than **SHA-2** and **similar** to that of **SHS-3**.
- Provides immunity to length extensions
- Removes the addition of constants to message words
- Simplifies padding and reduces the number of rounds from 16 to 12.

**BLAKE3**: Cryptographic function based on **Bao and BLAKE2**. It is a few times **faster** than **BLAKE2**. This algorithm provides many features like **parallelism**, XOF, KDF, etc.

**Whirlpool**: 512-bit hash function
- It is derived from the modified version of Advanced Encryption Standard (AES).
- Three versions of Whirlpool have been released; namely WHIRLPOOL-0, WHIRLPOOL-T and WHIRLPOOL


## Attacks on Hash Functions
These attacks may allow the attackers to double-spending their money or to tamper with the blockchain.
1. **Collision attacks**: A collision attack is an attack in which **two different messages** produce the **same hash value**. If an attacker can find a collision, they could potentially create **two different transactions** that have the **same hash value**.
![CA](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/3aadaa64-6ab4-48e7-ae75-ae77093bf617)

2. **Preimage attacks**: A preimage attack is an attack in which an attacker can find **a message** that **produces a given hash value**. If an attacker can find **a preimage**, they could potentially create **a fake transaction** that has the **same hash value** as a **legitimate transaction**. 
![PA](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/e0548049-5096-4e8e-b58f-5d21ae1d33ef)

3. **Second preimage attacks**: A second preimage attack is an attack in which an attacker can find **a second message** that **produces** the **same hash value** as a **given message**. If an attacker can find a **second preimage**, they could potentially create a **fake transaction** that has the **same hash value** as a **legitimate transaction**.
   
![SPA](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/e6b04d22-6679-44af-86c2-82914b05ad75)

5. **Length extension attacks**: A length extension attack is an attack in which an attacker can **extend a message** after it has been **hashed** and **produce a different hash value**. If the attacker perform this, may tamper with the data on the blockchain.
![LE](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/d9bd7315-8cfd-451e-9600-87ce0ecf56bc)

> [!WARNING]
> 1. Double spending: An attacker could use a **collision attack** to **create two different transactions** that have the **same valu**e. This would allow the attacker to **double-spend** their money.
> 2. Tampering with the blockchain: An attacker could use **preimage attack** or a **second preimage attack** to create a **fake transaction** that has the **same hash value** as a **legitimate transaction**.
> 3. Denial of service attacks: An attacker could use a **length extension attack** to **tamper with data** on the blockchain. Which would prevent **legitimate users** from **accessing** the blockchain.

## Conclusion:
Cryptographic hash functions are vital in ensuring the security and integrity of data in various digital applications, notably in blockchain technology. Their ability to provide a secure, one-way, and collision-resistant method of encoding information is fundamental in maintaining the trustworthiness and reliability of blockchain networks. Understanding these technical aspects is essential for appreciating how cryptographic hash functions underpin the security of modern digital transactions and data management systems.
