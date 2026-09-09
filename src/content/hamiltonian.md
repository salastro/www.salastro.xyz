---
id: "hamiltonian"
title: "Hamiltonian Simulation"
group: "concept"
level: 2
val: 5
date: "2024-04-25"
tags: ["Quantum", "Simulation", "Algorithms"]
links:
  - "quantum-systems"
---

Quantum algorithms for simulating the evolution of quantum systems under Hamiltonian dynamics. It's one of the oldest arguments for building a quantum computer at all: quantum chemistry, materials science, and lattice gauge theory simulations all reduce to it eventually.

## Problem statement

Given a Hamiltonian $H$ and time $t$, implement the unitary evolution

$$U(t) = e^{-iHt}$$

on a quantum computer to accuracy $\epsilon$.

## Classical difficulty

For sparse Hamiltonians on $n$ qubits, direct classical simulation takes effort exponential in $n$. That gap is the whole motivation.

## Quantum algorithms

### Product formula (Trotter-Suzuki)
Decomposes $H = \sum_j H_j$ into terms that are each easy to simulate:

$$e^{-i(H_1+H_2)t} \approx \left(e^{-iH_1 t/r}e^{-iH_2 t/r}\right)^r$$

Simple, but the gate counts get large.

### LCU methods
Linear Combination of Unitaries. Higher query complexity than product formulas, but better asymptotic scaling.

### Qubitization
Encodes the Hamiltonian into the spectral gaps of unitary operators. Near-optimal query complexity.

## Applications

Mostly chemistry: molecular spectroscopy, reaction dynamics, drug discovery, battery and catalyst design. Outside chemistry, the two that come up most are materials-property prediction and lattice QFT simulation.

## Resource requirements

Current hardware would need millions of physical qubits for a chemistry simulation that actually matters. Nowhere close to that yet.
