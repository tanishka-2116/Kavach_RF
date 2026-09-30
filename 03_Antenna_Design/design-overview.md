# Antenna Design Overview

## KAVACH-RF

The KAVACH-RF antenna is being developed as a **low-profile conformal antenna structure** intended for integration with a tactical helmet.

The design is being investigated for operation in two frequency regions:

* **UHF — 446 MHz target**
* **L-band — 1.575 GHz target**

---

## Design Concept

The antenna follows the curvature of the helmet instead of using a conventional externally protruding antenna.

```text
          HELMET SURFACE
       ╭──────────────────╮
      ╱                    ╲
     ╱   CONFORMAL         ╲
    │     ANTENNA           │
    │       LAYER           │
     ╲                    ╱
      ╰──────────────────╯
```

The final geometry will be determined through electromagnetic simulation and physical validation.

---

## Main Design Layers

```text
┌──────────────────────────────┐
│ Protective Layer / Radome    │
├──────────────────────────────┤
│ Conformal Radiator           │
├──────────────────────────────┤
│ Dielectric Substrate         │
├──────────────────────────────┤
│ EBG / AMC Structure          │
├──────────────────────────────┤
│ Bonding / Adhesive Layer     │
├──────────────────────────────┤
│ Helmet Shell                 │
└──────────────────────────────┘
```

---

## Current Design Approach

The development currently uses separate electromagnetic models for the investigated UHF and L-band designs.

### UHF

**Target:** 446 MHz

Current CST simulation:

**522.67 MHz**

Current simulated S11:

**−10.38 dB**

The UHF geometry therefore requires frequency retuning toward the target frequency.

### L-band

**Target:** 1.575 GHz

Current CST simulation:

**1.5755 GHz**

Current simulated S11:

**−2.63 dB**

The L-band model is close to the target frequency, but impedance matching requires further optimization.

---

## Design Workflow

```text
Frequency Target
       ↓
Initial Antenna Geometry
       ↓
Material Selection
       ↓
CST Model
       ↓
S11 / VSWR Analysis
       ↓
Geometry Optimization
       ↓
Helmet Integration
       ↓
Prototype Fabrication
       ↓
Experimental Validation
```

---

## Design Status

| Design |    Target | Current Simulation | Status                |
| ------ | --------: | -----------------: | --------------------- |
| UHF    |   446 MHz |         522.67 MHz | Retuning              |
| L-band | 1.575 GHz |         1.5755 GHz | Matching optimization |

These values represent the current simulation stage and should not be interpreted as final measured prototype performance.

---

## Related Documentation

* [`Antenna Architecture`](antenna-architecture.md)
* [`Frequency Plan`](frequency-plan.md)
* [`Materials`](materials.md)
* [`Simulation`](../04_Simulation/)
