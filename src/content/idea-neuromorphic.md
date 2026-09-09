---
id: "idea-neuromorphic"
title: "Neuromorphic Circuits"
group: "idea"
level: 2
val: 4
date: "2024-07-10"
tags: ["Bio-Inspired", "Hardware", "Computing"]
links:
  - "ideas"
---

Bio-inspired computing hardware that emulates neural structures and processes instead of a conventional digital layout. For some workloads it can be orders of magnitude more energy-efficient than standard digital hardware.

## Motivation

The brain runs vision, reasoning, and learning on about 20 watts. Digital processors need kilowatts for comparable computation. That gap alone says something is architecturally wrong with how we build computers.

## Spiking neural networks

Neurons communicate through discrete, precisely-timed spikes, closer to how biological neurons actually work than a standard artificial neural network. The upside: computation only happens when a spike does, so the network is naturally sparse and encodes information in timing, not just magnitude. The downside: training SNNs is harder than training ordinary ANNs, the theory behind them is thinner, and the hardware to run them is more complex to build.

## Analog computing

Uses continuous physical quantities, voltage or current, instead of digital logic. That buys inherent parallelism and low power for free, at the cost of the precision and reproducibility digital circuits give you by default.

## Technical approaches

Memristors are two-terminal devices whose resistance depends on history, which makes them a natural fit for synaptic connections. Phase-change materials store information densely by exploiting phase transitions. Photonic circuits use light for computation that's both fast and low-energy. Mixed-signal designs combine analog processing with digital control to get some of both worlds.

## Open problems

Fabricating complex analog circuits reliably is still hard, and so is handling component variation and noise without losing the efficiency gains. Designing algorithms that actually exploit the hardware, rather than just porting a digital algorithm onto it, is its own open problem. There's also no agreed way to benchmark neuromorphic systems against digital ones, since the usual metrics assume digital semantics.

## Potential applications

Always-on sensing, robotics, pattern recognition on resource-constrained devices, edge AI inference. Anywhere the power budget is the actual bottleneck, not raw throughput.

## Current status

Intel's Loihi 2 and IBM's TrueNorth are the two names that keep coming up, both still research systems rather than anything you'd deploy. Beyond that it's academic prototypes and demonstrations, nothing close to a general-purpose neuromorphic computer yet.
