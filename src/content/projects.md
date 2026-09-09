---
id: "projects"
title: "Engineering"
group: "focus"
level: 1
val: 20
date: "2024-01-15"
tags: ["Implementation", "Hardware", "Software"]
projects: ["proj-satellite", "proj-qkey", "proj-dsp-fpga"]
concepts: []
links:
  - "root"
  - "proj-satellite"
  - "proj-qkey"
  - "proj-dsp-fpga"
---

Three projects, three different constraints to design around: cryptography that has to survive quantum computers, a satellite that has to survive low power and orbital mechanics, an audio filter that has to survive FPGA resource limits. What ties them together isn't the domain, it's the same loop: work it out on paper, simulate it, build it, then find out where the theory was wrong.

## Active

- Quantum Key Distribution: post-quantum hybrid QKD protocols, and the deployment problems that don't surface until you try to run one for real.
- CubeSat Communications: a small satellite platform for testing orbital mechanics and low-power comms.
- FPGA Audio Filter: real-time DSP built for resource efficiency and low latency, not just correctness.

## How projects get picked

Mostly by whether it would teach me something a course wouldn't: a real technical obstacle, work that crosses domains instead of sitting in one, and something documented well enough that someone else could pick it up where I left off.
