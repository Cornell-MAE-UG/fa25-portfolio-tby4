---
layout: project
title: Spotted Lanternfly Separation System
image: /assets/images/slf-cad-model.png
permalink: /projects/slf-separation/
---

# Spotted Lanternfly Separation System

**Team:** Grape Soup  
**Client:** Cornell CALS Extension / E&J Gallo Winery / National Grape  

A density-based mechanical separation system designed to remove Spotted Lanternflies from harvested grapes before downstream juice or wine processing.

## Milestones

- [Client Pitch](#client-pitch)
- [Functional Prototype](#functional-prototype)
- [Client Report](#client-report)

---



# Client Pitch

## Problem Statement

During mechanical grape harvesting, grapes are collected alongside debris and insects such as Spotted Lanternflies (SLFs). A key challenge arises because approximately **50% of the harvested grapes are crushed into “grape soup”**, making traditional washing methods ineffective—washing would result in significant product loss.

As a result, SLFs and debris enter downstream processing, contaminating juice and wine production. Current solutions rely heavily on manual sorting or inefficient removal methods, increasing labor costs and reducing processing efficiency.

---

## Why This Matters

This problem directly impacts large-scale vineyard operations:

- **Product Quality:** Contamination affects final wine and juice quality  
- **Operational Efficiency:** Manual sorting is slow and labor-intensive  
- **Economic Impact:** Lost yield and added labor increase costs  
- **Scalability:** Existing methods do not scale well with mechanical harvesting  

A successful solution would provide a **reliable, scalable, and automated method** for removing SLFs from harvested grapes.

---

## Proposed Solution

We propose a **post-harvest mechanical separation system** based on density differences between grapes and SLFs.

### Core Concept

- Grapes (3–5 g) → **sink**
- SLFs (fraction of a gram) → **float**

### System Design

1. **Liquid-Solid Separation Stage**  
   Removes excess grape juice (“grape soup”)

2. **Flotation Tank**  
   Enables density-based separation

3. **Surface Skimming Mechanism**  
   Removes floating SLFs using a rotating paddle

4. **Bottom Drain System**  
   Allows clean grapes to exit for further processing

---

## Prototype Goal

The goal of the prototype is to demonstrate:

- Reliable SLF removal using buoyancy  
- Minimal or zero grape loss  
- Consistent mechanical operation  
- Feasibility for scaling to industrial use  

---

## Key Risks / Unknowns

Several uncertainties could impact the success of this design:

- **Fluid Dynamics:** Will water agitation cause grapes to be unintentionally removed?
- **Selective Removal:** Can the paddle reliably remove only floating SLFs?
- **Material Interaction:** Does water exposure affect grape quality?
- **Scaling:** Can the system handle real vineyard throughput?

---

## Questions for the Client

To guide further development, we identified key questions:

1. **What level of contamination is acceptable?**  
   → Determines required removal efficiency

2. **What processing time constraints exist?**  
   → Impacts system speed and throughput design

3. **Are water-based solutions acceptable in current workflows?**  
   → Affects feasibility of implementation

4. **What scale of operation is required?**  
   → Guides system sizing and design constraints

---

## Summary

This proposal focuses on a **targeted, high-impact intervention point** in the harvesting process. By addressing contamination at the post-harvest stage, the system avoids the complexity of vineyard-wide solutions while maximizing impact on the final product.







# Functional Prototype

## Prototype Purpose

The functional prototype was developed to validate the feasibility of a **density-based separation system** and evaluate whether a simple mechanical design could reliably remove floating SLF simulants while preserving grapes.

The prototype specifically aimed to:
- Test buoyancy-based separation
- Evaluate mechanical reliability of the paddle system
- Identify design limitations before final iteration

---

## Design Overview

<figure>
  <img src="{{ '/assets/images/slf-cad-model.png' | relative_url }}" alt="CAD model of SLF separation system" style="width:70%;">
  <figcaption><b>Figure 1:</b> CAD model of the density-based separation system showing the flotation tank, paddle mechanism, and crank input.</figcaption>
</figure>

The system consists of four main subsystems:

1. **Container / Flotation Tank**  
   A plastic storage container holds water and serves as the separation environment.

2. **Paddle Wheel Mechanism**  
   A rotating paddle interacts only with the surface layer to remove floating SLFs.

3. **Crank Input System**  
   A manually operated crank provides rotational motion to the paddle.

4. **Support Bracket System**  
   Holds the shaft in place and maintains alignment during rotation.

---

## Prototype Implementation

<figure>
  <img src="{{ '/assets/images/slf-first-prototype.jpg' | relative_url }}" alt="First functional prototype" style="width:70%;">
  <figcaption><b>Figure 2:</b> First functional prototype constructed using a plastic container, cardboard paddle system, and taped mounting structure.</figcaption>
</figure>

The initial prototype was constructed using:
- Cardboard (paddle + structure)
- Plastic container (tank)
- Tape and adhesive (mounting + joints)
- Cylindrical shaft (rotation axis)

This version allowed rapid testing of:
- Paddle motion
- Surface interaction
- Basic separation feasibility

---

## Component-Level Design

<figure>
  <img src="{{ '/assets/images/slf-components.png' | relative_url }}" alt="CAD components: paddle, crank, bracket" style="width:70%;">
  <figcaption><b>Figure 3:</b> CAD models of key components: paddle geometry, crank input mechanism, and bracket for shaft support.</figcaption>
</figure>

### Key Components

- **Paddle:**  
  Designed to maximize surface contact while avoiding disturbance of submerged grapes.

- **Crank:**  
  Converts manual input into rotational motion for controlled operation.

- **Bracket:**  
  Maintains shaft alignment and prevents unwanted motion during operation.

---

## Design Testing

### 1. Motion & Interference Testing
- Paddle rotated through full range of motion  
- **Result:** No binding, collision, or misalignment observed  

---

### 2. Repeat-Use Testing
- Operated at ~60 RPM for ~1 minute  
- **Result:** No loosening, cracking, or increased wobble  

---

### 3. Interference Testing
- Checked clearance between paddle and container walls  
- **Result:** No contact or obstruction  

---

### 4. Functional Separation Testing
- Tested with grapes and SLF simulants (marker caps)  
- **Result:** Successful surface skimming of floaters  

---

## Key Observations

- Paddle consistently interacted only with the surface layer  
- Grapes remained undisturbed at the bottom  
- System operated reliably across multiple cycles  
- Minor instability observed due to flexible mounting  

---

## Success Criteria

### Separation Efficiency
- Target: ≥80% removal  
- Achieved: ~83%

### Grape Loss
- Target: <2%  
- Achieved: 0%

### Processing Time
- Higher speeds significantly reduced separation time  

### Reliability
- Multiple trials completed without mechanical failure  

---

## Design Limitations

- Tape-based mounting introduced slight misalignment  
- Water agitation increased at higher speeds  
- Prototype not optimized for continuous operation  

---

## Summary

The functional prototype successfully demonstrated that:

- Density-based separation is feasible  
- A simple paddle mechanism can selectively remove floaters  
- The system meets key performance targets  

These results justified further refinement and development into a more robust and scalable final prototype.









# Client Report

## Final Prototype & Application

<figure>
  <img src="{{ '/assets/images/slf-final-prototype.jpg' | relative_url }}" alt="Final SLF separation prototype" style="width:70%;">
  <figcaption><b>Figure 4:</b> Final assembled separation system demonstrating flotation-based SLF removal with integrated paddle mechanism and drainage setup.</figcaption>
</figure>

We developed a **density-based separation system** designed for integration into vineyard receiving areas. The system targets the post-harvest stage, where harvested grapes and debris are processed before entering juice or wine production.

### Process Workflow

1. Harvested material is emptied into a **funnel separator**  
2. Liquids (“grape soup”) are filtered out  
3. Remaining solids enter a **water-filled flotation tank**  
4. Grapes (3–5 g) sink due to higher density  
5. SLFs (lighter) float to the surface  
6. A **rotary paddle mechanism** removes floating SLFs  
7. Clean grapes exit through a bottom drainage system  

This approach leverages fundamental density differences to achieve selective separation without complex sensing or sorting systems :contentReference[oaicite:0]{index=0}.

---

## Testing & Results

<figure>
  <img src="{{ '/assets/images/slf-results-table.png' | relative_url }}" alt="Experimental results table" style="width:80%;">
  <figcaption><b>Figure 5:</b> Experimental results showing SLF removal efficiency across different rotational speeds.</figcaption>
</figure>

Prototype testing validated the effectiveness of the separation system under different operating conditions.

### Key Results

- **Removal Efficiency:** ~83% across both low and high speeds  
- **Grape Loss:** 0% observed  
- **Processing Time:** Reduced significantly at higher RPM  
- **Repeatability:** Consistent performance across multiple trials  

### Interpretation

- Increasing rotational speed improves processing time **without reducing efficiency**  
- Paddle mechanism successfully interacts only with the surface layer  
- No grapes were unintentionally removed during testing  

These results meet the target performance criteria of ≥80% removal efficiency and <2% grape loss :contentReference[oaicite:1]{index=1}.

---

## Performance Observations

- At higher speeds, **water agitation increases**, introducing potential instability  
- Minor jamming occurred due to rigid marker caps (not representative of real SLFs)  
- Real SLFs are expected to deform, reducing interference risk  

The system maintained stable operation across repeated trials without failure.

---

## Prototype Evolution

The design progressed through three stages:

1. **Cardboard Prototype**  
   → Validated basic concept and geometry  

2. **Wood Prototype**  
   → Enabled motion, interference, and durability testing  

3. **3D Printed Prototype**  
   → Improved alignment, stiffness, and repeatability  

Each iteration refined the system’s mechanical performance and reliability.

---

## Conclusion

The prototype demonstrates that **buoyancy-based separation combined with a simple mechanical paddle system is an effective solution** for SLF removal.

Key achievements:

- High removal efficiency (~83%)  
- Zero grape loss  
- Reliable mechanical operation  
- Low system complexity  

This validates the core concept and supports further development toward real-world implementation :contentReference[oaicite:2]{index=2}.

---

## Recommendations / Next Steps

To advance the design:

- Add a **controlled drainage valve** for continuous operation  
- Improve **water level stability** at higher speeds  
- Optimize **paddle geometry** to reduce agitation  
- Scale system for **higher throughput testing**  
- Integrate into existing processing workflows  

---

## Bill of Materials

| Component | Description | Cost ($) |
|----------|------------|---------|
| Plastic Tank | Flotation container | 45.23 |
| Lid | (unused in final) | 9.19 |
| 3D Printed Brackets | Shaft support | 3.50 |
| 3D Printed Crank | Manual input | 3.86 |
| 3D Printed Paddle | Surface skimming | 53.31 |
| Adhesives | Bonding materials | 0.00 |
| Scrap Rubber | Paddle extension | 0.00 |
| **Total** |  | **115.09** |

---

## Final Takeaway

This project delivers a **low-cost, scalable mechanical solution** to a real agricultural problem. By leveraging simple physical principles, the system achieves strong performance while remaining practical for integration into existing vineyard operations.