# 📐 3D Mechanical CAD & Chassis Assembly

Welcome to the mechanical design repository for the **Team Vortex Analog PID Robot**. This directory contains all source CAD models, printable export files, neutral exchange formats, and visual renders for the robot's physical structure and custom chassis.

---

## 🛠️ CAD Toolchain & Folder Structure

All primary mechanical components are modeled in **SolidWorks**. Files in this directory are organized as follows:

| Path / File Type | Description |
| :--- | :--- |
| **`./` (Root)** | Native SolidWorks Part (`.SLDPRT`) and Assembly (`.SLDASM`) source files. |
| **`./step/`** | Universal **STEP** (`.step` / `.stp`) format files for cross-CAD compatibility and CAM toolpaths. |
| **`./previews/`** | High-resolution image renders (`.png` / `.jpg`) for quick visual review of parts without opening CAD software. |
| **`*.stl`** | 3D-printable mesh files optimized for rapid prototyping via FDM/SLA additive manufacturing. |

---

## 🎯 Design Features & Specifications

* **Custom Chassis Frame:** Optimized mounting interfaces for sensor arrays, motor drivers, and PCB hardware.
* **Prototyping Ready:** Pre-configured STL files tuned for standard 3D printing tolerances.
* **Neutral Formats:** Standardized STEP models provided for easy integration into secondary CAD environments.

---

## 🔒 Repository Hygiene

> **Note for Contributors:** Native SolidWorks temporary lock files (`~$*`), crash logs, and local backup files are automatically filtered out via `.gitignore`. Please ensure all updated parts are exported to both `./step/` and `./previews/` before pushing commits.
