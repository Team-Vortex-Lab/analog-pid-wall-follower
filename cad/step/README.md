# 🔄 STEP Neutral Exchange Files (`.step` / `.stp`)

Universal CAD exchange files for cross-platform compatibility and manufacturing workflows.

---

## 📌 Purpose & Guidelines

* **Version Independence:** Provides a reliable fallback to bypass SolidWorks version compatibility issues across different CAD software setups.
* **Manufacturing Ready:** Neutral format required for CAM toolpaths, CNC machining, or third-party CAD modeling software.
* **Optional Reference:** Used primarily for external collaboration and cross-CAD integration.

---

## 🔒 Contributor Checklist

* Export updated `.step` or `.stp` files whenever finalizing major revisions to native SolidWorks files (`.SLDPRT` / `.SLDASM`).
* Keep filenames identical to their parent SolidWorks models (e.g., `chassis_base.SLDPRT` $\rightarrow$ `chassis_base.step`).
