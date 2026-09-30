# System Architecture

## KAVACH-RF

The KAVACH-RF architecture connects the helmet-mounted antenna platform with the communication system through an RF interface.

---

## High-Level Architecture

```text
                    TACTICAL HELMET
                           │
          ┌────────────────┴────────────────┐
          │                                 │
          ▼                                 ▼
    ┌─────────────┐                   ┌─────────────┐
    │ UHF ANTENNA │                   │ L-BAND      │
    │  446 MHz    │                   │  1.575 GHz  │
    └──────┬──────┘                   └──────┬──────┘
           │                                 │
           └──────────────┬──────────────────┘
                          ▼
                   RF FEED / MATCHING
                          │
                          ▼
                 COMMUNICATION SYSTEM
                          │
                 ┌────────┴────────┐
                 ▼                 ▼
             RADIO LINK        VIDEO/DATA
```

---

## Functional Blocks

### 1. Helmet

Provides the mechanical platform for integrating the conformal antenna.

The antenna is designed around the available helmet surface rather than being treated as an independent external component.

---

### 2. UHF Antenna

**Target:** 446 MHz

The UHF section is intended for investigation as the tactical radio communication link.

The current CST model resonates at **522.67 MHz**, so frequency retuning remains part of the design process.

---

### 3. L-band Antenna

**Target:** 1.575 GHz

The L-band section is being investigated for the video/camera communication link.

The current CST model resonates at **1.5755 GHz**, while the simulated S11 of **−2.63 dB** indicates that further impedance matching is required.

---

### 4. RF Feed / Matching Network

The RF feed transfers energy between the antenna and the communication system.

The matching network will be optimized to achieve the required impedance response.

Target system impedance:

**50 Ω**

---

### 5. Communication System

The antenna interfaces with the appropriate communication hardware through the RF interface.

The antenna itself is an RF subsystem and does not replace the communication radio or data-processing hardware.

---

## Physical Layer Architecture

```text
                 OUTER SIDE
                     │
                     ▼
        ┌────────────────────────┐
        │ Protective / Radome    │
        ├────────────────────────┤
        │ Conformal Radiator     │
        ├────────────────────────┤
        │ EBG / AMC Structure    │
        ├────────────────────────┤
        │ Flexible Dielectric    │
        ├────────────────────────┤
        │ Helmet Shell           │
        └────────────────────────┘
                     │
                     ▼
                 HEAD SIDE
```

---

## Design Considerations

The architecture is evaluated considering:

* Helmet curvature
* Available mounting area
* Antenna-to-helmet interaction
* Human-body proximity
* RF feed routing
* Mechanical attachment
* Impedance matching
* Radiation characteristics

---

## Validation Path

```text
Architecture
     ↓
CST Model
     ↓
Simulation
     ↓
Prototype
     ↓
Helmet Integration
     ↓
VNA Measurement
     ↓
Simulation vs Measurement
```

---

## Related Documentation

* [`Solution Overview`](solution-overview.md)
* [`Working Principle`](working-principle.md)
* [`Antenna Design`](../03_Antenna_Design/)
