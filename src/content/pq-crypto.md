---
id: "pq-crypto"
title: "Post-Quantum Cryptography"
group: "concept"
level: 2
val: 5
date: "2024-05-05"
tags: ["Cryptography", "Quantum Safety", "Standards"]
links:
  - "cryptography"
  - "quantum-systems"
---

Cryptographic algorithms resistant to attacks by both classical and quantum computers. As quantum computing advances, post-quantum cryptography becomes essential for long-term data security.

## Threat model

Quantum computers running Shor's algorithm can factor large integers and solve discrete logarithm problems in polynomial time, which breaks RSA and ECC outright. PQC schemes resist both classical and quantum adversaries.

## Leading candidates

### Lattice-based cryptography
Built on hard problems over lattices (LWE, Ring-LWE). The fastest and most versatile family, with applications in encryption, signatures, and zero-knowledge proofs.

### Multivariate polynomial cryptography
Security rests on solving multivariate quadratic equations. Small signature sizes, but slower operations.

### Code-based cryptography
Based on the hardness of decoding random linear codes. Proven secure for decades, but large key sizes.

### Hash-based signatures
Unconditionally secure, requiring only collision-resistant hash functions. Limited signatures per key, but deterministic security.

## Standards and deployment

NIST has standardized post-quantum algorithms (ML-KEM, ML-DSA, SLH-DSA) for hybrid deployment alongside classical schemes during the transition period.

## Implementation challenges

- Integration with existing systems
- Performance trade-offs
- Key size management
- Backward compatibility
