# **Chapter 8**

---

### What is the most secure computer in the world?
**A:** The one that is not connected to the internet, located in a secure room, and guarded by armed personnel.

---

## What is Network Security?

### CIA Triad and AAA Model

#### CIA Triad (Information Security Model)
- **Confidentiality**: Information is only accessible to the intended person.
- **Integrity**: Information is correct and untampered with.
- **Availability**: Information is accessible when needed.
- These three principles are the cornerstone of security infrastructure and the tenets of cybersecurity.

#### AAA Model
- Methods to achieve cybersecurity objectives:
    - **Authentication**: Are you the person intended to view this information?
    - **Authorization**: Are you authorized to read, write, and execute?
    - **Accountability**: Are you accountable for what happens to the computer system?

---

## Friends and Enemies: Alice, Bob, and Trudy

- **Alice (A)** and **Bob (B)** are communicating, while **Trudy (T)** is the intruder.
- What can a bad actor do?
    - **Eavesdrop**: Intercept communication (e.g., opening cars without the key).
    - **Insert Messages**: Inject messages into the connection.
    - **Impersonation**: Pretend to be someone else.
    - **Hijacking**: Take over a session.
    - **Denial of Service (DoS)**: Disrupt service availability.

---

## Breaking Encryption Schemes

### Cipher-Only Attack
- Trudy has ciphertext to analyze.
- Two approaches:
    - **Brute Force**: Search through all possible keys.
    - **Statistical Analysis**: Use patterns to break encryption.

### Known-Plaintext Attack
- Trudy has plaintext corresponding to ciphertext.

---

## Symmetric Key Cryptography

- A cryptographic method where the same key is used for both encryption and decryption.

