# Spinal Fusion Cage Implant

## Overview
This project contains the 3D CAD design of a **posterior-fixation L1–L2 interbody spinal fusion cage** with a rectangular lattice structure for enhanced bone ingrowth.  
The design is optimized for additive manufacturing using **Ti-6Al-4V ELI** titanium alloy (choosen for its unique properties), following general FDA Class II design considerations.  
Radiolucent markers are intended to be integrated (not included in the current CAD model) for postoperative X-ray visibility.

## Key Features
- **Dimensions**: Designed to match L1–L2 lumbar anatomy with a 5–6° wedge for restoring sagittal balance.  
- **Lattice Structure**: Rectangular lattice promotes osseointegration while maintaining structural strength.  
- **Pore Scaling Concept**: Pores are intentionally modeled larger in CAD to represent multiple smaller pores in the manufactured part, or to allow for filling with an osteoinductive gel during surgery.  
- **Posterior Fixation Compatibility**: No screw holes included in the design, as the device is intended to be fixed posteriorly with pedicle screws.  
- **Chamfered & Filleted Edges**: Reduces insertion trauma to surrounding tissue.
- **Anti-Migration Teeth**: Small, evenly spaced teeth on the top surface prevent implant slippage post-insertion.  
- **Rounded Corners**: Improves patient safety and reduces the risk of localized stress points during implantation.
- **Gel Formulation**: A theoretical osteoinductive gel formulation for pore filling is described in docs/osteoinductive_gel.md.”

## Finite Element Analysis (FEA)

A **static stress analysis** was performed in Autodesk Fusion 360 to evaluate the implant’s preliminary mechanical performance under physiological loading.
- **Material:** Ti-6Al-4V ELI (ASTM-compliant)  
- **Load Case:** 1,500 N axial compression applied to the superior surface  
- **Constraints:** Inferior surface fully fixed to simulate contact with the lower vertebra  
- **Mesh:** Default parabolic solid mesh (future work will include refined meshing around lattice struts and anti-migration teeth)  
- **Max von Mises stress:** ~14 MPa  
- **Max displacement:** ~0.001 mm  
- **Calculated factor of safety:** >60 (preliminary — will be updated after mesh refinement and validation)

*Note: Current results are from an initial coarse mesh and should be interpreted as a best-case scenario. Further refinement and validation will be performed.*



Results showed stress distribution well below the yield strength of Ti-6Al-4V ELI (~830 MPa), with minimal displacement and a factor of safety above 2.0, indicating robust structural performance under typical spinal loading.


## Files
- `3D_Models/spinal fusion cage.step` — Neutral CAD file for cross-platform CAD software compatibility. This file
- `3D_Models/spinal fusion cage.stl` — Mesh file for 3D printing and simulation purposes. This file can be open in any broswers for viewing only purposes.  

## Intended Use
**For educational and research purposes only.**  
This design is not intended for direct clinical use without regulatory approval, mechanical testing, and biocompatibility validation.

## Future Improvements
- Integration of **radiolucent markers** into the CAD model.
- Optimization of lattice geometry for specific mechanical strength targets.

## License
This project is licensed under the **MIT License** – see the [LICENSE] file for details.
