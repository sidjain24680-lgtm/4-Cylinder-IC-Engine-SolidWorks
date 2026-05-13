# 🔧 4-Cylinder IC Engine — SolidWorks CAD Assembly

![Assembly Render](images/assembly_render.png)

> A fully parametric 3D CAD model of a 4-cylinder internal combustion engine bottom-end assembly, designed from scratch in SolidWorks. Includes 6 individual part files and a complete assembly.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Parts Modeled](#parts-modeled)
- [Assembly Preview](#assembly-preview)
- [Tools & Software](#tools--software)
- [File Structure](#file-structure)
- [Design Highlights](#design-highlights)
- [How to Open](#how-to-open)
- [Future Work](#future-work)
- [Author](#author)

---

## Overview

This project is a detailed SolidWorks CAD model of the bottom-end assembly of a **4-cylinder, 4-stroke inline IC engine**. Each component was modeled individually as a separate part file and then assembled together to replicate the real-world mechanism of a crank-slider system.

The project focuses on:
- Accurate geometry and proportions of each engine component
- Proper use of SolidWorks features (Boss-Extrude, Shell, Revolve, Fillet, Mirror, Pattern, etc.)
- Assembly constraints that reflect real mechanical relationships

---

## Parts Modeled

| # | Part Name | File | Key Features Used |
|---|-----------|------|-------------------|
| 1 | **Piston** | `Piston.SLDPRT` | Boss-Extrude, Shell, Cut-Extrude, Linear Pattern, Dome, Fillet |
| 2 | **Piston Ring** | `Piston Ring.SLDPRT` | Boss-Extrude (circular profile) |
| 3 | **Piston Pin** | `Piston Pin.SLDPRT` | Boss-Extrude, Chamfer, Body-Move/Copy |
| 4 | **Connecting Rod** | `Connecting rod.SLDPRT` | Boss-Extrude ×3, Cut-Extrude ×2, Fillet ×3 |
| 5 | **Connecting Rod Cap** | `connecting cover.SLDPRT` | Boss-Extrude ×2, Cut-Extrude ×3, Fillet ×2 |
| 6 | **Crankshaft** | `Cranck shaft.SLDPRT` | Boss-Extrude ×9, Mirror ×4, Plane references, Combine, Fillet |

---

## Assembly Preview

### Full Assembly
![Full Assembly](images/assembly_render.png)

### Individual Parts

| Piston | Piston Ring | Piston Pin |
|--------|-------------|------------|
| ![Piston](images/piston.png) | ![Piston Ring](images/piston_ring.png) | ![Piston Pin](images/piston_pin.png) |

| Connecting Rod | Connecting Rod Cap | Crankshaft |
|----------------|--------------------|------------|
| ![Con Rod](images/connecting_rod.png) | ![Con Rod Cap](images/connecting_rod_cap.png) | ![Crankshaft](images/crankshaft.png) |

---

## Tools & Software

- **CAD Software:** SolidWorks Premium 2022 SP1.0
- **Units:** MMGS (Millimeter, Gram, Second)
- **File Formats:** `.SLDPRT` (parts), `.SLDASM` (assembly)
- **Exported Formats:** `.STEP`, `.IGES` *(if applicable)*

---

## File Structure

```
4-Cylinder-IC-Engine-CAD/
│
├── Parts/
│   ├── Piston.SLDPRT
│   ├── Piston Ring.SLDPRT
│   ├── Piston Pin.SLDPRT
│   ├── Connecting rod.SLDPRT
│   ├── connecting cover.SLDPRT
│   └── Cranck shaft.SLDPRT
│
├── Assembly/
│   └── IC_Engine_Assembly.SLDASM
│
├── Images/
│   ├── assembly_render.png
│   ├── piston.png
│   ├── piston_ring.png
│   ├── piston_pin.png
│   ├── connecting_rod.png
│   ├── connecting_rod_cap.png
│   └── crankshaft.png
│
└── README.md
```

---

## Design Highlights

- **Crankshaft** is the most complex part — built using multiple reference planes, mirroring operations, and a Combine feature to achieve the multi-throw geometry of a 4-cylinder crank.
- **Piston** uses a Shell feature to hollow the body, with ring grooves modeled using Linear Pattern and a Dome for crown geometry.
- **Connecting Rod** features I-beam cross-section geometry for realistic mass-reduction, with proper big-end and small-end bores.
- **Assembly** uses standard SolidWorks mates (Concentric, Coincident) to constrain all 4 piston-rod-crank subassemblies.

---

## How to Open

1. Clone or download this repository
2. Open SolidWorks 2022 or later
3. Open `Assembly/IC_Engine_Assembly.SLDASM`
4. SolidWorks will automatically resolve all part references from the `Parts/` folder

> ⚠️ If you're using a different version of SolidWorks, some features may need to be rebuilt. STEP files are provided for cross-version compatibility.

---

## Future Work

- [ ] Add cylinder block and head to complete the full engine model
- [ ] Perform Motion Study / kinematic simulation of the crank-slider mechanism
- [ ] Add FEA (Finite Element Analysis) on the connecting rod and crankshaft under load
- [ ] Apply realistic materials and render using SolidWorks Visualize

---

## Author

**Siddharth Jain**
Mechanical Engineering Student | CAD & Simulation and Manufacturing Enthusiast

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/your-profile)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat&logo=github)](https://github.com/your-username)

---

*If you found this useful, feel free to ⭐ star this repo!*
