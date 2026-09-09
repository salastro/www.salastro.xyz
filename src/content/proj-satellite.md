---
id: "proj-satellite"
title: "CubeSat Comms"
group: "project"
level: 2
val: 7
date: "2024-08-10"
tags: ["CubeSat", "Communications", "Space"]
concepts: ["orbital-mechanics", "propulsion"]
links:
  - "projects"
  - "orbital-mechanics"
---

Design and implementation of communication protocols and orbital mechanics optimization for a 3-unit CubeSat platform. Focus on developing robust low-power communication algorithms and trajectory optimization for station-keeping.

## Mission overview

### Objectives

1. Communications: reliable command uplink and data downlink
2. Orbital operations: optimized station-keeping maneuvers for extended mission life
3. Propulsion: ionic propulsion for orbital adjustment
4. Science: radiation and plasma environment data collection

### Spacecraft parameters

- Mass: ~4 kg
- Power: solar cells, ~15W average
- Propulsion: ion thruster, 5mN nominal
- RF: UHF downlink, S-band uplink

## Technical challenges

- Power budget: limited solar power means careful scheduling of comms windows and computation
- Thermal management: temperature swings in LEO require passive and active thermal control
- Radiation: SEE-sensitive components need filtering and redundant architecture
- Orbital decay: atmospheric drag means periodic reboost maneuvers

## Development phases

1. Ground station network: develop and integrate receiving stations worldwide
2. Component qualification: test electronics in a thermal-vacuum chamber
3. System integration: assembly and functional testing
4. Pre-launch validation: final checkout and launch readiness
5. Mission operations: orbital deployment and data collection

## Expected outcomes

- Open-source spacecraft software and firmware
- Communications protocol documentation
- Ionization thruster performance characterization
- Radiation environment measurements
