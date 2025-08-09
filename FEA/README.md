# FEA Results

This folder contains finite element analysis (FEA) results for the L1–L2 interbody cage.  
Simulation performed in Autodesk Fusion 360 (static stress, Ti-6Al-4V ELI, 1500 N axial load, inferior surface fixed).  
Images include von Mises stress distribution, displacement map, and safety factor visualization.  

**Note:** These are preliminary results using a coarse mesh. A refined mesh study will be conducted in the future for more accurate validation.

---

## Simulation Setup
- **Software:** Autodesk Fusion 360 – Static Stress Analysis module.
- **Geometry:** Concept CAD model of the L1–L2 interbody spinal fusion cage, including macro lattice structure and anti-migration teeth.
- **Material:** Ti-6Al-4V ELI (ASTM F136 medical-grade titanium alloy)  
  - Young’s Modulus: 110 GPa  
  - Yield Strength: 880 MPa  
  - Poisson’s Ratio: 0.34
- **Mesh:** Default parabolic solid mesh for initial study; future iterations will include localized mesh refinement on lattice struts and teeth.
- **Boundary Conditions:**
  - Inferior surface: Fully fixed to represent rigid contact with the lower vertebra.
  - Superior surface: Load applied over the full contact area.

## Load Cases
1. **Axial Compression**  
   - **Load:** 1,500 N applied vertically downward to the superior surface.  
   - **Rationale:** Represents peak physiological compressive load in the lumbar spine during daily activities.

2. **Compression-Shear** *(planned for future work)*  
   - Axial compression combined with a 250 N anterior shear force to simulate bending and torsional stresses.

3. **Subsidence Test** *(planned for future work)*  
   - Axial compression with rigid bone surrogate materials to evaluate endplate penetration risk in accordance with ASTM F2267.

4. **Torsional Loading** *(planned for future work)*  
   - Pure rotational load applied about the vertical axis to evaluate torsional stiffness.
  
---

## Von Mises stress plot 
<img width="1403" height="839" alt="Screenshot 2025-08-08 at 12 13 42 PM" src="https://github.com/user-attachments/assets/d456b277-0a88-4c44-91f3-28d7141e1d24" />

## Total displacement plot
<img width="1394" height="835" alt="Screenshot 2025-08-08 at 12 14 27 PM" src="https://github.com/user-attachments/assets/90382a72-b989-4a32-921e-804f8c4f55f1" />

## Safety factor plot
<img width="1396" height="834" alt="Screenshot 2025-08-08 at 12 15 23 PM" src="https://github.com/user-attachments/assets/73e6323f-97c3-45fb-9fe1-0d9bbeb5db31" />
