# ⚡ Circuit Simulations (`.asc`)

This directory houses the LTspice schematic files and circuit models for the **Team Vortex Analog PID Robot** power, signal processing, and control hardware.

---

## 📌 Directory Contents & Scope

* **Sensor Signal Conditioning:** Amplification, active filtering, and noise suppression circuits for raw IR distance sensor signals.
* **Analog PID Controller:** Op-Amp-based Proportional, Integral, and Derivative analog processing stages for real-time error corrections.
* **Motor Driver Interfaces:** H-bridge control stages, PWM generation, and power stage decoupling configurations.

---

## ⚙️ Simulation Guidelines

* **Software:** Built and validated using **LTspice**.
* **Primary Source Files:** Track only native schematic files (`.asc`) and custom symbol/component libraries (`.asy`, `.lib`, `.sub`).
* **Repository Hygiene:** Log files (`.log`), raw waveform outputs (`.raw`), and netlists (`.net`) are excluded via `.gitignore` to prevent repository bloat.

---

## 🔒 Contributor Checklist

1. Verify that schematics run clean simulations locally without unhandled transient errors before pushing updates.
2. Label key node nets clearly (e.g., `V_ERR`, `PWM_OUT`, `PID_SUM`) to simplify peer review on schematic updates.
3. Bundle any custom third-party Op-Amp or MOSFET SPICE models in the folder alongside their corresponding `.asc` file.
