# **Spinal Fusion Cage Implant – Project Notes**

Degenerative disc disease, trauma, and age-related disc collapse can cause chronic pain, nerve compression, and reduced spinal stability.
This project presents the design and analysis of an L1–L2 interbody fusion cage engineered to restore load-bearing capacity while promoting osseointegration between adjacent vertebrae. The design follows FDA Class II guidelines and ASTM mechanical testing standards, with geometry optimized for surgical insertion, long-term stability, and compatibility with additive manufacturing. While the current device is intended as a stand-alone Class II implant, an optional osteoinductive gel upgrade is proposed, which would reclassify the device to FDA Class III as a combination product.

---

## **Design Overview**

### **Key Dimensions & Geometry**  
Dimensions were selected based on morphological data for the **average adult male L1–L2 intervertebral space**, ensuring anatomical compatibility and sufficient load-bearing surface area.  

- **Length:** 30 mm  
- **Width:** 12 mm  
- **Height (Posterior/Anterior):** 9 mm / 10 mm  
- **Wedge Angle:** ~5–6°  
- **Wall Thickness:** ~0.75 mm  
- Rectangular lattice architecture for high compressive strength, controlled stiffness, and optimized bone ingrowth.  
- **Anti-migration teeth** on superior and inferior surfaces (~0.5 mm height, ~1.0 mm spacing) to resist implant migration under cyclic loading.  
- Fully **rounded anterior/posterior edges** to minimize insertion trauma and reduce risk of endplate damage.  


### **Radiolucent Marker Placement**  
- Strategic positioning of radiolucent markers is critical for intraoperative placement verification and postoperative monitoring under X-ray and fluoroscopy.  
- In this concept-stage model, radiolucent markers were **not included** to prioritize geometry prototyping and lattice optimization in early iterations.  
- Final production designs will incorporate **tantalum or titanium alloy markers** embedded at **posterolateral and anterolateral corners**, ensuring visibility from multiple imaging angles without interfering with bone ingrowth.
- A marker housing can be integrated without affecting current geometry

---

## **Material Selection**  
- **Material:** Ti-6Al-4V ELI (**ASTM F136**), a medical-grade titanium alloy chosen for its exceptional **biocompatibility**, **high strength-to-weight ratio**, and **corrosion resistance** in physiological environments.  
- **Mechanical Properties:**  
  - **Young’s Modulus:** ~110 GPa — closer to cortical bone than stainless steel, reducing stress shielding.  
  - **Yield Strength:** ~880 MPa — comfortably above maximum physiological spinal loads, ensuring structural integrity.  
  - **Density:** ~4.43 g/cm³ — lightweight for patient comfort while maintaining mechanical strength.  
- **Rationale:** This alloy is the industry standard for spinal implants due to its proven performance in **osseointegration**, long-term durability, and compatibility with advanced manufacturing methods such as **EBM** (Electron Beam Melting) and **SLM** (Selective Laser Melting).  

---

## **Regulatory Classification**

  ### **Current Classification**
- **FDA Class II Medical Device** under *21 CFR §888.3080* – Intervertebral body fusion device.
- Covered by FDA Special Controls: **ASTM F2077**, **ASTM F2267**, and **ISO 10993** biocompatibility standards.

### **Upgrade to Class III**
- Adding **osteinductive gel** would reclassify this as a **combination product** (device + biologic) under *21 CFR §3.2(e)*.
- Which would require **Premarket Approval (PMA)** as per *21 CFR Part 814*.

---

## Osteoinductive Gel & Bone Integration Simulation

Portfolio R&D design for an **L1–L2 Ti-6Al-4V ELI interbody cage** with an **oste oinductive gel** to accelerate fusion.

- **Simulation:** FE mechanoregulation + agent-based modeling + diffusion–reaction transport, coupled across scales.
- **Gel:** Injectable hydrogel base (GelMA/HA-Tyramine) with staged VEGF → BMP-2 delivery, CaP nanoparticles, and optional exosomes/antimicrobial coating.
- **Integration:** In situ surgical injection into macro windows; fast crosslink or thermogel set for retention.
- **Regulatory:** Device only → Class II (FDA); add biologics → Class III PMA.

➡ Full technical details in (/OSTEOINDUCTIVE_GEL.md)

---

## **Pore Size Considerations**

### **Current State**  
The current lattice features oversized pores relative to the clinically optimal range. This was an intentional choice for the concept phase to accelerate CAD modeling, simplify visualization, and allow clear demonstration of the implant’s internal architecture during presentations.

### **Rationale**  
Producing a detailed lattice with clinically accurate pores (**300–700 µm**) would have significantly increased modeling time and computational load without impacting the validity of early mechanical simulations. Larger pores also make it easier to discuss potential filling materials, osteoinductive additives, or alternative scaffold geometries during the design review process. This oversized-to-final pore refinement approach mirrors common industry prototyping workflows, where early-stage designs prioritize manufacturability and visual inspection before committing to clinically accurate microarchitectures.

### **Solutions for Final Version**  
- Reduce pore size to **300–700 µm** in accordance with peer-reviewed literature on optimal osseointegration and bone ingrowth.  
- Maintain **interconnected porosity** for vascularization and nutrient transport.  
- Optionally fill pores with **osteinductive gel** or bone graft material at the time of surgery.  
- For simulation purposes, treat each oversized pore in the concept model as representing **multiple smaller pores** in the final manufactured implant.  

---

## **Finite Element Analysis (FEA)**  

### **Setup**  
- **Software:** Autodesk Fusion 360 – Static Stress Study.  
- **Load Case:** 1500 N axial compression applied to superior surface.  
- **Constraints:** Inferior surface fully fixed to simulate vertebral contact.  
- **Material:** Ti-6Al-4V ELI (ASTM F136 medical grade).  
- **Mesh:** Coarse global mesh due to computational limits; local refinement planned for lattice struts and anti-migration teeth in future iterations.  

### **Results**  
- **Max von Mises Stress:** ~14 MPa (*~1.6% of Ti-6Al-4V ELI yield strength of ~880 MPa*).  
- **Max Displacement:** ~0.001 mm (negligible under physiological loading).  
- **Factor of Safety:** >60 (indicates extremely conservative design margin).  

> **Interpretation:** Even with a coarse mesh, the analysis shows stress levels far below material yield limits and minimal deformation, confirming high structural integrity under typical lumbar spinal loads. Despite the coarse mesh, the results remain valid because axial load paths are carried primarily through the continuous outer walls and primary lattice struts, meaning the simulation still captures the dominant structural behavior under physiological compression. Additional mesh refinement will be conducted to validate results with greater accuracy.

---

## **Standards & Testing Requirements**  
- **ASTM F2077** – Standard test methods for intervertebral body fusion devices, including **static compression**, **compression-shear**, and **torsion** testing to verify mechanical strength.  
- **ASTM F2267** – Evaluates **subsidence resistance**, ensuring the cage maintains vertebral height without sinking into the bone under load.  
- **ISO 10993** – **Biological evaluation of medical devices**; verifies biocompatibility through cytotoxicity, sensitization, and implantation testing.  
- **FDA Special Controls** – Compliance with *21 CFR §888.3080* requirements for Class II spinal systems, including mechanical testing, material safety, and labeling.  
- **ASTM F136** – Material specification for **Ti-6Al-4V ELI** used in surgical implants; ensures chemical composition, mechanical properties, and microstructure meet medical-grade standards.  

---

## **Manufacturing Notes**  
- Optimized for **additive manufacturing** using **EBM** (Electron Beam Melting) or **SLM** (Selective Laser Melting).  
- Post-processing steps include **Hot Isostatic Pressing (HIP)** to eliminate porosity, surface blasting to enhance osseointegration, and anodizing for additional corrosion resistance.  
- Design supports **scalable production**, from patient-specific customization to large-scale manufacturing.  

---

## **Future Development**
- Refined pore sizes for optimal biological response.  
- Marker material optimization.  
- Custom anatomical matching.  
- In-vitro and cadaveric testing.

---

