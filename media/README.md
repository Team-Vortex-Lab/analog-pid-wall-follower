# 🧪 Robot Testing & Media Directory

Welcome to the testing documentation repository for the **Team Vortex Analog PID Robot**. This directory serves as a central media hub housing our oscilloscope waveform captures, hardware testbench photos, and daily physical testing video logs.

---

## 🎬 Testing Video Logs & Progress Reports

Follow our day-by-day hardware validation and circuit debugging process on YouTube:

### ⚡ Day 1: Signal Generation & Waveform Analysis
* **Focus:** Triangular Wave Generator & PWM Modulation
* **Description:** Assembled and verified the two-stage op-amp topology (Integrator + Schmitt Trigger) on the oscilloscope. Validated rail-to-rail square wave switching, peak-to-peak amplitude stability, and slope symmetry for clean carrier wave generation.
* **📺 Watch Video:** [Day 1 Testing — Triangular Waves & Basic PWMs](https://youtu.be/oQlUZ14VRn8)

---

### 🎛️ Day 2: Clustered PWM & Duty Cycle Control
* **Focus:** Multi-Channel Clustered PWM Modulation
* **Description:** Tested the precision comparator stages by combining the triangular carrier wave with analog reference signals. Verified dynamic duty cycle scaling ($0\%$ to $100\%$) across multiple synchronized output channels without signal crosstalk or noise jitter.
* **📺 Watch Video:** [Day 2 Testing — Clustered PWMs & Variable Duty Cycles](https://youtu.be/dxIQsn6eEPw)

---

### 🏎️ Day 3: Dual Sharp IR Sensor Closed-Loop Steering
* **Focus:** Real-Time Sensor Integration & Differential PWM Steering
* **Description:** Integrated two Sharp IR distance sensors with the clustered PWM stage. Measured real-time duty cycle modulation on the oscilloscope as sensor voltage output varied—confirming instantaneous differential motor speed adjustments for wall-following navigation.
* **📺 Watch Video:** [Day 3 Testing — 2-Sensor Dynamic PWM Duty Cycle Control](https://youtu.be/XEBVFFfyoN0)

---

## 📸 Testbed Gallery (`./testbench_gallery/`)

Physical test bench setups, breadboard debugging photos, and oscilloscope screen captures are organized in the **`./testbench_gallery/`** folder:

* **`./testbench_gallery/oscilloscope/`** — High-resolution captures of carrier waves, filtering stages, and PWM outputs.
* **`./testbench_gallery/hardware_bench/`** — Photographs of circuit breadboarding, sensor mounts, and PCB bench setups.

---

## 🔒 Media Guidelines

> **Note for Contributors:**
> * Keep all locally committed images (`.jpg`, `.png`, `.gif`) under **5 MB** per file to maintain repository lightness.
> * Store full-length video recordings on external streaming platforms (e.g., YouTube) and reference their direct links in this `README.md`.
