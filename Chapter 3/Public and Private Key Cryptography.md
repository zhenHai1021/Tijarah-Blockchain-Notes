# Public and Private Key Cryptography
## Elliptic Curve Cryptography (ECC)
ECC is a public key cryptosystem that leverages the elliptic curve theory and the mathematical properties of elliptic curves to provide secure communication and encryption. It is more efficient and immune to attacks compared to others, such as RSA encryption. 

**What are ECC**
An elliptic curve is a set of points defined by a specific equation, usually in the form of y2 = x3 + ax + b, where a and b are constants, determining the shape and characteristics of the curve. The equation describes the relationship between x and y coordinates of the points that lie on the curve.

![ECC](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/46f8befb-9e28-444d-badd-8ae1e46e7c36)

Properties:
- Horizontal Symmetry. If a point (x,y) is on the curve, its reflection point (x, -y) is also on the curve. The y-coordinate of the reflection point is the negation of the original point’s y-coordinate.
- Interpolation. Any non-vertical straight line intersects the curve at a maximum of three distinct points. Helps to determine the whereabouts of a point on the curve based on other known points.
- Group structure. EC from a mathematical group under an operation called point addition. This define how u can add 2 points on the curve to produce a third point on the same curve.

Graph Work:

![ECC graph](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/7f30c6d5-2e64-449e-a459-faaf79bdc95c)

From ascending flow start from 1G
1. Find the tangent of point 1G, then a line pass through any first point intersact the graph.
2. 2G is intesacted, a x-axis symmetric/mirror of point 2G is pointed out to 3G.
3. Again the process, Find the tangent of point 3G, line for the first intersaction.
4. 4G until the desired.

Ref: 
[Elliptic Curves - Computerphile](https://youtu.be/NF1pwjL9-DE?si=dAh5r9-nUzBTLE0Y)

**How does ECC Work**
The public key is shared with others. Then anyone can use it send the owner an encrypted message
THe private key is kept secret, only the owner knows it. They need it to decrypt the received encrypted mesasge.
![ECC(1)](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/7039ae82-496b-4cbe-8b52-f9e781c5de24)

The security of the ECC encryption relies on the relationship between the key pairs and the properties and mathematical problems of the elliptic curve.
1. Key Generation. Bob and Alice select a specific Elliptic Curve with known parameters. They can then independently choose or generate random numbers as their private keys. Once Bob’s private key is ready, he computes the corresponding public key using his private key and then chooses an elliptic curve.
   
![ECC1](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/4eca8a06-90dc-4c5a-aea1-a91f26808a7c)

2. Key distribution. Bob shares his ECC public key with whomever he wants to exchange messages with, let’s say his friend Alice.
   
![ECC2](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/f100c494-742e-4c72-b177-b74152cf3c8f)

3. Encryption. Once Alice knows Bob’s public key, she uses multiple calculations based on elliptic curve theory to transform a plaintext message into ciphertext.
   
![ECC3](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/66112432-77e5-48da-9698-80b88b124ea5)

5. Decryption. Bob receives the encrypted message and uses his valid ECC private key to obtain the original plaintext message.
   
![ECC4](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/3df84876-31e7-476f-92ba-e6507e95970f)

> [!Note]
> Is ECC secure?
>> ECC’s security deeply depends on correct implementation and the use of appropriate parameters, such as the size of the underlying elliptic curve and the ECC key length. The encryption will be vulnerable to attacks if weak parameters or inadequate key size are chosen.

**ECC vs Rivest-Shamir-Adleman (RSA)**
| ECC | RSA |
| --- | --- |
|Relies on solving the Elliptic Curve Discrete logarithm | Strength depends on the difficulty of factoring large numbers|
|Requires a shorter key length to achieve the same level of security.  
A 256-bit ECC key is = to a 3072-bit RSA key| - |
|Takes less computational power, bandwidth and memory. More efficient and faster|Efficient with a smaller key size, but compromise its security|
|ECC gaining popularity as more efficient and sustainable alternative.|Has been used for several decades and is well-established and standardized in many system.|
- ECC features smaller ciphertexts, keys and signatures, and faster generation of keys and signature. Its decryption and encryption speeds are moderately fast.
- ECC enable lower latency than inverse througout by computing signatures in 2 steage.
- ECC features strong protocols for authenticated key exchange and support for the tech is strong.

**Real Life applications of ECC**
1. Communication Protocols: ECC protects the confidentiality, integrity and authenticity of network data. Communication protocols, such as Transport Layer Security (TLS) and Secure Shell (SSH), often take advantage of ECC.
> [!Tip]
> Eg, TLS handshake uses ECC for key exchange and ECC-based digital certificates for server authentication.
2. Digital Signatures: ECC is handy for generating and verifying digital signatures in e-commerce, financial and other systems. It ensures the authenticity and integrity of digital documents, contracts and transactions.
3. Payment systems: ECC protects payment systems, including contactless and mobile payment solutions. From securing key exchange to encrypting transaction data and verifying the authenticity of the data’s owner, it helps to secure transactions, protect sensitive financial information, and ensure the integrity of payment processes.
4. Virtual Private Networks (VPNs): VPNs can use ECC to establish secure and encrypted connections between clients and servers. VPNs usually use ECC for secure key exchange and server authentication while establishing a VPN connection.
5. Email and messaging: Email protocols, such as Pretty Good Privacy (PGP) or Secure/Multipurpose Internet Mail Extensions (S/MIME), also use ECC. It helps to encrypt and digitally sign email messages, enabling secure communication and protecting the email contents’ privacy.
6. Blockchain and cryptocurrencies. Many blockchain platforms and cryptocurrencies, such as Bitcoin and Ethereum, use ECC for generating and managing digital signatures, verifying transactions, and securing underlying cryptographic protocols.

**Benefits of ECC:**
1. Strong security: Provides same level of security compared to other cryptosystems, but ECC keys are much smaller
2. Efficient Performance: Require fewer computational resources, storage space, and bandwidth > most public key cryptosystems. Suitable for devices with limited computational power, such as mobile devices and embedded systems, or for transmitting data over low bandwidth networks.
3. Standardization: Since cryptographic standard organizations and industry bodies have standardized various aspects of ECC for cryptographic applications, many ECC in modern cryptographic libraries, protocols and applications can be found.
4. Compatibility: Implementing ECC across different platforms and integrating it into existing cryptographic systems or protocols. ECC works seamlessly alongside other cryptographic algorithms.

**FAQ**
1. How Secure is ECC
Side-channel attacks including differential power attacks, fault analysis, simple power attacks, and simple timing attacks, typically result in information leaks. Simple countermeasures exist for all types of **side-channel attacks**.

> [!Tip]
> 1. Acoustic Cryptanalysis
>> Emit sounds when performing operations (Such as encryption or decryption), attackers can correlate them with specific operations and deduce information about the system. For instance, keystrokes on a keyboard can emit distinct sounds, which could be used to steal a user’s passphrase.
> 2. Power Analysis
>> Consume varying amounts of power during different operations. By monitoring power consumption, attackers can infer details about the cryptographic process.Differential Power Analysis (DPA) is a well-known technique where attackers analyze power traces to extract secret keys.
> 3. Timing Attacks
>> Take different amounts of time to execute different operations. Attackers measure execution times and exploit variations to deduce information. Eg, timing attacks can reveal secret keys by observing how long an operation takes
> 4. Electromagnetic Radiation (EM) Attacks
>> Emit radiation during operations. Sophisticated attackers can capture this radiation and analyze it to extract sensitive information. EM attacks are particularly effective against smart cards and hardware security modules
> 5. Cache Timing Attacks
>> Modern processors use caches to speed up memory access. By observing cache behaviour during cryptographic operations, attackers can infer information. Eg, cache timing attackers can reveal secret keys by analyzing cache hits and misses.
> 6. Fault Attacks
>> Intentionally inducing faults (eg, voltage glitches) during cryptographic operations. Analyzing the faulty results can reveal information about the system. Fault attack can lead to key extraction or even bypassing securing mechanisms.

Any additional type of ECC attack is the **twist-security attack/fault attack**. Such attacks may include invalid-curve attaks and small-subgroup attacks, may result in the private key of the victim leaking out. Twist-security attacks are typically simply mitigated with careful parameter validation and curve choices.

2. What is an Elliptic Curve Digital Signature?
An Elliptic Curve Digital Signature Algorithm (ECDSA) uses ECC keys to ensure each user is unique and every transaction is secure. Although this kind of Digital Signing Algorithm (DSA) offers functional outcomes as other DSAs, ECC uses smaller, which is more efficient.

> [!Tip]
> 1. Twist-Security Attack
>> A twist is a related curve that shares some properties with the original curve. This attacks exploit this relationship between the original curve and its twist. The attacker computers certain values modulo specific parameters and uses mathematical techniques to extract information. These attacks can result in the leakage of the victim’s private key.
> 2. Invalid-Curve Attacks
>> In an invalid-curve attack, the attacker deliberately sends a point that does not lie on the elliptic curve. The scalar multiplication device (used in ECC operations) processes this invalid pointBy choosing the invalid point, the attacker aims to exploit vulnerabilities in the ECC implementation. Invalid-curve attacks can lead to security breaches and the exposure of private keys

## Public and Private Key Cryptography
**Public and private key cryptography**, also known as **asymmetric cryptography**, is a fundamental component of security practices. A cryptographic key is a string of data used to **encrypt data** (to keep the data secret), **decrypt data** (to perform the reverse operation), **sign data** (to ensure that the data is authentic) or to **verify a signature**. This cryptographic system uses a **pair of keys** - a **public key** and **private key**, to secure communication and data transactions.

**Basic Principle:**
1. Key Pair: In asymmetric cryptography, two mathematically related keys are used. The public key (encryption key) is shared openly, while the private key (decryption key) is kept secret.
2. Encryption and Decryption: Messages encrypted with the public key can only be decrypted with the  corresponding private key, and vice versa.
3. Digital Signatures: Data signed with the private key can be verified by anyone using the corresponding public key, ensuring authenticity and integrity.
4. Forms of Encryption: In a symmetric algorithm, the key for encryption are the same; In an asymmetric algorithm, there are public and private keys.

**Technical Details:**
Key Generation: The strength cryptography lies in the **computational complexity** of **linking** the public and private keys. The keys are typically generated using algorithms based on mathematical problems such as the factoring of large prime numbers (RSA algo) or the discrete logarithm problem (as in ECC-Elliptic Curve Cryptography).

Encryption Process: Data encryption involves mathematical algorithms that use the public key to **transform data** into a format that can only be **reversed** (decrypted) with the **corresponding private key**.

Signature Creation and Verification: A **digital signature** is created by processing the data with a **private key**. The **signature**, along with the original data, can be sent to a recipient who can use the **public key** to **verify the signature’s authenticity**.

Symmetric Encryption and Asymmetric Encryption:
|Symmetric Encryption|Asymmetric Encryption|
|---|---|
|Uses a single key that needs to be shared between the people who need to receive the message|Uses a pair of public keys and a private key to encrypt and decrypt message|
|Problem inherent in the need to share the key on the symmetric cryptography model|Eliminate the need to share the key by using a pair of public and private keys|

**Public Key Infrastructure**
PKI is a framework of roles, policies, hardware, software, and procedures needed to create, manage, distribute, use, store and revoke digital certificates. Support identity management services within and across networks and underpin online authentication in secure socket layer (SSL) and transport layer security (TLS) for protecting internet traffic including document/transaction signing, code signing. 
- Support solutions for desktop login, mobile banking and device credentialing in the IoT
- Rely on digital certificates to link public keys to their owners. These certificates serve as credentials to confirm user identities during transactions
> passports verifying citizenship. Protecting the integrity of digital certificates for maintaining system trustworthiness, as they are used to identify recipients of encrypted data and verify the identity of information signer.
- In the context of PKI, a digital certificate, issued by a Certificate Authority (CA), binds a public key to an entity (like an individual or organization), ensuring the public key’s authenticity.
> [!Tip]
> Certificate Authorities (CAs) issue these digital credentials, compromising PKI security, However, CAs can be targets of sophisticated attacks. To safeguard against threats, PKIs implement physical and logical controls, including hardware security modules (HSM), to fortify their integrity

**Applications in Blockchain**
- Transaction Verification: User’s public key serves as their address, while the private key is used to sign transactions. This ensures that only the wonder of the private key can authorize transactions from their account.
- Security and Anonymity: While the public key is visible to all participants in the blockchain network, the private key remains confidential, maintaining security and user anonymity.

**Security Considerations**
- Key management: The security of asymmetric cryptography heavily relies on how private keys are managed and stored. If a private key is compromised, the security of the system is at risk.
- Computational Power: The security of public and private key cryptography is based on the current limitations of computational power and algorithmic efficiency. It is essential to stay updated with cryptographic advancements to counteract

## Public Key Cryptography/Asymmetric Cryptography
Public keys are those can be widely share, and private keys are known only to their owners.

![ASYM](https://github.com/zhenHai1021/Tijarah-Blockchain-Notes/assets/113818064/f65b1bba-7398-43e7-b2dc-669d6bca75a4)

This key pair insist **two functions**: Authentication and Encryption
- In authentication, the public key verifies that the holder of the paired private key can decrypt the message encrypted with the public key.
- In encryption, only the holder of the paired private key can decrypt the message encrypted with the public key.

**Symmetric Encryption**
Implementing symmetric cryptography, is efficient due to **minimal time delays** in encryption and decryption processes. It also offers **authentication**, as data **encrypted** with **one symmetric key** can only be **decrypted** with the **same key**, ensuring communication security between trusted parties. Symmetric keys are unique for each participant, exchanged securely to maintain confidentiality. However, the challenges lies in **securely exchanging** these secret keys, often **requiring encryption** with **another key** and creating a **dependency loop**. **Unauthorized access** to a symmetric key compromises both **confidentiality and authentication**.

**Public key challenges**
Security of encryption keys depends on choosing a strong encryption algorithm and maintaining high levels of operational security. The following key challenges must be considered:
- Management: Diligent management of private keys is necessary to protect them from loss, corruption or unauthorized access.
- Continuous updating: Private keys used to decrypt sensitive data must be changed regularly to minimize exposure in the event leakage, loss corruption or unauthorized access
- Recovery and Loss: If an encryption key becomes inaccessible, the data encrypted with that key will be unrecoverable and lost. This is why Ledger recently launched its Recover program, see the analysis of the risks and possible impacts of Ledger Recover here.

## Private Key/Secret Key
Or secret key, is a variable in cryptography used with an algorithm to encrypt and decrypt data. Secret keys (private keys) should only be shared with the **generator of the key** or the **parties authorized** to **decrypt** the data. 
A PK is usually a long sequence of bits, generated randomly or pseudo-randomly, which **cannot be easily guessed**. The complexity and length of the private key determine how easily an attacker can carry out the brute force attack, in which they try to find the right one among keys.

**Benefits**
Security: Longer private keys with greater randomness, are more secure against brute force or dictionary attacks.
Speed: Symmetric key cryptography is faster from a computational point of view than asymmetric cryptography with its public-private key pairs.
Better for encryption: Most cryptographic processes uses private keys to encrypt data transmissions.

**Private Key Challenge**
- Management: Storing and securely distributing.
- Key Length: As computational power increases, longer keys are needed to maintain security. Balancing key length with performance and efficiency.
- Side Channel attack: Side channel attacks may exploit information leaks during cryptographic operations
- Random Number Generation: High-quality random number generation is essential for creating secure keys. Weak random may be easily compromised
- Key expiry: Manageing revoked or expired.
- Human Factors: Mishandle private keys (eg, sharing, storing insecurely or forgetting passphrases)

## Private And Public Key Differences
Two different but mathematically linked keys are used to transform plain text in encrypted cipher text or encrypted text back into plain text.
| Private | Public |
|---|---|
|Used to **encrypted** the ciphertext, this text can be **decrypted** using the **public key**. This ciphertext can be a component of a **digital signature** and be used to **authenticate** the signature| Encrypt the ciphertext, that text can only be decrypted using the private key|
|Only the holder of the private key can have **encrypted** the ciphertext, so if the related public key manages to decrypt it, the **digital signature** will be **verified**|Allow anyone with **access** to the public key to **encrypt** a message, and only the holder of the **private key** can **decrypt** it|
|Private key is **confidential** and should only be accessed by the **owner** of the public key pair.|Made available to everyone who needs it in a publicly accessible repository|
> [!IMPORTANT]
> Anything encrypted with the public key requires the related private key for decryption. Public key cryptography is usually used to protect communication channels such as e-mail.

