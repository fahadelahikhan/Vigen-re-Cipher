# Vigenère Cipher 🔒

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A Python implementation of the **Vigenère cipher** — a polyalphabetic substitution cipher that uses dynamic keyword-based encryption/decryption.

## 📜 About
The Vigenère cipher is a classic cryptographic method that enhances security compared to simple substitution ciphers. It encrypts text by shifting letters according to a repeating keyword, making frequency analysis attacks harder.

## ✨ Features
- Encrypt/decrypt text with a custom keyword
- Preserves spaces and punctuation
- Case-insensitive input handling
- Simple command-line execution

## 🚀 Quick Start

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Vigenere-Cipher.git
   cd Vigenere-Cipher
   

### Basic Usage
```python
# Import functions
from vigenere import encrypt, decrypt

message = "Hello World!"
key = "SECRET"

# Encrypt
encrypted = encrypt(message, key)  # Output: "dlwor aeptl!"

# Decrypt
decrypted = decrypt(encrypted, key)  # Output: "hello world!"
```

### Example Decryption
```python
encrypted_text = "mrttaqrhknsw ih puggrur"
custom_key = "happycoding"

decrypted_text = decrypt(encrypted_text, custom_key)
print(decrypted_text)  # Output: "freecodecamp is awesome"
```

## 📖 Documentation
### How It Works
- **Encryption**: `(plaintext_char + key_char) mod 26`
- **Decryption**: `(ciphertext_char - key_char) mod 26`

Non-alphabetic characters (spaces, punctuation) remain unchanged during processing.

## ⚖️ License
Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

> **Note**: While historically significant, the Vigenère cipher is **not secure** for modern cryptographic needs. Use for educational purposes only.

