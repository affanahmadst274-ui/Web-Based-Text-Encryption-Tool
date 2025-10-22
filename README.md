# 🔐 Web-Based Text Encryption Tool

A single-page web app that lets users **encrypt, decrypt, and hash text** using multiple algorithms — built with **HTML, CSS, and JavaScript (CryptoJS)**.

---

## 🚀 Features

✅ **Encryption & Decryption Algorithms**
- Caesar Cipher (shift cipher)
- Base64 Encode/Decode
- AES Encryption (password-based)
- DES Encryption (password-based)

✅ **Hashing**
- SHA-256 (one-way hashing)

✅ **Extras**
- Copy ciphertext button
- Download result as `.txt`
- Input validation (empty checks, password required for AES/DES)

---

## 🖥️ Tech Stack

| Layer | Tools / Libraries |
|-------|--------------------|
| Frontend | HTML, CSS, JavaScript |
| Crypto Library | [CryptoJS 4.1.1 CDN](https://cdnjs.com/libraries/crypto-js) |
| Optional Backend | Node.js / Flask (not required for base version) |

---

## 📸 Screenshot

![App Preview](https://via.placeholder.com/900x400?text=Web-Based+Text+Encryption+Tool)

*(Add your real screenshot later — open app, take a screenshot, and upload to GitHub)*

---

## 🧠 Algorithms Used

### 1. Caesar Cipher
A basic substitution cipher that shifts letters by a fixed number (e.g., shift = 3 → “A” becomes “D”).

### 2. Base64
Encodes text to ASCII-safe characters; reversible using decoding.

### 3. AES (Advanced Encryption Standard)
Symmetric encryption algorithm using passphrase-derived keys. Implemented via CryptoJS AES module.

### 4. DES (Data Encryption Standard)
Block cipher using symmetric key encryption (demo purpose).

### 5. SHA-256
A secure one-way hashing algorithm — cannot be decrypted.

---

## ⚙️ How to Run

### 🟩 Option 1: Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/web-text-encryption-tool.git
