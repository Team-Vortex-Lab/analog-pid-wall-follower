# ⚡ Circuit Schematics & PCB Layouts

Welcome to the hardware design repository for the **Team Vortex Analog PID Robot**. This directory houses the complete schematic design, printed circuit board (PCB) layout, and manufacturing outputs for our real-time, hardware-based analog PID control system.

---

## 🛠️ EDA Toolchain & Design Files

This project is built and maintained in **Altium Designer**. The project hierarchy is structured as follows:

| Design File / Directory | Description |
| :--- | :--- |
| **`*.PrjPcb`** | Master Altium project container file. |
| **`*.SchDoc`** | Hierarchical schematics covering sensor signal conditioning, active Op-Amp PID control loops, and H-bridge motor driver stages. |
| **`*.PcbDoc`** | Multi-layer PCB layout featuring targeted ground planes, optimized power traces, and low-noise analog routing. |
| **`Libraries/`** | Project-specific schematic symbols (`*.SchLib`) and PCB footprints (`*.PcbLib`). |
| **`Outputs/`** | Production-ready Gerber files, NC Drill data, BOM, and CPL files configured for **JLCPCB SMT Assembly**. |

---

## 📋 Hardware Architecture Overview

* **Sensor Signal Conditioning:** Filtering and scaling stage for continuous analog proximity sensing.
* **Analog PID Controller:** Fully active operational amplifier circuit implementing parallel Proportional, Integral, and Derivative gain stages.
* **Actuator Driver:** Dual H-bridge power stage for motor speed and direction control.

---

## 🔒 Repository Hygiene

> **Note for Contributors:** Cache directories (`History/`, `__History/`), build logs (`*.CompileLog`), and workspace options are explicitly ignored via `.gitignore`. Please ensure all edits are saved to the primary project file (`*.PrjPcb`) before committing.
