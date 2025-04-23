# 🔐 Secure File Encryptor & Decryptor

A lightweight yet secure command-line application that allows users to encrypt and decrypt files using AES encryption. Ideal for protecting sensitive documents and ensuring safe file transfers.

## 🧠 About

This tool was developed as a simple, fast, and effective solution to securely encrypt and decrypt files. It uses the AES (Advanced Encryption Standard) algorithm in CBC mode, ensuring robust data protection. The encrypted files are saved with a `.enc` extension, and decrypted files are restored with their original name and content.

## ✨ Features

- 🔒 AES-256 Encryption for top-tier security  
- 📁 Handles both text and binary files  
- 🔑 Password-based key derivation using PBKDF2  
- 💡 Simple command-line interface  
- 🚀 Fast and reliable performance

## 📦 Requirements

- Python 3.6+
- `pycryptodome` package

Install dependencies using:

```bash
pip install pycryptodome
```

## ⚙️ Usage

### 🔐 Encrypt a File

```bash
python encryptor.py -e <file_path>
```

You will be prompted to enter a password for encryption.

### 🔓 Decrypt a File

```bash
python encryptor.py -d <encrypted_file_path>
```

You will be prompted to enter the same password used during encryption.

## 🛠️ How It Works

- The AES-256 algorithm is used in CBC (Cipher Block Chaining) mode.
- A random 16-byte IV (Initialization Vector) is generated for every encryption operation.
- The password is transformed into a 32-byte key using PBKDF2 with a random salt and multiple iterations.
- The IV and salt are stored at the beginning of the encrypted file to facilitate decryption.

## 📂 Project Structure

```plaintext
.
├── encryptor.py         # Main script to encrypt/decrypt files
├── README.md            # Documentation file
```

## 👨‍💻 Developed By

**Aayush Vishwakarma**  
B.Tech CSE | IET Lucknow  
[LinkedIn](https://www.linkedin.com/in/aayush-vishwakarma-68a8a92a1/)
