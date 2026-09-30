# Frequency Plan

## KAVACH-RF

KAVACH-RF currently investigates two RF operating regions:

| Band   | Target Frequency | Current Simulation | Current Status              |
| ------ | ---------------: | -----------------: | --------------------------- |
| UHF    |      **446 MHz** |     **522.67 MHz** | Frequency retuning required |
| L-band |    **1.575 GHz** |     **1.5755 GHz** | Impedance matching required |

---

## 1. UHF Design

### Target

**446 MHz**

The UHF section is being investigated as the lower-frequency communication antenna.

### Current CST Result

The present simulation shows a resonance at:

**522.67 MHz**

with:

**S11 = −10.38 dB**

The simulated resonance is therefore above the current 446 MHz target.

### Current Engineering Task

The UHF geometry needs to be optimized to shift the resonant frequency toward **446 MHz** while maintaining acceptable impedance matching.

```text
Target
446 MHz
   │
   ▼
Current Design
522.67 MHz
   │
   ▼
Geometry / Matching Optimization
   │
   ▼
Retuned UHF Design
```

---

## 2. L-band Design

### Target

**1.575 GHz**

### Current CST Result

The present L-band simulation shows a resonance at approximately:

**1.5755 GHz**

The resonance is therefore close to the current target frequency.

However, the present simulated S11 is:

**−2.63 dB**

which indicates that the impedance match still requires improvement.

### Current Engineering Task

The L-band geometry and/or matching structure will be optimized to improve the input match around **1.575 GHz**.

```text
Target
1.575 GHz
   │
   ▼
Current Design
1.5755 GHz
   │
   ▼
Impedance Optimization
   │
   ▼
Validated L-band Design
```

---

## 3. Design Targets

The current project uses the following RF targets:

| Parameter        |        Target |
| ---------------- | ------------: |
| UHF frequency    |   **446 MHz** |
| L-band frequency | **1.575 GHz** |
| System impedance |      **50 Ω** |
| Desired S11      |  **≤ −10 dB** |
| Desired VSWR     |     **≤ 2:1** |

These are **engineering targets**, not claims of final prototype performance.

---

## 4. Simulation vs Target

### UHF

```text
446 MHz                     522.67 MHz
TARGET ────────────────────────●
                               ↑
                         Current resonance
```

The UHF design requires a significant frequency shift toward the target.

### L-band

```text
1.575 GHz       1.5755 GHz
TARGET ─────────────●
                   ↑
             Current resonance
```

The L-band resonance is close to the target, but its impedance matching requires improvement.

---

## 5. Validation

Frequency performance will ultimately be verified using experimental RF measurements.

Planned validation:

```text
CST Simulation
      ↓
Prototype Fabrication
      ↓
VNA Calibration
      ↓
S11 Measurement
      ↓
Resonant Frequency
      ↓
Bandwidth / VSWR
      ↓
Simulation vs Measurement
```

The final frequency values will be reported only after experimental validation.

---

## Related Documentation

* [`Design Overview`](design-overview.md)
* [`Antenna Architecture`](antenna-architecture.md)
* [`Materials`](materials.md)
* [`Simulation`](../04_Simulation/)
