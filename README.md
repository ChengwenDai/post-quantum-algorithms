# Post-Quantum Cryptography Algorithms

## Introduction

This project demonstrates two post-quantum cryptography algorithms:

- ML-KEM (Module-Lattice-Based Key-Encapsulation Mechanism)
- ML-DSA (Module-Lattice-Based Digital Signature Algorithm)

The project was developed as part of a Post-Quantum Cryptography workshop.

The purpose of this project is to demonstrate how post-quantum algorithms can be used for secure key establishment and digital signatures.

## Algorithms

### ML-KEM

ML-KEM is a post-quantum key-encapsulation mechanism based on module lattices.

In this demonstration:

1. Alice generates a public key and a private/decapsulation key.
2. Bob uses Alice's public key to generate a shared secret and ciphertext.
3. Alice uses her private/decapsulation key to recover the shared secret.
4. The two shared secrets are compared to confirm successful key establishment.

The demonstration uses ML-KEM-768.

### ML-DSA

ML-DSA is a post-quantum digital signature algorithm based on module lattices.

In this demonstration:

1. A public key and secret key are generated.
2. A message is signed using the secret key.
3. The signature is verified using the public key.
4. The program reports whether the signature is valid.

The demonstration uses ML-DSA-65.

## Project Structure

```text
post-quantum-algorithms/
├── mlkem_demo.py
├── mldsa_demo.py
├── README.md
└── .gitignore
