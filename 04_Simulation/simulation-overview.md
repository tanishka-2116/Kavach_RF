# Simulation & Electromagnetic Validation

## Purpose

CST Studio Suite is being used to investigate the electromagnetic behaviour of the proposed KAVACH-RF antenna designs before physical fabrication.

The current development investigates two frequency regions:

* **UHF — 446 MHz target**
* **L-band — 1.575 GHz target**

---

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
Prototype Fabrication
       ↓
VNA Validation
```

---

## UHF Simulation

**Target:** 446 MHz

**Current simulated resonance:** 522.67 MHz

**Current S11:** approximately −10.38 dB

The current UHF design shows a resonant response, but the resonance is shifted above the intended 446 MHz target.

**Current status:** Frequency retuning required.

[View detailed UHF simulation →](uhf-simulation.md)

---

## L-band Simulation

**Target:** 1.575 GHz

**Current simulated resonance:** approximately 1.5755 GHz

The L-band model produces a resonance close to the intended target frequency.

The S11 response is documented in the detailed L-band simulation page.

**Current status:** Impedance and geometry optimization ongoing.

[View detailed L-band simulation →](l-band-simulation.md)

---

## Simulation Summary

| Band   |    Target | Current Simulation | Development Status |
| ------ | --------: | -----------------: | ------------------ |
| UHF    |   446 MHz |         522.67 MHz | Frequency retuning |
| L-band | 1.575 GHz |        ~1.5755 GHz | Optimization       |

---

## What the Simulation Establishes

The current CST work provides:

* Initial electromagnetic models
* Resonant-frequency information
* S11 response analysis
* A basis for geometry optimization
* A reference for comparison with the physical prototype

These results represent the **current simulation stage** and are not final measured prototype performance.

---

## Planned Experimental Validation

After optimization and fabrication, the antenna will be evaluated experimentally.

```text
CST Simulation
      ↓
Optimized Design
      ↓
Prototype Fabrication
      ↓
Helmet Integration
      ↓
VNA Measurement
      ↓
Measured S11 / VSWR
      ↓
Simulation vs Measurement
```

The measured results will be used to determine how closely the physical prototype matches the simulated design.

---

## Related Documentation

* [`UHF Simulation`](uhf-simulation.md)
* [`L-band Simulation`](l-band-simulation.md)
* [`Antenna Design`](../03_Antenna_Design/)
* [`Frequency Plan`](../03_Antenna_Design/frequency-plan.md)
