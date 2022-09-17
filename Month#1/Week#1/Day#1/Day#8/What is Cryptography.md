# What is Cryptography?

## **Cryptography Definition.**

* **Cryptography is the process of hiding or coding information so that only the person a message was intended for can read it. The art of cryptography has been used to code messages for thousands of years and continues to be used in bank cards, computer passwords, and ecommerce.**

* Modern cryptography techniques include algorithms and ciphers that enable the encryption and decryption of information, such as 128-bit and 256-bit encryption keys. Modern ciphers, such as the Advanced Encryption Standard (AES), are considered virtually unbreakable. 

* A common cryptography definition is the practice of coding information to ensure only the person that a message was written for can read and process the information. This cybersecurity practice, also known as cryptology, combines various disciplines like computer science, engineering, and mathematics to create complex codes that hide the true meaning of a message.
# The Importance of Cryptography
* Cryptography remains important to protecting data and users, ensuring confidentiality, and preventing cyber criminals from intercepting sensitive corporate information.
*  **Common uses and examples of cryptography include the following:**
# Privacy and Confidentiality
* Individuals and organizations use cryptography on a daily basis to protect their privacy and keep their conversations and data confidential. Cryptography ensures confidentiality by encrypting sent messages using an algorithm with a key only known to the sender and recipient. A common example of this is the messaging tool WhatsApp, which encrypts conversations between people to ensure they cannot be hacked or intercepted. 

**Cryptography also secures browsing, such as with virtual private networks (VPNs), which use encrypted tunnels, asymmetric encryption, and public and private shared keys.**
# Authentication

## Integrity

* Similar to how cryptography can confirm the authenticity of a message, it can also prove the integrity of the information being sent and received. Cryptography ensures information is not altered while in storage or during transit between the sender and the intended recipient. For example, digital signatures can detect forgery or tampering in software distribution and financial transactions.

## Nonrepudiation

* Cryptography confirms accountability and responsibility from the sender of a message, which means they cannot later deny their intentions when they created or transmitted information. Digital signatures are a good example of this, as they ensure a sender cannot claim a message, contract, or document they created to be fraudulent. Furthermore, in email nonrepudiation, email tracking makes sure the sender cannot deny sending a message and a recipient cannot deny receiving it.
# Key Exchange

* Key exchange is the method used to share cryptographic keys between a sender and their recipient.

# Types of Cryptographic Algorithms

* There are many types of cryptographic algorithms available. They vary in complexity and security, depending on the type of communication and the sensitivity of the information being shared.

# Secret Key Cryptography

* Secret key cryptography, also known as symmetric encryption, uses a single key to encrypt and decrypt a message. The sender encrypts the plaintext message using the key and sends it to the recipient who then uses the same key to decrypt it and unlock the original plaintext message.

## Stream Ciphers

* Stream ciphers work on a single bit or byte at any time and constantly change the key using feedback mechanisms. A self-synchronizing stream cipher ensures the decryption process stays in sync with the encryption process by recognizing where it sits in the bit keystream. A synchronous stream cipher generates the keystream independently of the message stream and generates the same keystream function at both the sender and the receiver.

## Block Ciphers
* Block ciphers encrypt one block of fixed-size data at a time. It will always encrypt a plaintext data block to the same ciphertext when the same key is used. A good example of this is the Feistel cipher, which uses elements of key expansion, permutation, and substitution to create vast confusion and diffusion in the cipher. 

* The stages of encryption and decryption are similar if not identical, which means reversing the key reduces the code size and circuitry required for implementing the cipher in a piece of software or hardware.

# What Are Cryptographic Key Attacks? What Are the Types?

* Modern cryptographic key techniques are increasingly advanced and often even considered unbreakable. However, as more entities rely on cryptography to protect communications and data, it is vital to keep keys secure. One compromised key could result in regulatory action, fines and punishments, reputational damage, and the loss of customers and investors.

**Potential key-based issues and attack types that could occur include:**

## Weak Keys

* Keys are essentially random numbers that become more difficult to crack the longer the number is. Key strength and length need to be relative to the value of the data it protects and the length of time that data needs to be protected. Keys should be created with a high-quality, certified random number generator that collects entropy—the information density of a file in bits or characters—from suitable hardware noise sources.

## Incorrect Use of Keys

* When keys are used improperly or encoded poorly, it becomes easier for a hacker to crack what should have been a highly secure key.

## Reuse of Keys

* Every key should only be generated for a specific single-use encrypt/decrypt purpose, and use beyond that may not offer the level of protection required.

## Non-rotation of Keys

* Keys that are overused, such as encrypting too much data on a key, become vulnerable to attacks. This is particularly the case with older ciphers and could result in data being exposed. Keys need to be rotated, renewed, and updated when appropriate.

## Inappropriate Storage of Keys

* Storing keys alongside the information they have been created to protect increases their chances of being compromised. For example, keys stored on a database or server that gets breached could also be compromised when the data is exfiltrated.

## Inadequate Protection of Keys

* Huge cyberattacks like Meltdown/Spectre and Heartbleed have been capable of exposing cryptographic keys stored in server memory. Therefore, stored keys must be encrypted and only made available unencrypted when placed within secure, tamper-protected environments, or even kept offline.

## Insecure Movement of Keys

* Moving keys between systems should only occur when the key is encrypted or wrapped under an asymmetric or symmetric pre-shared transport key. If this is not possible, then the key must be split up into multiple parts that are kept separate, re-entered into the target system, then destroyed.

## Insider Threats (User Authentication, Dual Control, and Segregation of Roles)

* Insider threats are one of the most serious threats posed to any key. This is most likely to occur through a rogue employee having access to a key, then using it for malicious purposes or giving or selling it to a hacker or third party.

## Lack of Resilience

* Resilience is vital to protecting the availability, confidentiality, and integrity of keys. Any key that suffers a fault with no backup results in the data the key protects being lost or inaccessible.

## Lack of Audit Logging

* Key life cycles must be logged and recorded in full to ensure any compromise can be tracked and enable subsequent investigations to occur smoothly.

## Manual Key Management Processes

* Recording key management processes manually on paper or spreadsheets runs the risk of human error and makes the keys highly vulnerable to attack or theft.

# How to Minimize the Risks Associated with Cryptography

* Organizations and individuals can minimize and mitigate cryptography-related threats with a dedicated electronic key management system from a reputable provider. The solution must use a hardware security module to generate and protect keys, and underpin the entire system’s security. 

* It needs to include features like full key management life cycle, strong key generation, strict policy-based controls, swift compromise detection, secure key destruction, strong user authentication, secure workflow management, and a secure audit and usage log. This will protect the organization's keys, enhance efficiency, and ensure compliance with data and privacy regulations. 

**Another potential solution is cryptography quantum, whereby it is impossible to copy data encoded in a quantum state.**
