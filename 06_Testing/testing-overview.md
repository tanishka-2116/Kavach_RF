# Testing & Experimental Validation

## Purpose

The testing stage is used to compare the physical antenna prototype with the CST simulation results.

The objective is to verify the antenna's RF behaviour after fabrication and helmet integration.

---

## Test Flow

```text id="gk8r2m"
Fabricated Prototype
        ↓
Visual / Mechanical Inspection
        ↓
VNA Calibration
        ↓
S11 Measurement
        ↓
Resonant Frequency
        ↓
VSWR / Impedance
        ↓
Simulation vs Measurement
```

---

## 1. Visual Inspection

Before RF measurements, the prototype should be inspected for:

* Correct dimensions
* Layer alignment
* Feed connection
* Conductor continuity
* Mechanical attachment
* Visible fabrication defects

---

## 2. VNA Calibration

A Vector Network Analyzer (VNA) will be calibrated before measurement.

The calibration process establishes the measurement reference plane and reduces systematic measurement errors.

The exact calibration method will depend on the VNA and measurement setup used.

---

## 3. S11 Measurement

The primary RF measurement is the input reflection coefficient:

**S11**

S11 indicates how much of the incident RF signal is reflected back from the antenna input.

The measured response will be evaluated around:

* **446 MHz — UHF target**
* **1.575 GHz — L-band target**

---

## 4. Resonant Frequency

The measured resonant frequency will be identified from the S11 response.

The measured value will then be compared with the CST simulation.

```text id="xujzkl"
CST Resonance
      │
      │ Compare
      ▼
Measured Resonance
```

---

## 5. VSWR

VSWR will be used as an additional indicator of impedance matching.

The measured VSWR will be compared with the simulated antenna response.

---

## 6. Simulation vs Measurement

The final validation will compare:

| Parameter          | CST Simulation    | Physical Prototype |
| ------------------ | ----------------- | ------------------ |
| Resonant frequency | Recorded from CST | Measured using VNA |
| S11                | Recorded from CST | Measured using VNA |
| VSWR               | Simulated         | Measured           |
| Bandwidth          | Simulated         | Measured           |

This comparison will help identify differences caused by fabrication tolerances, material properties, feed implementation and helmet integration.

---

## 7. Helmet-Integrated Testing

After initial antenna characterization, testing can be performed with the antenna mounted on the intended helmet structure.

This allows the effect of the actual integration environment to be investigated.

```text id="d7f0u1"
Antenna Alone
     ↓
Measure
     ↓
Helmet Integrated
     ↓
Measure Again
     ↓
Compare
```

---

## Validation Status

**Current status:** Experimental validation is planned after prototype fabrication.

The simulation results documented in `04_Simulation` should not be treated as measured prototype results.

---

## Related Documentation

* [`Prototype Overview`](../05_Prototype/prototype-overview.md)
* [`Prototype Materials`](../05_Prototype/prototype-materials.md)
* [`UHF Simulation`](../04_Simulation/uhf-simulation.md)
* [`L-band Simulation`](../04_Simulation/l-band-simulation.md)
