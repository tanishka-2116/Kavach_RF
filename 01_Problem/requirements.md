# Project Requirements

## SIH26185 — KAVACH-RF

This document converts the problem statement into the main engineering requirements for the project.

---

## 1. Functional Requirements

The antenna system should:

* Be suitable for helmet integration.
* Maintain a low-profile form factor.
* Follow or accommodate the helmet curvature.
* Provide an RF interface to the communication system.
* Support investigation of UHF operation.
* Support investigation of L-band operation.
* Allow RF performance to be measured experimentally.

---

## 2. RF Requirements

| Parameter        | Requirement / Target              |
| ---------------- | --------------------------------- |
| UHF target       | **446 MHz**                       |
| L-band target    | **1.575 GHz**                     |
| System impedance | **50 Ω**                          |
| Target S11       | **≤ −10 dB**                      |
| Target VSWR      | **≤ 2:1**                         |
| Radiation        | Controlled / application-oriented |
| Validation       | Simulation + measurement          |

> The frequency and performance values above represent the current project targets. They are not final measured prototype results.

---

## 3. Mechanical Requirements

The antenna should:

* Maintain a compact profile.
* Avoid a conventional protruding whip configuration.
* Be compatible with helmet curvature.
* Use a lightweight implementation where practical.
* Allow secure mounting and RF-feed routing.

---

## 4. Material Requirements

The current project approach investigates:

* Flexible dielectric substrate
* Conductive radiator
* EBG / AMC structures
* RF connector and feed
* Protective outer layer / radome

The selected material stack will be finalized during the design and fabrication stages.

---

## 5. Simulation Requirements

The antenna should be evaluated using electromagnetic simulation for:

* Resonant frequency
* S11
* VSWR
* Impedance matching
* Radiation pattern
* Gain
* Efficiency
* Helmet integration effects

The current project workflow uses **CST Studio Suite**, with HFSS considered as an additional simulation platform.

---

## 6. Validation Requirements

After simulation, the physical prototype should be evaluated using appropriate RF measurement equipment.

Planned validation includes:

```text
Prototype
   ↓
VNA Calibration
   ↓
S11 Measurement
   ↓
VSWR
   ↓
Resonant Frequency
   ↓
Bandwidth
   ↓
Radiation Pattern
   ↓
Simulation vs Measurement
```

---

## 7. Current Simulation Baseline

The current CST results provide the initial engineering baseline:

| Band   |    Target | Current Simulation |       S11 | Action           |
| ------ | --------: | -----------------: | --------: | ---------------- |
| UHF    |   446 MHz |         522.67 MHz | −10.38 dB | Retune frequency |
| L-band | 1.575 GHz |         1.5755 GHz |  −2.63 dB | Improve matching |

These values represent the **current simulation stage** and will be updated as the design is optimized and experimentally validated.

---

## 8. Success Criteria

The project will progress toward a validated prototype when:

* The antenna is physically integrated with the helmet.
* Target frequencies are approached through simulation optimization.
* Impedance matching meets the defined target.
* RF performance is measured experimentally.
* Simulation and measurement results are compared.
* Design deviations are analyzed and corrected.

---

## Next Stage

**Requirements → Antenna Architecture → Simulation → Prototype**

Next documentation:

[`02_Solution`](../02_Solution/)
