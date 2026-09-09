---
id: "propulsion"
title: "Ionic Propulsion"
group: "concept"
level: 2
val: 5
date: "2024-06-05"
tags: ["Space", "Propulsion", "Physics"]
links:
  - "orbital-mechanics"
---

Electric propulsion systems accelerating ionized propellant to extremely high velocities, achieving high specific impulse for efficient long-duration space missions. Critical for beyond-LEO operations and spacecraft with limited fuel budgets.

## Physics principles

Ionic propulsion generates thrust through:

$$F = \dot{m} v_e + (P_e - P_a)A_e$$

where $\dot{m}$ is mass flow rate, $v_e$ is exhaust velocity, and $P_e$ is exit pressure.

By ionizing propellant and accelerating it electrostatically or electromagnetically, exhaust velocities reach 20-50 km/s, against roughly 4 km/s for chemical propulsion.

## Advantages

Specific impulse runs 2000-5000 seconds, versus 300-450s for chemical engines, which is the whole reason ion drives exist: a spacecraft that can afford to burn slowly gets far more delta-v per kilogram of propellant. That trades into extended operations on limited propellant, precise maneuvers at low thrust, and a long operational life since there's no combustion, only gradual electrode wear.

## System components

An ionization stage produces plasma, either by electron bombardment or microwave excitation. An acceleration region then pushes the ions with an electric or magnetic field. A neutralizer fires electrons into the exhaust so the spacecraft doesn't accumulate charge, and a power supply, usually solar arrays or a nuclear reactor, drives the whole thing.

## Challenges

Thrust sits in the millinewton range, so missions need long duration burns to get anywhere. Plasma from the plume interacts with spacecraft surfaces and instruments, ion bombardment erodes electrodes over time, and high-power systems demand more power than most spacecraft can easily supply.

## Heritage missions

- Deep Space 1 (ion drive validation)
- Dawn (asteroid missions)
- GOSAT-2 and other satellite stations

## Future development

- Hall-effect thrusters (higher power)
- Field-emission electric propulsion
- Nuclear electric propulsion
