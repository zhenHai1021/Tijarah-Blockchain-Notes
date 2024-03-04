# Digital Signatures
Ensuring authenticity and integrity of transactions within a distributed network. They serve as a cryptographic tool that not only secure transactions but also establishes a layer of accountability and trust among participants.

Understanding Digital Signatures
A digital signature is a cryptographic technique analogous to a handwritten signature or a stamped seal, but with far more inherent security built into its design. It is a mathematical scheme for demonstrating the authenticity of digital messages or documents. 

![DS(AB)](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/44b9253a-5b6e-4c7f-a617-9e32f64a0493)

> Alice signs a message “Hello Bob” by appending a signature computed from the message and her private key. Bob receives both the message and signature. He uses Alice’s public key to verify the authenticity of the signed message.

**A digital signatures typically consists of 3 algorithms:**
- a key generation algorithm that selects a **private key** uniformly at **random** from a set of **possible private keys**. The algorithm outputs the **private key** and a corresponding **public key**
- A signing algorithm that, given a message and a private key, produces a **signature**
- A signature verifying algorithm that, given then message, public key and signature, either accepts or reject the message’s claim to authenticity.

## Technical Mechanism
<ol>
  <li>
    Creation of Digital Signatures
    <ul>
      <li>
        A digital signature is created using a private key to ‘sign’ a transaction or a piece of data.
      </li>
      <li>
        When a user initiates a blockchain transaction (like sending cryptocurrency), they generate a digital signature using their private key. This process involves creating a hash of the transaction data and then encrypting the hash with the private key.
      </li>
    </ul>
  </li>
  <li>
    Verification Process
    <ul>
      <li>
        The verification of a digital signature is done using the signer’s public key.
      </li>
      <li>
        When other participants in the blockchain network receive the transaction, they use the sender’s public key to decrypt the signature. They independently compute the hash of the original transaction data. If this hash matches the decrypted hash from the signature, it confirms that the transaction is authentic and has not been tampered with.
      </li>
    </ul>
  </li>
</ol>

## Key Properties of Digital Signatures in Blockchain
1. Integrity: Ensure the **integrity of a transaction** by certifying that the contents have not been **altered in transit**. Without the hash function, the text “to be signed” may have to split (separated) in blocks small enough for the signature scheme to act on them directly. However, the receiver of the signed blocks is not able to recognize if all the blocks are present and in the appropriate order.
   
2. Authentication: They provide proof of the origin of the transaction, affirming that it was indeed created by the stated sender.
> [!Note]
> A branch office bank want to send instructions to the central office to change the balance of an account. To ensure the authenticity and integrity of the message, the branch office use its private key to generate a digital signature for the message.
  > 1. The branch office **creates** the** message**.
  > 2. Using its **private key**, the branch office generates a **unique digital signature** for the message.
  > 3.The signed message is then **transmitted** to the central office along with the **digital signature**.
  > 4. Upon **receiving** the message, the central office uses the **public key** from the branch office to **verify** the digital signature. If the verification is **successful**, it **confirms** that the message was indeed sent by the branch office and has no tampered with during transit.
  > 5. With the authenticity and integrity of the message **verified**, the central office can **proceed** to act on the instructions provided in the message, such as updating the account balance.
> Authentication ensures if the message is intercepted by a malicious entity during transit, they would not be able forge or modify the message without detection. The use of digital signatures provides a secure method for authentication of the origin message for trust and security.

3. Non-repudiation: The signer cannot **deny** their intention of the transaction since the DS uniquely binds them to it. An entity that has signed some information cannot at a later time deny having signed it. Similarly, access to the access public key only does not enable a fraudulent party to fake a valid signature. Ensuring that secret keys used for authentication and non-repudiation have not been revoked before their usage. Revocation of key-pairs to prevent leaked secret keys from being exploited by unauthorized. 
> [!Note]
>  Similar to how a vendor checks the validity of a credit card online before accepting payment, verifying the revocation status of a key-pair requires an "online" check through methods like certificate revocation lists. Failure to revoke stolen key pairs promptly can lead to unauthorized use, such as signing bogus certificates for malicious purposes, which may only be discovered after the fact.

4. Security: DS are virtually **impossible to forge**, provided the p**rivate key remains secure**.

## Applications in Blockchain
1. Transaction Verification: In cryptocurrencies, every transaction is signed by the **sender’s private key** and **verified** by the network, ensuring that the transaction is initiated by the **rightful owner** of the digital assets.
 
2. Smart Contracts: In blockchain platforms like Ethereum, digital signatures are used to **execute smart contracts**, ensuring that the contract is executed by the parties involved without repudiation.
  
3. Identity Verification: Blockchain applications that require **identity management** use digital signatures to **authenticate** user actions and secure personal data.

## Digital signatures limitation
1. Replays: A digital signature scheme on its own does not prevent a valid signed message from being recorded and then maliciously reused in a replay attack.
> Eg, the branch office may request that bank transfer be issued once in a signed message. If the bank doesn't use a system of transaction ids in their messages to detect which transfers have already happened, someone could illegitimately reuse the same signed message many times to drain an account.

2. Uniqueness and malleability of signatures: A signature itself cannot be used to uniquely identify the message it signs, in some signature schemes, every message has a large number of possible valid signatures from the same signer, and it may be easy, even without knowledge of the private key, to transform one valid signature into another.
> [!Note]
> Malleability means quality of smtg can be shaped into something else without breaking.

3. Authenticating a public key: **Public key** can be used to **verify authenticity** of a signed message, but not the other way around, signed message cannot be used to verify authenticity of a public key. In some signature schemes, **given** a **signed message**, it is easy to **construct a public key** under which the **signed message** will pass **verification**, even without knowledge of the private key that was used to make the signed message in the first place.

> [!WARNING]
> Security Consideration: 
> The security of a digital signature in blockchain is tied to the security of the private key. If a private key is compromised, it can lead to unauthorized transactions and breaches. Therefore, robust key management practices are essential.

## Some digital signature algorithms
1. ECDSA (Elliptic Curve Digital Signature Algorithm): Widely used in blockchains, including Bitcoin & Ethereum. Offers strong security with relatively short key lengths, making it efficient for use in resource constrained environments like blockchain networks. ECDSA relies on the difficulty of solving the problem in ECC.
ECDSA used for Transport Layer Security (TLS), the successor to Secure Sockets Layer (SSL), by encrypting connections between web browsers and a web application. The encrypted connection of a HTTPS website[^1].

2. RSA (Rivest-Shamir-Adleman): RSA relies on the difficulty of factoring large prime numbers, offering strong security for digital signatures. However, RSA key lengths tend to be longer compared to ECDSA, which can impact performance and efficiency in blockchain networks.
   
3. EdDSA (Edwards-curve Digital Signature Algo): EdDSA efficiency and its security properties. It is based on twisted Edwards curves, offering fast signature generation and verification with strong security guarantees. EdDSA is well suited for use in decentralized systems like blockchain due to its performance advantages and resistance to side-channel attacks.
  
4. ElGamal Signature scheme: DS is based on the algebraic properties of modular exponentiation together with the diffculty of computing discrete logarithms. This is rarely used in practice.
 
5. Schnorr signature: ECDSA lacks one important property i.e. there is no efficient way to compress and verify signatures together. Schnorr signature schemes are provably secure with standard crytographic assumptions, non-malleable and provide linearity.
 
6. BLS Signature: BLS DS relies on pairings-based cryptography. BLS signatures enable key and signature aggregation but they are deterministic, allow signature aggregation across an entire block, and are overall 50% smaller. 

## Conclusion
Digital Signatures are crucial in maintaining the trustworthiness of blockchain. They provide a secure and efficient means of ensuring transactions authenticity and integrity. By leveraging cryptographic principles, digital signatures enable the secure and transparent operation of blockchains, underpinning the trust in decentralized digital transactions and interactions. As blockchain technology continues to evolve and integrate into various sectors, the role of digital signatures as a means of securing and validating data becomes increasingly vital.

---
# REFERENCE
[^1]: [ECC Digital Signature Algorithm](https://www.hypr.com/security-encyclopedia/elliptic-curve-digital-signature-algorithm#:~:text=The%20Elliptic%20Curve%20Digital%20Signature%20Algorithm%20(ECDSA)%20is%20a%20Digital,public%20key%20cryptography%20(PKC).)
