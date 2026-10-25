<div align="center">

# Engineered Window Rollers
### *FEM-verified replacement rollers for aluminium-profile sliding windows*

<img src="https://RolandThsive.github.io/FeaturedImages/8203012936776499720.jpg" alt="Engineered Window Rollers" width="720"/>

[![Blog](https://img.shields.io/badge/Build%20Guide-ro--h--bots-FF5722?style=for-the-badge&logo=blogger&logoColor=white)](https://ro-h-bots.blogspot.com/2026/07/engineered-window-rollers.html)
[![Instagram](https://img.shields.io/badge/@ro__h__bots-Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/ro_h_bots)

![FreeCAD](https://img.shields.io/badge/CAD-FreeCAD-418FDE?style=flat-square&logo=freecad&logoColor=white)
![FEM](https://img.shields.io/badge/Analysis-FEM%20%2B%20ParaView-6A4C93?style=flat-square)
![PETG](https://img.shields.io/badge/Printed%20in-PETG-2E7D32?style=flat-square)
![SKF](https://img.shields.io/badge/Bearing-SKF%20626--2RSH-005B99?style=flat-square)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg?style=flat-square)](http://creativecommons.org/licenses/by-nc-sa/4.0/)

</div>

---

## Overview

A project by [@RolandThsive](https://ro-h-bots.blogspot.com/p/about-me.html).

The rollers that came with my sliding windows kept failing — they deformed and cracked around the screws and the pulley holder under the weight of the glass. So I redesigned them from scratch: the weak spots are reinforced, the pulley runs on a sealed **SKF 626-2RSH** bearing, and every load-bearing part was checked with **Finite Element Analysis** before it was printed.

Each window pane weighs **10 kg** and rides on two symmetrically placed rollers, so each roller carries about **5 kg**. A spring-loaded pulley retracts for installation, and the roller screws in from the side so the pulley drops into the window's slot.

---

## Features

- **Reinforced where the originals failed** — around the screws and the pulley holder
- **SKF 626-2RSH sealed bearing** for smooth, quiet, long-lasting rolling
- **Hardened stainless-steel dowel pins** as axles instead of plastic pegs
- **Spring-loaded, retractable pulley** for easy installation and constant contact with the track
- **FEM-verified** in FreeCAD and ParaView — under 40 µm of deflection at full static load
- Printed solid — **PETG, 100% infill**

---

## Gallery

<div align="center">

| Full Assembly | Full Assembly — 3D Model |
| :---: | :---: |
| <img src="https://blogger.googleusercontent.com/img/a/AVvXsEg9bcYX-PTBF5_QqGlvZhowcvS3IYgyHNUN_Oqq0GiE43wO0MNCbLj_v32XEqOFPAvYsXokB5c-I4tR2Mg_hnIU2_xKJM2AL9jpK3oA-9V4MnAqMhhg2PqF6HYFfMPtiif6dX3BvyRwPwzCUDwhInIMmk_NvK_GyHqMzmFyxnaXrKcnALTJbZjZdYdPty_r=w640-h430" alt="Full Assembly" width="380"/> | <img src="https://RolandThsive.github.io/posters/WindowRoller_FullAssembly.png" alt="Full Assembly 3D model" width="380"/> |

*Want to spin it around? The blog post has an interactive 3D view of the full assembly.*

</div>

---

## Finite Element Analysis

Both printed load-bearing parts were analysed under static load in **FreeCAD FEM** (CalculiX) and post-processed in **ParaView**.

<div align="center">

| Free Body Diagram | Base Body — Forces & Constraints |
| :---: | :---: |
| <img src="https://blogger.googleusercontent.com/img/a/AVvXsEhGb0uKTnqnArcn4lwM5W9SQjQ8mzvfoqSSW9GJzDbeclddTjwxyZADL4tMaasTS81WIeWJcCKNeN-y17R2Tzu0FkyIItpQ9zCJLyIREjdtLT2lB0kd8_VbM9QUg5tdwgROJxCW9C13YzaUseI4jW9-xI4TIA2eCGPm2ODMw-n859DPtgptzSziqFa0uT_0=w640-h408" width="380"/> | <img src="https://blogger.googleusercontent.com/img/a/AVvXsEjl-8Qkc8vkUgb4PuoZ4hDfJdjn-0NaQacK4hyG4Jz-jtU5pDohwPKcjBWonpiMHZtuvEDE_rrLrIVSuJbvoHEV9hyLAY_XxL4F73dNkOzUs5LmOOVwlXSik0E7Y8EYUJMEG0J6v9OQUjFPRT9PdBSsEHraauF1B5JcJ6c7u2VDtvS6wpWhWMLxNAtO55-R=w640-h483" width="380"/> |
| **Undeformed Displacement — Base Body** | **Undeformed Displacement — Pulley Holder** |
| <img src="https://RolandThsive.github.io/posters/BaseBody_Displacement_Undeformed_Analysed.png" alt="Undeformed Displacement - Base Body" width="380"/> | <img src="https://RolandThsive.github.io/posters/PulleyHolder_Displacement_Undeformed_Analysed.png" alt="Undeformed Displacement - Pulley Holder" width="380"/> |

</div>

| Load case | Value |
| :--- | :--- |
| Load along Y | 50 N |
| Load along X | 68 N |

| Part | Max deflection (static) |
| :--- | :---: |
| Base Body | ~35 µm |
| Pulley Holder | ~17 µm |

The raw CalculiX results (`.vtu`) are in [`FreeCAD Files/Results_VTK_FREECAD/`](FreeCAD%20Files/Results_VTK_FREECAD) — open them in ParaView to explore the stress and displacement fields yourself. Dynamic load testing is next.

---

## Instructions

For the full write-up, FEM results and the interactive 3D model, head to the official blog post:
[Engineered Window Rollers](https://ro-h-bots.blogspot.com/2026/07/engineered-window-rollers.html)

### Printing

| Setting | Value |
| :--- | :--- |
| Material | PETG |
| Infill | 100% |
| Orientation | Top side down on the plate |

The printable parts are in [`Printables/`](Printables) as STEP files — import them straight into your slicer.

### Installing

1. Retract the pulley against its spring.
2. Slide the roller into place and screw it in from the side.
3. Let the pulley go — it engages the window's slot.

> [!TIP]
> Each pane needs **two** rollers. The BOM below is for **one** roller — double it per pane.

---

## Bill of Materials (BOM)

*Per roller.*

| Quantity | Item Description |
| :---: | :--- |
| **1x** | M5 x 35 mm Hex Head Allen Type Screw |
| **1x** | M5 Square Nut |
| **2x** | M5 Washer |
| **1x** | 8mm OD and 5mm ID Spring |
| **1x** | M3 x 25mm CSK Torx Screw |
| **1x** | M3 x 12mm StandOff |
| **1x** | SKF 626 - 2RSH Bearing |
| **1x** | M6 x 12mm Hardened SS Dowel Pin |
| **2x** | M2 x 12mm Hardened SS Dowel Pin |
| **1 Set** | 3D Printed Components - SET = BaseBody, Pulley and Pulley Holder |
| **1x** | B7000 Glue |

---

## Tools Required

| Tool | Description |
| :---: | :--- |
| **1x** | PB Swiss Allen type 4mm Hex Driver |
| **1x** | PB Swiss Torx type 8 Torx Driver |
| **1x** | Gressel/Proxxon 75mm Bench Vice |
| **1x** | A Set of Utility Tweezers |
| **1x** | Human Hands |

---

## Repository Structure

```
Window-Roller/
├── FreeCAD Files/
│   ├── FullAssembly.FCStd          # Complete assembly
│   ├── BaseBody.FCStd              # Printed parts
│   ├── PulleyHolder.FCStd
│   ├── Pulley.FCStd
│   ├── SKF_Bearing_626_2RSH.FCStd  # Hardware models
│   ├── 6x12_ROD.FCStd · Spring.FCStd · Standoffs.FCStd · Fastners.FCStd
│   └── Results_VTK_FREECAD/        # FEM results (.vtu) for ParaView
├── Full Assembly Step File/        # STEP of the complete assembly
├── Printables/                     # STEP files of the parts to print
├── LICENSE
└── README.md
```

---

## Connect With Me
* **Blog:** [ro-h-bots.blogspot.com](https://ro-h-bots.blogspot.com/)
* **Insta:** [@ro_h_bots](https://www.instagram.com/ro_h_bots?igsh=cDNkcnNpYnB5aWR1)

---

## License

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

<div align="center">

Made with love by **RolandThsive ([@RolandThsive](https://github.com/RolandThsive))**

</div>
