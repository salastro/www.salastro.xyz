---
id: "proj-qkey"
title: "QKD Protocol Impl"
group: "project"
level: 2
val: 7
date: "2024-09-15"
tags: ["QKD", "Cryptography", "Quantum"]
concepts: ["cryptography", "quantum-systems", "zkp", "pq-crypto"]
links:
  - "projects"
  - "cryptography"
  - "quantum-systems"
---

Implementation of post-quantum hybrid quantum key distribution protocols combining quantum and classical cryptographic primitives for enhanced security against both current and future adversaries.

## Protocol design

### Hybrid approach

Combines a quantum component (BB84 or Ekert '91 for key generation), a classical component (a post-quantum KEM for the classical channel), and zero-knowledge proofs for entity authentication.

The final key is the XOR of both components, so both the quantum and classical channels have to be secure for the whole thing to hold.

### Security properties

- Quantum advantage: eavesdropping on the quantum channel leaves detectable traces
- Post-quantum safety: resistant to quantum computing attacks
- Forward secrecy: compromised long-term keys don't expose past sessions

## Implementation challenges

- Experimental apparatus: needs quantum optics (single-photon sources, detectors) and classical networking
- Timing synchronization: quantum and classical channels have to stay precisely synced
- Loss and detection: photon losses in the channel cut the key generation rate
- Real-time processing: sifted key extraction needs fast classical post-processing

## Platform targets

- Chip-scale: integrated photonics on silicon
- Free-space: satellite-ground links
- Fiber: metropolitan area networks

## Expected outcomes

- Working prototype implementation
- Performance characterization (throughput, error rates, range)
- Integration standards for hybrid systems
- Security analysis against defined threat models

## Deliverables

- Open-source software implementation
- Hardware design files
- Security proofs and analysis
- User documentation and tutorials
