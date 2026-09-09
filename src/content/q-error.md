---
id: "q-error"
title: "Quantum Error Correction"
group: "concept"
level: 2
val: 5
date: "2024-04-20"
tags: ["Quantum", "Error Correction", "Fault-Tolerance"]
links:
  - "quantum-systems"
---

Ways to protect quantum information from decoherence and noise, through encoding schemes and recovery procedures. There's no fault-tolerant quantum computer without it.

## The challenge

Quantum information is fragile. Measuring it, or letting it interact with the environment, destroys coherence. Copying it, the obvious classical fix, is ruled out by the no-cloning theorem.

## Stabilizer codes

Most practical QEC codes use the stabilizer formalism: a stabilizer code encodes $k$ logical qubits in $n$ physical qubits, using stabilizer generators that are multi-qubit Pauli operators.

The surface code is the most studied one, a 2D lattice with local interactions and an error threshold around 1%. The toric code is a topological variant with the same robustness built into its structure. Concatenated codes take a different approach, stacking encodings recursively instead of relying on geometry.

## Error models

The usual error models are bit-flip ($X$ errors), phase-flip ($Z$ errors), depolarization (a random Pauli), and dephasing (loss of coherence).

## Threshold theorem

Below a critical error threshold $p_t$, the logical error rate drops exponentially as code distance increases. That's what makes arbitrarily accurate computation possible even with fixed, noisy physical qubits.

## Current status

Realized experimentally in trapped ions and superconducting qubits, at a cost of hundreds to thousands of physical qubits per logical qubit. Most active research is aimed at bringing that overhead down.
