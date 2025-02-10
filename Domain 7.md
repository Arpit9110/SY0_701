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

