#  Short Report — Web-Based Text Encryption Tool

##  Objective
The objective of this project is to develop a **web-based text encryption and decryption tool** that allows users to secure their messages using multiple encryption algorithms.  
The system demonstrates how **cryptography** can protect data confidentiality through symmetric and asymmetric encryption, encoding, and hashing techniques.

---

##  Introduction
With the rapid growth of online communication, securing textual information has become essential.  
This project presents a **single-page web application** that lets users:
- Enter plaintext,
- Select an encryption algorithm,
- Encrypt or decrypt text instantly on the browser using **JavaScript (CryptoJS library)**.

It also provides a **hashing feature (SHA-256)** for irreversible message verification.

---

##  Tools and Technologies
| Component | Technology |
|------------|-------------|
| Frontend | HTML5, CSS3, JavaScript (ES6) |
| Encryption Library | [CryptoJS 4.1.1](https://cdnjs.com/libraries/crypto-js) |
| Optional Backend | Node.js (Express) or Python (Flask) |
| Platform | Web Browser |
| Hosting | GitHub Pages (recommended) |

---

##  Algorithms Implemented

### 1. Caesar Cipher
- **Type:** Classical substitution cipher  
- **Description:** Shifts each character in the plaintext by a fixed number (e.g., shift = 3).  
- **Example:**  
  Plaintext: `HELLO`  
  Ciphertext: `KHOOR`  
- **Decryption:** Reverse the shift.

---

### 2. AES (Advanced Encryption Standard)
- **Type:** Symmetric-key block cipher  
- **Library Used:** `CryptoJS.AES`  
- **Mechanism:** Encrypts plaintext with a user-provided passphrase.  
- **Features:**  
  - 128-bit, 192-bit, or 256-bit encryption  
  - Strong industry-standard security  
- **Example:**  
  Input: `HELLO`, Key: `1234` → `U2FsdGVkX1+Lk...`

---

### 3. DES (Data Encryption Standard)
- **Type:** Symmetric-key block cipher  
- **Library Used:** `CryptoJS.DES`  
- **Purpose:** Demonstrates older encryption model for comparison.  
- **Note:** Less secure than AES, included for educational purpose.

---

### 4. Base64 Encoding
- **Type:** Text-to-ASCII encoding (not true encryption)  
- **Use Case:** Converts binary data to printable ASCII for safe transmission.  
- **Example:**  
  Input: `HELLO` → Output: `SEVMTE8=`

---

### 5. SHA-256 Hashing
- **Type:** One-way hashing function  
- **Library Used:** `CryptoJS.SHA256`  
- **Purpose:** Generates a fixed-length digest — cannot be decrypted.  
- **Example:**  
  Input: `HELLO` → Output: `185f8db32271fe25f561a6fc938b2e264306ec304eda518007d1764826381969`

---

##  Key Features
- Encrypt and decrypt text using different algorithms  
- SHA-256 hashing option  
- Input validation (no empty text, password required for AES/DES)  
- Copy ciphertext button  
- Responsive design with dark/light mode support  
- Runs entirely in the browser (no server required)

---

##  Results
| Algorithm | Example Input | Example Output | Type |
|------------|----------------|----------------|-------|
| Caesar Cipher | HELLO | KHOOR | Reversible |
| Base64 | HELLO | SEVMTE8= | Reversible |
| AES | HELLO (key=1234) | U2FsdGVkX1+9Gf... | Reversible |
| DES | HELLO (key=1234) | U2FsdGVkX19VgD... | Reversible |
| SHA-256 | HELLO | 185f8db3...81969 | Non-Reversible |

All algorithms worked correctly and produced expected results for encryption, decryption, and hashing.

---

##  Learning Outcomes
- Understood core principles of **cryptography**: symmetric vs. asymmetric encryption, encoding, and hashing.  
- Implemented multiple algorithms in **pure JavaScript** using CryptoJS.  
- Learned how to build a responsive web app and integrate encryption logic with UI elements.  
- Gained experience with **client-side validation** and **user-friendly interaction** design.

---

##  Conclusion
The project successfully demonstrates how encryption and decryption can be implemented in a web-based interface using modern JavaScript libraries.  
Users can protect sensitive text using AES or DES, apply reversible ciphers like Caesar, or generate irreversible SHA-256 hashes.  
This tool highlights the importance of encryption in modern web security and provides a simple yet effective educational demonstration.

---

##  Author
**Name:** *Affan Ahmad*  
**Roll Number:** *03-134221-003*  
**Course:** Infromation Security  
**Institution:** *Bahria University Lahore *  
**GitHub Repository:** [https://github.com/affanahmadst274-ui/web-text-encryption-tool](https://github.com/affanahmadst274-ui.github.io/web-text-encryption-tool)
