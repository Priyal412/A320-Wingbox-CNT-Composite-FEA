# CNT-Functionalized CFRP for Aircraft Airframe Structures
### Master's Thesis — Moscow Aviation Institute (MAI), 2024
**Author:** Priyal Chaturvedi | **Program:** M.Sc. Aerospace Engineering (Aircraft Design) | **Department:** Institute No.1 "Aviation Technology", Faculty 101

---

## Overview

This research investigates the feasibility of using **Carbon Nanotube (CNT)-functionalized Carbon Fiber Reinforced Polymer (CFRP)** composites as a structural material for aircraft airframe components — specifically the **A320 wingbox**.

The aviation industry demands materials that are simultaneously lightweight, strong, and stiff. While conventional CFRP is already widely used (Boeing 787, Airbus A350), this study explores whether embedding Single-Walled Carbon Nanotubes (SWCNTs) in the fiber-matrix interphase region can push material performance further.

---

## Research Objectives

- Characterize the mechanical properties of CNT-functionalized IM7/8552 CFRP at micro, meso, and macro scales
- Model the CNT interphase using **Christensen's Generalized Self-Consistent Method**
- Perform multi-scale **Finite Element Analysis (FEA)** using ABAQUS
- Compare induced stresses and deformations in an A320 wingbox made of conventional CFRP vs CNT-functionalized CFRP

---

## Methodology

### Scale 1 — Micro-scale: CNT Interphase Modelling
- SWCNTs embedded in the interfacial region between IM7 carbon fiber and 8552 epoxy matrix
- A Representative Volume Element (RVE) unit cell was developed to model the CNT-functionalized interphase
- Christensen's three-phase composite model used to estimate interphase elastic properties

### Scale 2 — Meso-scale: Laminate Analysis
- Classical Laminate Theory (CLT) applied to build up ply-by-ply properties
- Quasi-isotropic layup `[0/±45/90]s` evaluated for both conventional and CNT-reinforced CFRP
- Engineering constants (E₁₁, E₂₂, G₁₂, ν₁₂) predicted for comparative study

### Scale 3 — Macro-scale: A320 Wingbox FEA
- Full wingbox geometry modelled in ABAQUS with 6 equivalent ribs and realistic boundary conditions
- Aerodynamic loading applied based on A320 wing geometry parameters
- Results: maximum displacement, maximum principal stress compared between the two material systems

---

## Tools & Software

| Tool | Purpose |
|---|---|
| **ABAQUS** | FEA modelling at all scales (unit cell, laminate, wingbox) |
| **Classical Laminate Theory** | Analytical prediction of laminate properties |
| **Christensen's Self-Consistent Model** | Interphase property estimation |
| **Microsoft Excel / MATLAB** | Data processing and engineering constant calculations |

---

## Key Results

### Material Properties — CNT Reinforced IM7/8552

| Property | Value |
|---|---|
| E₁₁ | 52.14 GPa |
| E₂₂ | 52.88 GPa |
| E₃₃ | 13.97 GPa |
| G₁₂ | 4.06 GPa |
| G₁₃ | 6.47 GPa |
| ν₁₂ | 0.42 |

### Wingbox FEA — Comparison Summary

| Parameter | Conventional CFRP | CNT-Functionalized CFRP |
|---|---|---|
| Max Displacement | ~1.199 m | Marginally lower |
| Max Principal Stress | ~889 MPa | ~796 MPa (**~10% lower**) |

> The CNT-functionalized composite demonstrated improved interphase strength, leading to reduced plastic strain in the fiber and matrix. While the improvement did not scale linearly to the macro level, the wingbox made of CNT-CFRP showed slightly better stress distribution overall.

---

## Figures

### A320 Wingbox Model in ABAQUS
![Wingbox Model](images/wingbox_model_abaqus.jpg)

### FEA Results — Conventional CFRP: Displacement & Max Principal Stress
![FEA Displacement and Stress - Conventional](images/fea_displacement_stress_conventional.jpg)

### FEA Results — CNT Composite: Max Principal Stress
![FEA Stress - CNT Composite](images/fea_stress_cnt_composite.jpg)

### Wing Deformation Under Load
![Wing Deformation](images/fea_wing_deformation.jpg)

### CNT Composite Engineering Constants (ABAQUS Output)
![Engineering Constants](images/engineering_constants_cnt.jpg)

---

## Conclusions

1. CNTs in the interphase region **significantly enhanced local strength** — the high stiffness of SWCNTs (E ~ 1 TPa) improved the interphase modulus considerably
2. However, these gains **did not translate linearly** to the laminate or structural level due to the small volume fraction of CNTs relative to the total composite
3. The A320 wingbox made of CNT-functionalized CFRP showed **comparable or slightly better** performance vs conventional CFRP
4. Further optimization of CNT volume fraction and investigation of different fiber whisker geometries is recommended before industrial adoption

---

## Future Work

- Optimize CNT volume fraction (current: ~1%) for better macro-scale property improvement
- Investigate multi-walled CNTs (MWCNTs) and other whisker geometries
- Conduct experimental validation of predicted elastic constants
- Extend analysis to dynamic loading, fatigue, and impact resistance

---

## Full Thesis

The complete thesis document is available here: [Masters_Thesis_Priyal_Chaturvedi.pdf](Masters_Thesis_Priyal_Chaturvedi.pdf)

---

## References (Key)
- Christensen & Lo (1979) — Generalized Self-Consistent Model
- Chatzigeorgiou, Seidel et al. (2012) — Effective mechanical properties of fuzzy fiber composites
- Tsai & Azzi (1965) — Elastic moduli of laminated anisotropic composites
- Seidel & Lagoudas (2006) — Micromechanical analysis of CNT-reinforced composites

---

*Moscow Aviation Institute (MAI) | Faculty 101 — Aircraft Design | 2022–2024*
