# Blochain Vulnerabilities & Attacks
Enhanced security compared to traditional databases. Understanding these vulnerability attacks are crucial for developers, users and stakeholders in blockchain.

## Common Blockchain Vulnerabilities
<ol>
  <li>
    51% Attack
    <ol>
      <li>
        Description: When a single entity gains control >50% of the network hashing power, allowing to monopolize the creation of blocks 
      </li>
      <li>
        Implications: The attacker can double-spend coins and prevent other transactions from being confirmed, undermining the blockchain’s integrity 
      </li>
    </ol>
  </li>
  <li>
    Smart Contract
    <ol>
      <li>
        Description: Smart contract code can make it vulnerable. Since smart contracts are immutable once deployed, and bugs code can be exploited.
      </li>
      <li>
        Reentrancy attacks (like the famous DAO attack on Ethereum), where a function is repeatedly called before the first execution is completed, can drain funds from contracts. 
      </li>
    </ol>
  </li>
  <li>
    Sybil Attacks
    <ol>
      <li>
        Description: Creating large number of pseudonymous identities, using them to gain a disproportionately massive influence.
      </li>
      <li>
        Attacks: It can disrupt network operations or skew consensus processes. 
      </li>
    </ol>
  </li>
  <li>
    Routing Attacks
    <ol>
      <li>
        Description: Blockchain rely on internet infrastructure that susceptible to routing attacks. Attackers can intercept and modify unencrypted data during transmission between nodes.
      </li>
      <li>
        Impact: This can lead to double-spending, transaction delays, or privacy leaks 
      </li>
    </ol>
  </li>
</ol>

## Types of Blockchain Attacks
<ol>
  <li>
    Double Spending: When an actor spends the same token/currency twice. This is often the goal of a 51% attack
  </li>
  <li>
    Eclipse Attacks
    <ol>
      <li>
        Mechanics: Attacker isolate and surrounds a specific node with malicious nodes, controlling the node’s view of the blockchain
      </li>
      <li>
        Goal: To feed the targeted node false information, preventing it from legitimate transactions and blocks
      </li>
    </ol>
  </li>
  <li>
    Phishing Attacks
    <ol>
      <li>
        Mechanics: Attacker tricks users to reveal their private key from malicious email link/fraudulent addresses
      </li>
      <li>
        Mitigation: Require user awareness and robust security practices, such as two-factor authentication (2FA) and wallet security measures.
      </li>
    </ol>
  </li>
  <li>
    Timejacking Attacks
    <ol>
      <li>
        Mechanics: Manipulating a node’s system time to disrupt network synchronization
      </li>
      <li>
        Consequence: Lead to creation of parallel blockchains, causing confusion and disrupting consensus process 
      </li>
    </ol>
  </li>
  <li>
    DDoS Attack
    <ol>
      <li>
       Mechanic: Spam/flood the network with massive amounts of traffic or request to cause service disruptions and delays
      </li>
    </ol>
  </li>
  <li>
    Cryptographic Attacks
    <ol>
      <li>
        Mechanic: Attackers may try to break the algo or protocols, such as hashing algo, digital signatures, or encryption schemes.
      </li>
    </ol>
  </li>
  <li>
    Privacy Attacks
    <ol>
      <li>
        Mechanic: By analyzing transaction patterns, metadata and other on-chain data, attackers may attempt to disable anonymity users and compromise privacy.
      </li>
    </ol>
  </li>
  <li>
    Quantum Computing
    <ol>
      <li>
        Mechanic: May potentially leverage quantum computers to break cryptographic algo used in blockchain
      </li>
    </ol>
  </li>
</ol>

