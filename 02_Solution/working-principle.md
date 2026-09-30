# Working Principle

## How KAVACH-RF Works

KAVACH-RF works by integrating a conformal RF antenna structure onto the helmet surface and connecting it to the communication system through an RF feed.

---

## Signal Flow

```text
Communication System
        │
        ▼
   RF Feed / Match
        │
        ▼
 Conformal Antenna
        │
        ▼
 Electromagnetic Radiation
        │
        ▼
     RF Link
```

For reception, the process occurs in the reverse direction:

```text
Incoming RF Signal
        │
        ▼
 Conformal Antenna
        │
        ▼
   RF Feed / Match
        │
        ▼
Communication System
```

---

## Dual-Band Concept

The project investigates two operating regions:

```text
                 KAVACH-RF
                     │
          ┌──────────┴──────────┐
          │                     │
         UHF                   L-band
       446 MHz                1.575 GHz
          │                     │
     Tactical Radio        Video / Camera
```

Each frequency region requires appropriate antenna geometry and impedance matching.

---

## Role of Conformal Integration

Instead of mounting a conventional antenna as a large external structure, the proposed approach places the radiating structure along the helmet geometry.

This provides a design platform for investigating:

* Compact installation
* Reduced protrusion
* Helmet-compatible geometry
* RF behavior near the helmet and user
* Radiation characteristics in the integrated configuration

---

## Role of EBG / AMC

The proposed architecture investigates an **EBG / AMC layer** beneath the antenna.

Its purpose within the design is to investigate electromagnetic interaction between the radiator and the helmet/user environment and to help control the antenna's electromagnetic behavior.

The actual benefit will be established through simulation and measurement rather than assumed.

---

## Optimization Loop

The antenna is developed iteratively:

```text
Initial Geometry
       ↓
CST Simulation
       ↓
Check Resonance
       ↓
Check S11 / VSWR
       ↓
Modify Geometry
       ↓
Re-simulate
       ↓
Prototype
       ↓
VNA Measurement
       ↓
Compare Results
       ↓
Final Optimization
```

---

## Current Development Status

The initial simulation demonstrates that the proposed architecture can produce resonances in the investigated UHF and L-band regions.

However, the current model still requires optimization:

* UHF → resonance needs to move toward **446 MHz**
* L-band → impedance matching needs improvement toward the desired S11 target

The next stage is therefore **antenna optimization followed by physical validation**.

---

## Related Documentation

* [`Solution Overview`](solution-overview.md)
* [`System Architecture`](system-architecture.md)
* [`Simulation`](../04_Simulation/)
* [`Testing`](../06_Testing/)
