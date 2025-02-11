# Cryptographic Solutions

### Symmetric vs Asymmetric
#### Symmetric Encryption 
It uses a single key for both encryption and decryption. Often referred to as private key encryption. Requires both sender and receiver to share the same secret key. It offers confidentiality but lacks non-repudiation. It pose challenges with key distribution in large-scale usage. More people means more sharing of the keys.

#### Asymmetric Encryption 

It uses two separate keys: Public key for encryption, Private key for decryption. Often called “Public Key Cryptography”, No need for shared secret keys. Commonly used algorithms include Diffie-Hellman, RSA, and Elliptic Curve Cryptography (ECC). Slower compared to symmetric encryption but solves key distribution challenges.


#### Hybrid Approach

It combines both symmetric and asymmetric encryption for optimal benefits. Asymmetric encryption used to encrypt and share a secret key. Symmetric encryption used for bulk data transfer, leveraging the shared secret key. Offers security and efficiency.

#### Stream Cipher

Encrypts data bit-by-bit or byte-by-byte in a continuous stream. It uses a keystream generator and exclusive XOR function for encryption. It is suitable for real-time communication data streams like audio and video. It is often used in symmetric algorithms.

#### Block Cipher

This method breaks input data into fixed-size blocks before encryption, usually 64, 128, or 256 bits at a time. Padding is added to smaller data blocks to fit the fixed block size. Advantages include ease of implementation and security. It can be implemented in **software**, whereas stream ciphers are often used in hardware solutions.

### Symmetric Algorithms

- DES (Data Encryption Standard) : This algorithm uses 64-bit key (56 effective bit due to parity. This encrypt the data in 64-bit block through 16 round of transposition and substitution. It was widely used from the 1970's to ealry 2000's.

- Triple DES (3times DES) :  This algorithm usages three 56 bit keys. This encypts data with the frirst key decrypt it with second key and re-encrypt it with the third key. It provides 112-bit key strength but is lower than DES.

- IDEA (International Data Encryption Algorithm) : This a symmetric block cipher with a 64-bit block size. It usages a 128 bit key, fater and more secure than DES.

- AES (Advance Encryption Standard) : This algorithm replaces the DES and 3DES as the US Government encryption standard. It supports 128-bit, or 256-bit keys and matching block sizes. It was widely adopted and considerd the encryption standard for the sensitive unclassified information.

- Blowfish : It is a form of Block cipher with key size raging from 32 to 448 bits. Developed as  a DES replacement but not widely adopted.

- Twofish : It is a block cipher supporting a 128-bit blocks sizeand key size of 128,192 or 256 bits.It is open source and available for use.

- RC Cipher Suite (RC4, RC5, RC6) : It is created by cryptogapher Ron Rivest. It was a stream cipher that usages keys from 40 to 2048 bits. It wase used in SSL, WEP and TLS communication. 
   - RC5 is a block cipher with key size up to 2048 bits
   - RC6 was based on RC5. It was considered as a DES replacement.

These all were the Symmetric encryption algorithms. 
Most are block cipher except for RC4, which is a stream cipher

Note: Working with the encryption always identify the whether it's a symmetric or asymmetric and whether it's a block or a stream cipher.


### Asymmetric Algorithms 

It is called as a public key Cryptography. As it have no shared secret key requirement. It usages a Key pair namely public-private key for encyption and dceryption respectively. It better provides confidentiality, integrity, authentication, and non-repudiation.

- The confidentiality with public key is as follows : The data is encrypted with the receiver's public key and only the receiver's private key can decrypt it. 

- Non-Repudiation with Private Key ia as follows: Encrypt data using the sender's private key.  Anyone with access to the sender's public key can verify the sender's identity.

Integrity and authentication with digital signature

Digital signature : In this a hash digest of the message is created and then that hash digeast is encrypted is with the sender's private key. By using this method the reciever can verify the document by decypring the hash by sender's public key and comparing the hash to the newely created one. This way the recipient can be sure that document was sent by the authentic sender.

Encryping the message with the reciever's public key will ensure the message integrity, Non-repudation and confidentiality.

Common Asymmetric Algorithms
- Diffie-Hellman: It is used for key exchange and secure key distribution. It is vulnerable to man-in-the-middle attacks, requires authentication. It is commonly used in VPN's tunnel establishment (IPSec).

- RSA (Ron Rivest, Adi Shamir, Leonard Adleman): it is used for key exchange, encryption and digital signatures. It relies on the mathematical difficulty of factoring large prime numbers. It supports key size from 1024 to 4096 bits.

- Elliptical Curve Cryptography (ECC). It is efficient and secure, uses algebric structure of ellipticall curves. Commonly used in mobile devices and low power computing. Six times more efficient than RSA fro equivalent security. 
  It's variants include:
	 - ECDH (Elliptic Curve Diffie-Hellman)
	 - ECDHE (Elliptic Curve Diffie-Hellman Ephemeral)
	 - ECDSA (Elliptical Curve Digital Signature Algorithm)
 
 
Hashing 
 
Hashing : It a one-way cryptographic function that produces a unique message digest from an input. Hashes changes drastically even with minor chages in the imput. Hashing is used to verify data integrity and detect any changes.

Hash Digest : It's like a digital fingerprint for the original data. It is of always the same length regardless of the input's length

Common Hashing Algorithms : 

- MD5 ( Message Digest Algorithms 5) : It create s a 128-bit hash value. It have Limited unique value leading to collisions. Not recommended for security-critical applications due to vulnerabilities.

- SHA (secure hash Algorithm) Family 

	- SHA-1: Produces a 160-bit hash digest, less prone to collision than MD5
	- SHA-2: Offers longer hash digests (SHA-224, SHA-256, SHA-348, SHA-512)
	- SHA-3: Uses 224-bit to 512-bit hash digests, more secure, it have 120 rounds of computations.

- RIPEMD ( RACE Integrity Primitive Evaluation Message Digest):
	Version Available : 
	 - 160 bits (Most Common)
	 - 256-bits
	 - 320-bits
	  It is an open source competitor to SHA but less popular.

- HMAC (Hash-based Message Authentication Code): It checks message integrity and authenticity. Utilizes other hashing algorithms e.g. HMAC-MD5, HMAC-SHA1, HMAC-SHA256).

Digital Signature: It uses a hash digest encrypted with a private Key. The sender hashes the message and encrypt the hash with their private key. Recipient decrypt the digital signature using the sender's public key. It verify integrity of the message and ensures non-repudation.

Common Digital Signature Algorithms

- DSA(Digital Security Algorithms): It is utilized for digital Signatures. It uses a 160-bit message digest created by DSS (Digital Security Standard). 

- RSA (Rivest-Shamir-Adleman): This algorithm supports digital signature, encryption, and key distribution. It is widely used in various applications, including code signing.


 Increasing Hash Security
 
Common Hashing Attacks
 
**Pass The Hash Attack** 
A Hacking technique that allows the attacker to authenticates to remote server or service by using the underlying hash of a user's password instead of requiring the associated plaintext password.
Hackers can be obtained by attackers to impersonate user without cracking the password. Difficult to defend against due to various windows vulnerabilities and applications. 
Penetration tools like Mimikatz automate hash harvesting.
Prevention
- Ensure trusted OS 
- Proper windows domain trust
- patching 
- Multi-factor authentication.
- Least Privilege

**Birthday attack**

Occurs when two different messages result in the same hash digest (collision). Named after the birthday paradox, where shared birthday becomes likely in a group. Collision in hashes can be exploited by attacker to bypass authentication system. 
Using longer hash output (e.g. SHA-256) to reduce collision and mitigate the attack.

**Increasing hash security security** 

- Key Stretching: This technique that is used to mitigate a weaker key by creating longer more secure key (at least 128 bits). It increases the time it needs to crack the key. used in system like WIFI protected Access, Wi-Fi Protected Access Version 2 and Pretty Good Privacy.

- Salting: This adds random data (salt) to passwords before hashing. Ensures distinct hash outputs for the same password due to different salts.  The common threat for this method are: Thwarts dictionary attacks, brute-force attacks, and rainbow tables.

- Nonces (Number Used Once) :Adds unique random number to password-based authentication porcesses. It prevent attackers from reusing stolen authentication data. Adds an extra layer of security against replay attacks.

- Limiting Failed login attempts: As the name suggests it limits the number of login attempts a user can make. It increases security by deterring the attacker attempting to guess passwords. the system typically locks the account after three incorrect attempts.

### Public Key Infrastructure (PKI)
Public key infrastructure (PKI) is a set of tools that create, manage, and distribute digital certificates and public keys. An entire system involving hardware, software, policies, procedures, and people. It is based on asymmetric encryption. Facilitates secure data transfer, authentication, and encrypted communications. Used in HTTPS Connections on website

#### Establishing a secure connection:

User connects to a website via HTTPS.
- Web browser contacts a trusted certificate authority for the web server's public key. 
- A random SHared secret key is generated for symmetric encryption.
- The shared secret is securely transmitted using public key encryption.
- The web server decrypts the shared secret with it's private key.
- Both parties use the shared secret for symmetric encryption (e.g. AES) to create a secure tunnel.

Security Benefits
Confidentiality: Data is encrypted using a shared secret.
Authentication: The web server's identity is verified using it's private key.
Visual indicators like a padlock show secure communication.


Public Key Infrastructure  vs Public Key Cryptography

Public Key Infrastructure (PKI): This term encompasses the entire system fro managing public and public key pairs, policies, and trust. It involves generating, validating nad managing public and private keys pairs that are used in the encryption and decryption process. It ensures the security and trustworthiness of keys.

Public Key Cryptography: Refers to the encryption and decryption process using public and private keys. It is only a part of the overall PKI architecture.


Key Escrow: it refers to the storage of cryptographic keys in a secure , third-party location called escrow. it enables key revival in case of key loss or for legal investigations. 

Relevance in PKI:
 In PKI, key escrow ensures that encrypted data is not permanently inaccessible

 Useful when individual or organization lose access to their encryption keys.

Security Concerns:
 Malicious access to escrowed keys could lead to data decryption.
 Requires stringent security measure and access control.
 
 
### Digital Certificates

Digital Certificates: These are digitally signed electronic documents. It binds a public key with a user's identity. These are used for individuals, servers, workstations, or devices.
These uses the X.509 Standard:
 Commonly used standard for digital certificates within PKI
 Contains owner's/user's information and certificate authority details.
 
 Types of digital certificates:
  
  Wildcard Certificate.
   Allows multiple subdomains to use the same certificate.  Easier management, cost-effective for subdomains. Compromise affect all subdomains.
   
  SAN(Subject Alternate Name) field.
   Certificate that specifies what additional domains and IP addresses are going to be supported. Used when domain name don't have the same root domain.
  
  Single-Sided and Dual-Sided Certificates.
   Single-sided
     Only requires the server to be validated
   Dual-sided
     Both server and user validate each other. Dual-sided for  higher security, requires more processing power.
  
  Self-Signed certificates
     Digital certificate that is signed by the same entity whoose identity it certifies. Provides encryption but lacks third-party trust. Used in testing or closed systems.
   
  Third-party Certificates
     Digital certificates issued and signed by trustedcertificate authorities (CA's). These are trusted by browser and systems. Preferred for public- facing websites.


Key Concepts

 - Root Of Trust: Highest level of trust in certificate validation. Trusted third-party providers like Verisign, Google,etc. Froms a certification path for trust.
 
 - Certificate Authority(CA): These are the trusted third party issue digital certificates. Certificates contains CA's information and digital signature. Validates and manages certificates.
 
 - Registration Authority(RA): Request identifying information form the user and forwards certificate request up to the CA to create a digital certificate. It Collects user infromation for certificates. Assists in the certficate issuance process.
 
 - Certificate Signing Request(CSR):  A block of encoded text with information about the entity requesting the certificate. It includes the public key. It is submitted yo CA fro cetificate issuance. Private key remains secure with the requester.
 
 - Certificate Revocation List(CRL): Thses are maintained by CA's. It contain list of all digital certificates that certificate authority has already revoked. Checked before validating a certificate.
 
 - Online Certificate Status Protocol(OCSP): It determines certificate revocation status or any digital certificate using the certificate's serial number. These are faster but less secure than CRL.
 
 - OCSP Stapling: This is an alternative to OCSP. It allows the certificate holder to get the OCSP record from the server at regular intervals. It includes OCSP record in the SSL?TLS handshake. This is a spped up the secure tunnel creation.
 
 - Public Key Pinning: It allows an HTTPS website to resist impersonation attacks from users who are trying to present fraudulent certificates. This presents trusted public keys to browsers. This alerts users if a fradulent certificates is detected.
 
 - Key Escrow Agents: This securely store copies of private keys. This ensures key recovery in case of loss. It requires strong access controls.
 
 - Key Recovery Agents: This specialized type of software that allows the restoration of a lost or corrupted key to be performed. This acts as a backup for certificate authority keys.
 
Trust in Digital Certificates: 
 - Trust is essential in digital certificates.
 - Compromised root CAs can impact all issued certificates.
 - Commercially trusted CAs are more secure.
 - Self-managed CAs must be vigilant against compromises.
    


Blockchain

 Blockchain: It shared immutable ledger for transactions and asset tracking. It is build to increase trust and transparency. It is widely associated with cryptocurrencies like bitcoin, dog-coin, etc. It is essentially a really long series of information with each block containing information in it. Each block has the hash for the block before it.
 Block Structure :
  Chain of block, each containing 
   - Previous Block's hash
   - Timestamp
   - Root Transactions(Hashes of individual transaction)
 Blocks are linked together in a chronological order
 
 Public ledger : It is more secure and more anonymous record keeping system. It maintain participant's identities. It tracks the cryptocurrency balances. It records all the genuine transactions in a network.

Blockchain Applications
 - Smart Contracts: It basically the self executing contract with code defined terms. It execute action automatically when the condition is/are met. It is transparent, tamper proof and trust-enhancing.

  - Commercial Uses:  Companies like IBM promote blockchain for commercial purposes, as these enhances trust and transparency with immutable public ledger.
  
  - Supply Chain Management: There is Transparency and traceability in the supply chain. There is immutable records of product origin, handling, and distribution. It Ensures compliance and quality control. 
  
  
Broad Implications of Blockchain

- Versatility:  Beyond finance and cryptocurrencies there are various applications across various industries. It promises transparency, efficiency, and trust
- Decentralization: It is the key feature of blockchain. It eliminates need for central authorities. It empowers peer-to-peer networks.

- Immutable Ledger:  It ensures data integrity. The records cannot be altered or deleted. This reinforces trust in transactions and information.

- Digital Evolution: Blockchain's impact on technology and industries is huge and it have a huge potential to reshape traditional systems. It Offers transparency, efficiency, and trust in the digital era.


### Encryption Tools 

Encryption Tools for Data Security are 

TPM(Trusted Platform Module):  It is a dedicated microcontroller for hardware-level security. It protects digital secrets through integrated cryptographic keys. It used in BitLocker drive encryption for Windows devices. It adds an extra layer of security against software attacks 

HSM(Hardware Security Module): These are Physical device for safeguarding and managing digital keys. These are ideal for mission-critical scenarios like financial transactions. This performs encryption operations in a tamper-proof environment. It ensures key security and regulatory compliance.

Key Management System: It manages, stores, distributes, and retires cryptographic keys. It is a centralized mechanism for key lifecycle management. It is crucial for securing data and preventing unauthorized access. It automates key management tasks in complex environments.

Secure Enclaves : It is basically a coprocessor integrated into the main processor of some devices. It is isolated from the main processor for secure data processing and storage. It provides safeguards to sensitive data like biometric information. It enhances device security by preventing unauthorized access.

### Obfuscation

Obfuscation Techniques in Data Security 