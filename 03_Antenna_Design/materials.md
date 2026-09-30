# Materials & Physical Construction

## KAVACH-RF

The antenna is being developed as a **compact, helmet-integrated RF structure**. Material selection is considered from both electromagnetic and mechanical perspectives.

---

## 1. Proposed Material Stack

```text
┌────────────────────────────┐
│ Protective / Radome Layer  │
├────────────────────────────┤
│ Conductive Radiator        │
├────────────────────────────┤
│ Flexible Dielectric        │
├────────────────────────────┤
│ EBG / AMC Structure        │
├────────────────────────────┤
│ Bonding Layer              │
├────────────────────────────┤
│ Helmet Shell               │
└────────────────────────────┘
```

---

## 2. Conductive Radiator

The radiating element requires a conductive material suitable for RF operation and practical fabrication.

### Current prototype direction

**Copper**

Copper is being considered for the initial physical radiator because it provides:

* High electrical conductivity
* Easy availability
* Practical fabrication
* Suitability for prototype development

The final conductor geometry will be established through electromagnetic simulation and fabrication trials.

---

## 3. Flexible Dielectric

A flexible dielectric layer is being investigated to support conformal integration with the helmet surface.

The substrate selection will consider:

| Property              | Requirement                      |
| --------------------- | -------------------------------- |
| Flexibility           | Suitable for helmet curvature    |
| Dielectric properties | Suitable for RF design           |
| Thickness             | Compatible with antenna geometry |
| Loss                  | Low RF loss preferred            |
| Mechanical strength   | Suitable for handling            |
| Availability          | Practical for prototyping        |

The final substrate specification will be documented after material selection and characterization.

---

## 4. EBG / AMC Layer

The proposed architecture investigates an **EBG / AMC electromagnetic layer** beneath the radiator.

The layer is intended to be evaluated for its influence on:

* Electromagnetic coupling
* Radiation behaviour
* Antenna performance near the helmet/user
* Isolation from the underlying structure

Its effectiveness will be established through simulation and experimental comparison.

---

## 5. Protective Layer

A protective outer layer may be used to protect the antenna from:

* Mechanical abrasion
* Environmental exposure
* Handling damage

The protective material must not adversely affect the intended RF performance.

---

## 6. Bonding / Attachment

A suitable bonding or mounting method is required to attach the antenna structure to the helmet.

The attachment method should:

* Maintain the antenna geometry
* Follow the helmet curvature
* Provide mechanical stability
* Avoid unnecessary RF detuning
* Allow practical assembly

---

## 7. Helmet Interface

The helmet is not treated only as a mechanical mounting surface.

Its:

* Material
* Curvature
* Thickness
* Distance from the radiator

can influence the electromagnetic behaviour of the antenna.

Therefore, the integrated helmet structure should be included in the simulation where appropriate.

---

## 8. Material Selection Status

| Component        | Current Direction                 | Status               |
| ---------------- | --------------------------------- | -------------------- |
| Radiator         | Copper                            | Prototype direction  |
| Dielectric       | Flexible substrate                | Under selection      |
| EBG / AMC        | Electromagnetic surface           | Under development    |
| Protective layer | RF-compatible protective material | To be finalized      |
| Bonding          | Helmet-compatible attachment      | To be finalized      |
| Helmet           | Tactical helmet shell             | Integration platform |

---

## 9. Material Selection Workflow

```text
Material Candidates
        ↓
Electrical Properties
        ↓
Mechanical Properties
        ↓
CST Material Model
        ↓
Simulation
        ↓
Prototype Fabrication
        ↓
RF Measurement
        ↓
Final Selection
```

---

## Important Note

Material names and specifications in this document represent the **current development direction**.

Final material selection will be based on the actual antenna design, electromagnetic simulation, fabrication requirements and experimental RF measurements.

---

## Related Documentation

* [`Design Overview`](design-overview.md)
* [`Antenna Architecture`](antenna-architecture.md)
* [`Frequency Plan`](frequency-plan.md)
* [`Simulation`](../04_Simulation/)
* [`Prototype`](../05_Prototype/)
