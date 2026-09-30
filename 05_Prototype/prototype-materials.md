# Prototype Materials & BOM

## Purpose

This document records the materials and components required to convert the optimized antenna design into a physical prototype.

The final quantities and specifications will be updated as the design is finalized.

---

## Prototype Material Categories

| Category                    | Purpose                             | Status                           |
| --------------------------- | ----------------------------------- | -------------------------------- |
| Conductive sheet / copper   | RF radiator                         | Selected for prototype direction |
| Dielectric substrate        | Supports RF structure               | Under final selection            |
| EBG / AMC structure         | Electromagnetic surface             | Under development                |
| RF connector                | Measurement interface               | Required                         |
| RF cable                    | Connection to measurement equipment | Required                         |
| Adhesive / bonding material | Mechanical attachment               | To be finalized                  |
| Helmet shell                | Integration platform                | Required                         |
| Protective layer            | Physical protection                 | To be finalized                  |

---

## RF Components

### RF Connector

A suitable RF connector will provide the interface between the antenna feed and measurement equipment.

The connector and feed structure should maintain the intended **50 Ω RF interface**.

### RF Cable

A suitable 50 Ω RF cable will be used to connect the prototype to the VNA during characterization.

---

## Mechanical Materials

The mechanical assembly requires materials capable of maintaining the antenna geometry while following the helmet curvature.

Selection will consider:

* Flexibility
* Thickness
* Adhesion
* Mechanical stability
* RF compatibility
* Availability

---

## Fabrication Requirements

Before fabrication, the following parameters must be finalized from the optimized CST model:

* Radiator dimensions
* Substrate dimensions
* Substrate thickness
* EBG / AMC geometry
* Feed location
* Feed dimensions
* Layer thicknesses
* Mounting location

---

## Prototype BOM

| No. | Item                        | Purpose                             |    Quantity | Status              |
| --: | --------------------------- | ----------------------------------- | ----------: | ------------------- |
|   1 | Copper / conductive sheet   | Radiating element                   |           1 | Prototype direction |
|   2 | Dielectric substrate        | Antenna support                     |           1 | To be finalized     |
|   3 | RF connector                | RF interface                        |           1 | Required            |
|   4 | 50 Ω RF cable               | VNA connection                      |           1 | Required            |
|   5 | Adhesive / bonding material | Mechanical attachment               | As required | To be finalized     |
|   6 | Helmet shell                | Antenna integration                 |           1 | Required            |
|   7 | Protective layer            | Environmental/mechanical protection |           1 | To be finalized     |

---

## Procurement Principle

Prototype materials should be selected based on:

1. RF suitability
2. Mechanical compatibility
3. Availability
4. Fabrication practicality
5. Cost

Final specifications will be recorded once the optimized antenna geometry and material stack are frozen.

---

## Related Documentation

* [`Prototype Overview`](prototype-overview.md)
* [`Antenna Materials`](../03_Antenna_Design/materials.md)
* [`Simulation`](../04_Simulation/)
* [`Testing`](../06_Testing/)
