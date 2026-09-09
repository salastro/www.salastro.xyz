---
id: "cryptography"
title: "Cryptography"
group: "focus"
level: 1
val: 10
date: "2024-02-20"
img: "https://images.unsplash.com/photo-1770159116807-9b2a7bb82294?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwxfHxjcnlwdG9ncmFwaHklMjBkYXRhJTIwc2VjdXJpdHklMjBjb2RlJTIwZGFya3xlbnwxfHx8fDE3NzA4MjI5NjV8MA&ixlib=rb-4.1.0&q=80&w=1080"
tags: ["Security", "Privacy", "Math"]
projects: ["proj-qkey"]
concepts: ["zkp", "ecc"]
equations:
  - 'P(A(g^a, g^b) = g^{ab}) \approx \frac{1}{|G|}'
  - '\text{Enc}_{pk}(m) \rightarrow c'
links:
  - "projects"
  - "math"
  - "zkp"
  - "pq-crypto"
  - "ecc"
---

Secure communication in the presence of adversarial behavior. Specifically interested in post-quantum cryptographic primitives and zero-knowledge proofs for privacy-preserving systems.

## Core principles

Modern cryptography rests on computational hardness assumptions. A scheme's security is measured against polynomial-time adversaries with bounded computational resources.

## Post-quantum considerations

As quantum computers improve, lattice-based cryptography and hash-based signatures are the leading candidates to replace RSA and ECC for long-term security.

## Applications

Privacy-preserving protocols including zero-knowledge proofs enable verifiable computation without revealing sensitive inputs, with applications in decentralized identity and secure multi-party computation.
