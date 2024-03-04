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
