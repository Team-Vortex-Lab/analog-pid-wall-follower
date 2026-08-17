# 📐 3D Mechanical CAD & Chassis Assembly

Welcome to the mechanical design repository for the **Team Vortex Analog PID Robot**. This directory contains all source CAD models, printable export files, neutral exchange formats, and visual renders for the robot's physical structure and custom chassis.

---

## 🛠️ CAD Toolchain & Folder Structure

All primary mechanical components are modeled in **SolidWorks**. Files in this directory are organized as follows:

| Path / File Type | Description |
| :--- | :--- |
| **`./` (Root)** | Native SolidWorks Part (`.SLDPRT`) and Assembly (`.SLDASM`) source files. |
| **`./3d_print_parts/`** | 3D-printable **STL** (`.stl`) mesh files optimized for rapid prototyping via FDM/SLA additive manufacturing. |
| **`./step/`** | Universal **STEP** (`.step` / `.stp`) format files for cross-CAD compatibility and CAM toolpaths. |
| **`./previews/`** | High-resolution image renders (`.png` / `.jpg`) for quick visual review of parts without opening CAD software. |

---

## 🎯 Design Features & Specifications

* **Custom Chassis Frame:** Optimized mounting interfaces for sensor arrays, motor drivers, and PCB hardware.
* **Prototyping Ready:** Pre-configured STL files tuned for standard 3D printing tolerances located in `./3d_print_parts/`.
* **Neutral Formats:** Standardized STEP models provided for easy integration into secondary CAD environments.

---

## 👷 Message for 3D Designers & Contributors

Please review the primary design assets and reference materials before starting assembly or modeling:

### 📌 Reference Materials & Links
* **Reference Model Diagram:** [View CAD Reference Model](https://drive.google.com/file/d/1-P2Z6PWNmvsWfch-ZRc7PMqoGPqI8Aun/view?usp=sharing)
* **Component Measurement Specifications:** [View Component Measurements](https://drive.google.com/file/d/1M3fZRFy8i3cnOhA6xqmA4AMep1WubyNB/view?usp=sharing)

### 📐 Mechanical & Modeling Guidelines
1. **PCB Shape Flexibility:** The PCB outline shown in the reference design diagram is **strictly a reference layout**. You have full freedom to modify or redesign the PCB shape as needed to optimize the overall chassis geometry.
2. **PCB Board Sheet Thickness:** Please model the PCB using a standard **1.6 mm sheet thickness** in your 3D assembly to ensure accurate vertical stack-up and component clearance checks.
3. **Required Exports:** Whenever you finish or update a model, always export and update the corresponding files in **`./3d_print_parts/`** (`.stl`), **`./step/`** (`.step`), and **`./previews/`** (`.png`/`.jpg`).
4. **Units & Tolerances:** Ensure all models are designed in **millimeters (mm)** with a minimum printing tolerance of **0.2 mm – 0.4 mm** for mating surfaces, mounts, and screw holes.

---

## 🔒 Repository Hygiene

> **Note:** Native SolidWorks temporary lock files (`~$*`), crash logs, and local backup files are automatically filtered out via `.gitignore`. Please verify all STEP and STL files are updated in their respective subfolders before pushing your branch.
