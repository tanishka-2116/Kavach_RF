# Simulation & Electromagnetic Validation

## Purpose

CST Studio Suite is being used to investigate the electromagnetic behaviour of the proposed KAVACH-RF antenna designs before physical fabrication.

The simulations currently cover two frequency regions:

* **UHF — 446 MHz target**
* **L-band — 1.575 GHz target**

## Simulation Workflow

```text
Antenna Geometry
       ↓
Material Definition
       ↓
Feed / Port Definition
       ↓
CST Electromagnetic Simulation
       ↓
S11 / Resonance Analysis
       ↓
Geometry Optimization
       ↓
Prototype Validation
```

## Current Simulation Evidence

### UHF

The current UHF model shows a simulated resonance at **522.67 MHz** with an S11 of approximately **−10.38 dB**.

The design is being optimized toward the **446 MHz target**.

### L-band

The current L-band model operates close to the **1.575 GHz target**.

The L-band geometry still requires impedance-matching optimization.

## Important Note

The values documented here are **simulation results**, not final measured prototype results.

Experimental validation will be performed using RF measurement equipment after prototype fabrication.
