<div align="center">

# ⚡ PCB Layout, Copper Pours & Hardware Assembly Documentation

**Precision Trace Routing • Low-Impedance Ground Plane • Dual-Rail Power Pours • Hardware Verification**

![Layer Count](https://img.shields.io/badge/Layers-2--Layer%20PCB-0078D4?style=for-the-badge)
![Copper Weight](https://img.shields.io/badge/Copper-1%20oz%20Cu-D97706?style=for-the-badge)
![Signal Trace](https://img.shields.io/badge/Signal%20Width-0.254%20mm-10B981?style=for-the-badge)
![Power Rails](https://img.shields.io/badge/Power%20Rails-%2B5V%20%2F%20--5V-8B5CF6?style=for-the-badge)

---

</div>

This repository contains the PCB layout assets, copper pour configurations, and physical hardware assembly documentation for the controller board. The board architecture emphasizes controlled trace widths, signal return stability, low-impedance dual-rail power delivery, and clean physical assembly.

---

## 1. Trace Routing & Current-Capacity Design

<table>
  <tr>
    <td width="44%" align="center">
      <img src="Images_preview/routings.png" alt="PCB Trace Routing" width="100%" style="border-radius: 8px;" />
    </td>
    <td width="56%" valign="top">
      <h3>🛣️ Routing Strategy</h3>
      <ul>
        <li>🎯 <b>0.254 mm Signal Traces:</b> Standard <b>0.254 mm (10 mil)</b> trace widths are utilized across all low-current signal lines, delivering an optimal balance between routing density, manufacturing reliability, and clean signal propagation.</li>
        <li>⚡ <b>High-Capacity Power Traces:</b> Dedicated power-carrying tracks are routed with significantly wider trace geometries tailored to their specific current demands.</li>
        <li>🛡️ <b>Thermal & Current Safety Margin:</b> All power trace widths are sized well above their theoretical maximum current limits—incorporating a deliberate safety headroom to prevent resistive voltage drops, localized heating, and thermal stress under peak load.</li>
      </ul>
    </td>
  </tr>
</table>

---

## 2. Top Layer Ground Pour (Top Copper)

<table>
  <tr>
    <td width="56%" valign="top">
      <h3>🟩 Ground Plane Architecture</h3>
      <ul>
        <li>🔄 <b>Continuous GND Return Path:</b> The top copper layer is flooded with a unified Ground (<code>GND</code>) plane, providing the shortest, lowest-impedance return path for high-speed and sensitive analog signals.</li>
        <li>📉 <b>Signal Tail & Reference Stabilization:</b> By establishing an uninterrupted ground reference beneath and around signal traces, signal ringing, overshoot, and trailing transients are effectively dampened.</li>
        <li>⚖️ <b>Balanced Charge Distribution:</b> The continuous copper pour promotes uniform electrostatic charge distribution across the entire PCB surface, minimizing ground bounce and electromagnetic interference (EMI).</li>
      </ul>
    </td>
    <td width="44%" align="center">
      <img src="Images_preview/top_pour.png" alt="Top Layer GND Copper Pour" width="100%" style="border-radius: 8px;" />
    </td>
  </tr>
</table>

---

## 3. Bottom Layer Dual-Rail Power Pours (Bottom Copper)

<table>
  <tr>
    <td width="44%" align="center">
      <img src="Images_preview/bottom_pour.png" alt="Bottom Layer +5V and -5V Power Pours" width="100%" style="border-radius: 8px;" />
    </td>
    <td width="56%" valign="top">
      <h3>🔋 Split Power Plane Distribution</h3>
      <p>Rather than relying on narrow, routed power tracks—which introduce parasitic inductance and resistance—the bottom copper layer is partitioned into dedicated <b>+5V</b> and <b>-5V</b> copper pours to deliver smooth, low-noise power directly to the operational amplifiers (<code>Op-Amps</code>) and active analog stages.</p>
      <table>
        <thead>
          <tr>
            <th align="left">Power Rail</th>
            <th align="left">Copper Zone</th>
            <th align="left">Primary Function & Design Advantage</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><b>+5V Pour</b></td>
            <td>Positive Supply Zone</td>
            <td>Delivers smooth, low-impedance positive bias power to Op-Amps, logic, and sensor interfaces</td>
          </tr>
          <tr>
            <td><b>-5V Pour</b></td>
            <td>Negative Supply Zone</td>
            <td>Provides an isolated, ripple-free negative supply plane for symmetric dual-rail Op-Amp operation</td>
          </tr>
        </tbody>
      </table>
    </td>
  </tr>
</table>

---

## 4. Bare PCB Inspection (Pre-Assembly)

<table>
  <tr>
    <td width="56%" valign="top">
      <h3>🔍 Fabricated Board Verification</h3>
      <ul>
        <li>✨ <b>Bare Board Quality:</b> View of the freshly fabricated, unpopulated PCB prior to component placement and soldering.</li>
        <li>🧩 <b>Pad & Soldermask Integrity:</b> Confirms clean copper pad finishes, accurate silkscreen component designators, crisp soldermask clearances, and verified continuity across the top and bottom copper pours before assembly.</li>
      </ul>
    </td>
    <td width="44%" align="center">
      <img src="Images_preview/before_soldering.jpeg" alt="Original Unpopulated PCB Before Soldering" width="100%" style="border-radius: 8px;" />
    </td>
  </tr>
</table>

---

## 5. Assembled Hardware (Post-Soldering)

<table>
  <tr>
    <td width="44%" align="center">
      <img src="Images_preview/after_soldering.jpeg" alt="Fully Assembled PCB After Soldering" width="100%" style="border-radius: 8px;" />
    </td>
    <td width="56%" valign="top">
      <h3>🛠️ Completed Board Assembly</h3>
      <ul>
        <li>🔧 <b>Component Population:</b> Fully populated controller board with all surface-mount and through-hole components soldered in place.</li>
        <li>✅ <b>Joint & Thermal Inspection:</b> Verified clean solder fillets, proper component orientation, and reliable mechanical/electrical connections across power rails, Op-Amp stages, and I/O headers.</li>
      </ul>
    </td>
  </tr>
</table>

---

<div align="center">

### 📋 PCB Design Specifications Summary

| Parameter | Specification | Design Purpose |
| :---: | :---: | :---: |
| **Board Stackup** | 2-Layer FR4 (1 oz Cu) | Cost-effective, robust double-sided layout |
| **Signal Trace Width** | 0.254 mm (10 mil) | Reliable high-density signal routing |
| **Power Trace Sizing** | Over-spec'd with safety margin | Prevents thermal rise & voltage drop under load |
| **Top Layer Copper** | Full `GND` Pour | Signal stabilization, EMI shielding & uniform charge flow |
| **Bottom Layer Copper** | Split `+5V` / `-5V` Pours | Low-impedance, smooth dual-rail power for Op-Amps |

</div>
