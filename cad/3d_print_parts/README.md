# 🖨️ 3D Printing Files (`.stl`)

Ready-to-print **STL** mesh files for the **Team Vortex Analog PID Robot** chassis components.

---

## 📌 Guidelines for Printing

* **Format:** Watertight `.stl` exports ready for slicing (FDM / SLA).
* **Tolerance:** Pre-sliced and clearance-checked for standard desktop 3D printer tolerances ($0.2\text{ mm}$ fit clearance).
* **Naming:** Match STL filenames directly to their source CAD parts (e.g., `chassis_base.SLDPRT` $\rightarrow$ `chassis_base.stl`).

---

## 🔒 Contributor Checklist

* Export new `.stl` files whenever modifying the main SolidWorks models in the root directory.
* Verify mesh integrity in your slicer software before pushing updates.
