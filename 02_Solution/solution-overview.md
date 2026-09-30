# Proposed Solution

## KAVACH-RF

KAVACH-RF proposes a **helmet-mounted conformal antenna platform** for tactical communication requirements in urban CQB environments.

The approach replaces the dependence on a conventional protruding antenna with a **low-profile antenna structure integrated with the helmet geometry**.

---

## Core Concept

The proposed antenna platform investigates a dual-band architecture:

| Band   | Target Frequency | Intended Link                |
| ------ | ---------------: | ---------------------------- |
| UHF    |      **446 MHz** | Tactical radio communication |
| L-band |    **1.575 GHz** | Video / camera communication |

The final antenna geometry and matching network will be optimized through electromagnetic simulation and physical testing.

---

## Proposed Antenna Stack

The current concept consists of multiple functional layers:

```text
        ┌──────────────────────────┐
        │ Protective / Radome Layer│
        ├──────────────────────────┤
        │   Conformal Radiator     │
        ├──────────────────────────┤
        │       EBG / AMC          │
        ├──────────────────────────┤
        │ Flexible Dielectric      │
        ├──────────────────────────┤
        │      Helmet Shell        │
        └──────────────────────────┘
```

The layered structure is intended to support compact integration while allowing the RF characteristics to be optimized.

---

## Design Objectives

The solution is being developed around the following objectives:

* Low-profile helmet integration
* Compact antenna architecture
* Reduced external protrusion
* Dual-band operation investigation
* Controlled radiation characteristics
* Improved integration with the communication platform
* Simulation-based optimization
* Experimental RF validation

---

## Development Strategy

```text
                    KAVACH-RF
                        │
          ┌─────────────┴─────────────┐
          │                           │
        UHF                         L-band
     446 MHz                       1.575 GHz
          │                           │
          └─────────────┬─────────────┘
                        ↓
                Antenna Architecture
                        ↓
                  CST Simulation
                        ↓
                 Optimization
                        ↓
                Physical Prototype
                        ↓
                 VNA Validation
```

---

## Current Design Status

The initial CST model has produced resonances in both investigated frequency regions.

### UHF

* Target: **446 MHz**
* Current simulated resonance: **522.67 MHz**
* Current S11: **−10.38 dB**
* Status: **Frequency retuning required**

### L-band

* Target: **1.575 GHz**
* Current simulated resonance: **1.5755 GHz**
* Current S11: **−2.63 dB**
* Status: **Impedance matching optimization required**

These are current simulation results and are not final experimental performance claims.

---

## Next Engineering Step

The immediate design work is:

1. Retune the UHF resonance toward 446 MHz.
2. Improve L-band impedance matching.
3. Finalize the material stack.
4. Fabricate the antenna.
5. Integrate it with the helmet.
6. Measure the prototype using a VNA.
7. Compare measured and simulated results.

---

## Related Documentation

* [`System Architecture`](system-architecture.md)
* [`Working Principle`](working-principle.md)
* [`Antenna Design`](../03_Antenna_Design/)
* [`Simulation`](../04_Simulation/)
