<div align="center">

# 🛠️ Mechanical & CAD Assembly

**Integrated PCB Chassis Architecture • Custom 3D Printed Hardware • Multi-Layer Support**

---

</div>

This directory contains the complete 3D CAD design files, mechanical assemblies, and structural layouts for the Micromouse robot chassis. The design leverages a **PCB-as-chassis** approach, paired with custom 3D-printed mounting brackets and an elevated acrylic backbone for weight optimization, low center of gravity, and modular repairability.

---

## 1. Chassis Overview (Top & Bottom Views)

<div align="center">
  <img src="previews/Top%20and%20Bottom%20Views.png" alt="Top and Bottom Views" width="600" style="border-radius: 8px;" />
</div>

### 🔍 Key Features
* 🟩 **PCB Chassis Integration:** The primary PCB serves double-duty as both the main structural frame and circuit substrate, reducing unnecessary weight and maintaining a tight footprint.
* 🖨️ **3D-Printed Mounts:** Custom brackets house the optical distance sensors and secure the drive motors firmly to the chassis.
* 🔧 **Modular Construction:** Fastener locations are designed for fast disassembly and rapid hardware iteration during testing.

---

## 2. Technical Dimensions & Sensor Alignment

<div align="center">
  <img src="previews/Measurements.png" alt="Measurements" width="600" style="border-radius: 8px;" />
</div>

### 📐 Physical Specifications & Layout

| Parameter | Specification | Notes / Purpose |
| :--- | :--- | :--- |
| **Width** | `90 mm` | Compact width for narrow maze clearance |
| **Height** | `110 mm` | Total front-to-back chassis footprint |
| **Ground Clearance** | `3 mm` | Optimized center of gravity |
| **Front Sensors (×2)** | `Forward-facing` | Detects front wall proximity |
| **Side Sensors (×2)** | `15° Offset Angle` | Angled relative to side walls for dynamic centering |

---

## 3. Structural Acrylic Backbone & Motor Assembly

<div align="center">
  <img src="previews/With%20Acralic.png" alt="With Acrylic Support" width="600" style="border-radius: 8px;" />
</div>

### 🛡️ Mechanical Layering
* 🟦 **Elevated Acrylic Plate:** Positioned **5 mm above the primary PCB**, acting as the main rigid structural spine.
* ⚙️ **Motor Mounting System:** Drive motors mount directly to the acrylic layer, ensuring strict maintenance of the **3 mm ground clearance**.
* 🔋 **Battery Housing:** The acrylic upper deck provides a stable, isolated mounting surface for the power supply.

---

## 4. Fully Populated Final Assembly

<div align="center">
  <img src="previews/WFinal_assembly.png" alt="Final Assembly View" width="600" style="border-radius: 8px;" />
  <p><i>Complete 3D CAD view showing the populated PCB, mounted sensors, 3D-printed motor clips, and upper acrylic deck.</i></p>
</div>

---

<div align="center">

| CAD Environment | Primary Material | Sensor Count |
| :---: | :---: | :---: |
| SolidWorks / Fusion 360 | FR4 (PCB) + Acrylic + PLA | 4× Distance Sensors |

</div>
