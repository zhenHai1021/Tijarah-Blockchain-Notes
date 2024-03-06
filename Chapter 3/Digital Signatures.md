# Digital Signatures
KEYWORD:
Digital Signature, Private Key/Public Key, Authentication, Security

Digital Signatures ensure authenticity and integrity of transactions in distributed networks. Cryptographic tool security transactions, establishing accountability and trust among participants. Analogous to handwritten signatures with enhanced security. Mathematical scheme demonstrating authenticity of digital messages/documents.

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
        User initiates blockchain transaction, generates digital signature using private key.
        Process: Create hash of transaction data, encrypt hash with private key.
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
        Other blockchain participants receive transaction, use sender's public key to decrypt signature. Independently compute hash of original transaction data. If hash matches decrypted hash from signature, confirms transaction authentic and untampered.
      </li>
    </ul>
  </li>
</ol>

## Key Properties of Digital Signatures in Blockchain
1. Integrity: Ensure the **integrity of a transaction** by certifying that the contents have not been **altered in transit**. Hash function allows signing entire message without splitting into blocks, enabling receiver to verify all blocks are present and in correct order.
   
2. Authentication: They provide **proof of the origin** of the transaction, affirming that it was **indeed created** by the **stated sender**.
> [!Note]
> A branch office bank want to send instructions to the central office to change the balance of an account. To ensure the authenticity and integrity of the message, the branch office use its private key to generate a digital signature for the message.
  > 1. The branch office **creates** the **message**.
  > 2. Using its **private key**, the branch office generates a **unique digital signature** for the message.
  > 3.The signed message is then **transmitted** to the central office along with the **digital signature**.
  > 4. Upon **receiving** the message, the central office uses the **public key** from the branch office to **verify** the digital signature. If the verification is **successful**, it **confirms** that the message was indeed sent by the branch office and has no tampered with during transit.
  > 5. With the authenticity and integrity of the message **verified**, the central office can **proceed** to act on the instructions provided in the message, such as updating the account balance.
> Authentication ensures the message transmission from malicious entity intercept, they would not be able forge or modify the message without detection. The use of DS provides a secure authentication of the origin message for trust & security.

3. Non-repudiation: The signer cannot **deny** their intention of the transaction since the DS uniquely binds them. Cannot later deny signing information. Access to public key alone does not enable forging valid signatures. Ensuring secret keys used for authentication and non-repudiation have not been revoked before use. Revocation of key-pairs prevent exploitation of leaked secret keys by unauthorized parties.
> [!Note]
>  Similar to vendors checking the credit card validity online before accepting payment, verifying revocation status of a key-pair requires an "online" check through methods like certificate revocation lists. Failure to revoke stolen key pairs promptly can lead to unauthorized use, such as signing bogus for malicious purposes, which may only be discovered after the fact.

4. Security: DS are virtually **impossible to forge**, provided the p**rivate key remains secure**.

## Applications in Blockchain
1. Transaction Verification: In cryptocurrencies, every transaction is signed by the **sender’s private key** and **verified** by the network, ensuring that the transaction is initiated by the **rightful owner** of the digital assets.
 
2. Smart Contracts: In blockchain platforms like Ethereum, digital signatures are used to **execute smart contracts**, ensuring that the contract is executed by the parties involved without repudiation.
  
3. Identity Verification: Blockchain applications that require **identity management** use digital signatures to **authenticate** user actions and secure personal data.

## Limitation
1. Replays: A digital signature scheme on its own does not prevent a valid signed message from being recorded and then maliciously reused in a replay attack.
> Eg, the branch office requests that bank transfer once in a signed message. If the bank doesn't use a system of transaction ids in their messages to detect which transfers have already happened, someone could illegitimately reuse the same signed message many times to drain an account.

2. Uniqueness and malleability of signatures: In some signature schemes, a signature cannot unqieuly identify the message it signs. Every message has multiple possible valid signatures from the same signer. Possible, even without the private key, to transform one valid signature into another valid signature on the same message.
> [!Note]
> Malleability means quality of smtg can be shaped into something else without breaking.

3. Authenticating a public key: **Public key verifies authenticity** of a signed message, but signed message cannot be used to verify authenticity of a public key. In some signature schemes, **given** a **signed message**, can **construct a public key** under which **signed message** will pass **verification**, even without knowledge of the private key originally used to sign the message.
4. Theft of keys: lost or theft of keys is one of the major drawback of digital signature. The use of vulnerable storage.
5. Additional cost: To effectively use digital signatures sender and receiver needs to buy digital certificate and verification software at a cost.
6. Need for standard: There is a strong need for a standard through which these different methods can intetract.

> [!WARNING]
> Security Consideration: 
> The security of a digital signature in blockchain is tied to the security of the private key. If a private key is compromised, it can lead to unauthorized transactions and breaches. Therefore, robust key management practices are essential.

## Some digital signature algorithms
1. ECDSA (Elliptic Curve Digital Signature Algorithm): Widely used in blockchains, including Bitcoin & Ethereum. Strong security with short key lengths, efficient for resource constrained blockchain networks. ECDSA relies on the difficulty of solving in ECC.
ECDSA used for Transport Layer Security (TLS), the successor to Secure Sockets Layer (SSL), web browsers and a web application connections. Enables encrypted HTTPS website[^1].

2. RSA (Rivest-Shamir-Adleman): RSA relies on the difficulty of factoring large prime numbers, offering strong security for digital signatures. However, RSA key lengths tend to be longer compared to ECDSA, which can impact performance and efficiency in blockchain networks.
   
3. EdDSA (Edwards-curve Digital Signature Algo): Efficient with fast signature generation/verification and strong security guarantees. Based on twisted Edwards curves. Well-suited for decentralized blockchain systems due to performance advantages and resistance to side-channel attacks.
  
4. ElGamal Signature scheme: DS is based on the algebraic properties of modular exponentiation together with the diffculty of computing discrete logarithms. This is rarely used in practice.
 
5. Schnorr signature: ECDSA lacks one important property i.e. there is no efficient way to compress and verify signatures together. Schnorr signature schemes are provably secure with standard crytographic assumptions, non-malleable and provide linearity.
 
6. BLS Signature: BLS DS relies on pairings-based cryptography. BLS signatures enable key and signature aggregation but they are deterministic, allow signature aggregation across an entire block, and are overall 50% smaller. 

## Conclusion
Digital Signatures crucial for blockchain trustworthiness. Provide secure, efficient means ensuring transaction authenticity and integrity. Leveraging cryptography for secure, transparent blockchain operation. Enable trust in decentralized digital transations. Role vital as blockchain integrates across sectors to secure and validate data.

![Untitled-2024-02-26-1801](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/f5235bd3-e4eb-495b-a504-d6c04b0ac72e)

---
# REFERENCE
[^1]: [ECC Digital Signature Algorithm](https://www.hypr.com/security-encyclopedia/elliptic-curve-digital-signature-algorithm#:~:text=The%20Elliptic%20Curve%20Digital%20Signature%20Algorithm%20(ECDSA)%20is%20a%20Digital,public%20key%20cryptography%20(PKC).)
