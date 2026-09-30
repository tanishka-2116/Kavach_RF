# Antenna Architecture

## Layered Conformal Structure

The proposed antenna uses a layered structure designed to follow the helmet curvature.

![Layer Exploded View](../assets/concept/layer-exploded-view.jpg)

---

## Layer Stack

### 1. Protective Outer Layer

Provides physical protection to the antenna structure.

The layer is intended to protect the conductive elements from environmental exposure and mechanical abrasion.

---

### 2. Conformal Antenna Layer

Contains the RF radiating structure.

The conductor geometry is designed to follow the helmet surface.

The current concept investigates a microstrip / patch-based structure.

---

### 3. Dielectric Substrate

The dielectric provides mechanical support and establishes the electromagnetic environment required by the radiator.

The final substrate selection will depend on:

* Relative permittivity
* Loss tangent
* Thickness
* Flexibility
* Mechanical compatibility
* Availability

---

### 4. EBG / AMC Layer

The design investigates an electromagnetic band-gap / artificial magnetic conductor structure beneath the radiator.

Its electromagnetic effect will be evaluated through simulation and measurement.

---

### 5. Bonding Layer

Provides mechanical attachment between the antenna structure and helmet surface.

Its thickness and dielectric properties can influence RF performance and therefore should be considered in the electromagnetic model.

---

### 6. Helmet Shell

The helmet acts as the mechanical integration platform.

Its material and geometry can affect the antenna's electromagnetic behavior and therefore should be included in the integrated simulation where appropriate.

---

## Physical Arrangement

```text
              OUTSIDE
                 ↓
        ┌─────────────────┐
        │ Protective Layer│
        ├─────────────────┤
        │    Radiator     │
        ├─────────────────┤
        │    Substrate    │
        ├─────────────────┤
        │    EBG / AMC    │
        ├─────────────────┤
        │ Bonding Layer   │
        ├─────────────────┤
        │  Helmet Shell   │
        └─────────────────┘
                 ↓
               USER
```

---

## Design Principle

The antenna is treated as an **integrated RF structure**, rather than simply attaching a conventional antenna to the helmet.

This means the following must be considered together:

* Antenna geometry
* Helmet curvature
* Material stack
* Feed location
* Human-body proximity
* Electromagnetic coupling
* Mechanical integration

---

## Current Status

The architecture shown here represents the **proposed design direction**.

The final layer dimensions, substrate selection, radiator geometry, EBG/AMC geometry and mounting method remain subject to simulation optimization and prototype validation.
