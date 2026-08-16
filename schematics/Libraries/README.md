# 📚 Altium Component Libraries

This directory contains the verified schematic symbols, PCB footprints, and 3D models for all custom components used in our project.

---

### 📦 Included Files
* **`Project_Library.IntLib`** – Compiled integrated library (Recommended).
* **`Symbols.SchLib`** – Custom schematic symbols & pin definitions.
* **`Footprints.PcbLib`** – Standard PCB land patterns & component 3D bodies.

---

### 🛠️ Quick Rules
* **Use Local Libs:** Always place components from this folder to guarantee footprint alignment across all team workstations.
* **Verify Datasheets:** Double-check pad dimensions and pinouts against manufacturer datasheets before adding new parts.
* **Commit Updates:** Recompile the `.IntLib` file whenever you modify source symbols or footprints.
