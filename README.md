# KAVACH-RF

### Helmet-Mounted Conformal Antenna for Tactical Communications

**Smart India Hackathon 2026 — SIH26185**

> **“Shielding the soldier, connecting the squad.”**

---

## 📡 Project

**KAVACH-RF** is a research and engineering project focused on developing a **helmet-mounted conformal antenna platform** for tactical communication requirements in urban CQB environments.

The concept integrates a **low-profile conformal antenna architecture** with a tactical helmet while investigating controlled radiation, compact integration and dual-band operation.

### Target platform

* **UHF** — tactical radio communication
* **L-band** — video / camera communication
* Flexible, helmet-integrated antenna structure
* Electromagnetic simulation followed by physical validation

---

## 🎯 Problem

Conventional external antennas can introduce:

* Antenna snagging and protrusion
* Poor antenna positioning
* Signal blockage caused by surrounding structures
* Human-body interaction and detuning
* Separate antenna requirements for different communication links

KAVACH-RF investigates a **helmet-integrated alternative**.

---

## 💡 Proposed Architecture

```text
                  TACTICAL HELMET
                        │
        ┌───────────────┴───────────────┐
        │                               │
     UHF ANTENNA                   L-BAND ANTENNA
     Tactical Radio               Video / Camera
        │                               │
        └───────────────┬───────────────┘
                        │
                  RF INTERFACE
                        │
                 COMMUNICATION
                    SYSTEM
```

The proposed physical stack consists of:

```text
Protective / Radome Layer
          ↓
Conformal Antenna Layer
          ↓
EBG / AMC Layer
          ↓
Flexible Dielectric
          ↓
Helmet Shell
```

---

## 🔬 Development Workflow

```text
DESIGN
   ↓
SIMULATION
   ↓
ANTENNA & FEED DESIGN
   ↓
FABRICATION
   ↓
HELMET INTEGRATION
   ↓
RF VALIDATION
   ↓
OPTIMIZATION
```

---

## 📊 Current Simulation Status

The current CST simulation provides the following starting point:

| Band   |    Target |  Simulated |       S11 | Status                         |
| ------ | --------: | ---------: | --------: | ------------------------------ |
| UHF    |   446 MHz | 522.67 MHz | −10.38 dB | Frequency retuning required    |
| L-band | 1.575 GHz | 1.5755 GHz |  −2.63 dB | Matching optimization required |

These are **simulation results**, not final experimental measurements.

### Current next steps

* Retune UHF toward the 446 MHz target
* Improve L-band impedance matching
* Fabricate the antenna on the selected flexible substrate
* Measure the prototype using a VNA
* Compare simulation against experimental results

---

## 🧩 Repository

| Section                                   | Contents                                            |
| ----------------------------------------- | --------------------------------------------------- |
| [01 — Problem](01_Problem/)               | Problem statement and requirements                  |
| [02 — Solution](02_Solution/)             | Proposed solution and system architecture           |
| [03 — Antenna Design](03_Antenna_Design/) | Frequency, geometry, materials and dimensions       |
| [04 — Simulation](04_Simulation/)         | CST models and simulation results                   |
| [05 — Prototype](05_Prototype/)           | Fabrication, assembly and BOM                       |
| [06 — Testing](06_Testing/)               | VNA and experimental validation                     |
| [07 — Feasibility](07_Feasibility/)       | Technical, manufacturing and deployment feasibility |
| [08 — Research](08_Research/)             | Literature and technical references                 |
| [09 — Documentation](09_Documentation/)   | Pitch and project documentation                     |

---

## 🛠️ Technology Stack

### Simulation

* CST Studio Suite
* Ansys HFSS — planned / comparative analysis

### Mechanical Design

* SolidWorks
* Helmet surface / curvature mapping

### RF Hardware

* Flexible substrate
* Conductive radiator
* RF feed
* SMA / U.FL interface
* VNA for characterization

---

## 📈 Project Status

**Current stage: Simulation → Optimization → Prototype**

* ✅ Problem analysis
* ✅ Solution architecture
* ✅ Initial dual-band concept
* ✅ Initial CST simulation
* 🔄 UHF frequency optimization
* 🔄 L-band impedance optimization
* ⬜ Prototype fabrication
* ⬜ VNA validation
* ⬜ Radiation-pattern measurement
* ⬜ Final optimization

---

## 📚 Documentation

For the complete technical development, navigate through the folders above.

The repository is maintained as a **living engineering record**:

**Research → Design → Simulation → Fabrication → Measurement → Optimization**

---

## 👥 Team

### KAVACH-RF

**SIH Problem Statement:** SIH26185
**Category:** Hardware
**Theme:** Robotics and Drones
**Team ID:** AF-HW-03

---

<p align="center">

**KAVACH-RF**

*Shielding the soldier, connecting the squad.*

</p>
