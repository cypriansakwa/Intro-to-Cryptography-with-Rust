# Intro to Cryptography with Rust

## Overview
This project demonstrates how to implement basic cryptographic concepts using Rust. It includes examples of encrypting and decrypting messages using the `ChaCha20-Poly1305` AEAD cipher.

## Prerequisites
- Rust 1.50 or higher
- `cargo` for building and running the project

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/cryptography-with-rust.git
   cd cryptography-with-rust
## Build the project:
```bash
cargo build --release
```
## Run the example:
```bash
cargo run
```
## Usage

The program demonstrates how to:

- Generate a key and nonce  
- Encrypt a plaintext message  
- Decrypt the ciphertext to recover the original message

## Example Output

```bash
Encryption done. Check ciphertext.bin  
Decryption done. Check decrypted.txt
```
## 🔐 Security Notes

- ✅ The key and nonce never leave memory.  
- ✅ The nonce is unique per encryption to prevent security vulnerabilities.  
- ⚠️ For real-world use, consider integrating with a secure key management system (KMS).  
- 🚫 Never reuse a nonce with the same key.

## 📚 References

- [ChaCha20Poly1305 crate documentation](https://docs.rs/chacha20poly1305)
- [RFC 8439: ChaCha20 and Poly1305 for IETF Protocols](https://datatracker.ietf.org/doc/html/rfc8439)
