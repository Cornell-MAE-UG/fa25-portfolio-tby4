---
layout: project
title: Spotted Lanternfly Separation System
permalink: /projects/slf-separation/
---

# Spotted Lanternfly Separation System  
**Team: Grape Soup**  
**Client: Cornell CALS Extension / E&J Gallo Winery / National Grape**

---

## Project Overview

The goal of this project is to remove Spotted Lanternflies (SLFs) from harvested grape batches before they enter downstream processing. Current harvesting methods are non-selective, allowing insects and debris to contaminate grape “soup,” reducing quality and increasing processing costs.

Our team developed a **density-based mechanical separation system** that leverages the natural buoyancy difference between grapes and SLFs. Grapes (3–5 g) sink, while SLFs float and are mechanically removed.

---

## Milestones (Click to Navigate)

- [Client Pitch](#client-pitch)
- [Functional Prototype](#functional-prototype)
- [Client Report](#client-report)

---

# Client Pitch

## Problem Statement

During mechanical harvesting, grapes are collected along with debris and insects such as Spotted Lanternflies (SLFs). Approximately **half of the harvested grapes are crushed into “grape soup”**, making traditional washing ineffective due to yield loss.

This creates a contamination problem during post-harvest processing, requiring manual sorting or risking reduced product quality.

## Why It Matters

- Reduces contamination in wine/juice production  
- Minimizes manual labor costs  
- Improves efficiency in large-scale vineyard operations  
- Provides a scalable solution integrated into existing workflows  

## Proposed Solution

We proposed a **post-harvest density-based separation system**:

1. Liquid-solid separation stage  
2. Flotation tank  
3. Surface skimming mechanism  

Key idea:
- Grapes sink  
- SLFs float → removed mechanically  

### Prototype Goal
A small-scale system demonstrating:
- Reliable separation  
- Minimal grape loss  
- Repeatable operation  

## Key Risks / Unknowns

- Will agitation cause grape carryover?
- Can the paddle reliably remove only floaters?
- Does water exposure affect grape quality?
- Can the system scale to industrial throughput?

## Questions for Client

- What level of contamination is acceptable?
- How much processing time can be added?
- Are water-based systems acceptable in workflow?
- What throughput is required?

---

# Functional Prototype

## Prototype Purpose

The functional prototype was built to:
- Validate density-based separation  
- Test mechanical reliability  
- Evaluate system performance under repeated use  

---

## Design Overview

The system consists of:

- **Funnel separator** → removes excess liquid  
- **Water tank** → enables density separation  
- **Rotary paddle** → skims floating SLFs  
- **Drain system** → removes clean grapes  

---

## Design Documentation

### Key Components

- Plastic tank (4.5 gal)
- 3D printed paddle, crank, and brackets
- Epoxy + adhesive bonding
- Rubber extension for paddle reach

### Assembly

- Brackets mounted to container using epoxy  
- Paddle connected to crank mechanism  
- Manual rotation drives surface skimming  

---

## Design Testing

### 1. Motion & Interference Test
- Paddle rotated through full motion range  
- **Result:** No collisions or binding  

### 2. Repeat-Use Test
- Operated at ~60 RPM for 1 minute  
- **Result:** No structural failure or loosening  

### 3. Interference Test
- Checked paddle clearance vs walls  
- **Result:** No contact observed  

### 4. Stability Test
- System operated across multiple trials  
- **Result:** Stable with minor water displacement  

---

## Success Criteria

### Separation Efficiency
- Target: ≥80% SLF removal  
- Achieved: ~83%

### Grape Loss
- Target: <2%  
- Achieved: 0%

### Processing Time
- Faster operation at higher RPM  

### Reliability
- Multiple consecutive runs without failure  

---

# Client Report

## Final Design

We developed a **density-based separation system installed at vineyard receiving areas**.

### Process Flow:
1. Harvest dumped into funnel  
2. Liquids separated  
3. Solids enter flotation tank  
4. Grapes sink  
5. SLFs float  
6. Paddle removes SLFs  
7. Grapes drain out  

---

## Testing & Results

### Performance Data

| Speed | Removal | Time |
|------|--------|------|
| ~8.3 RPM | 4–6 / 6 | 40–60 sec |
| ~16.5 RPM | 5 / 6 | ~20 sec |

### Key Findings

- ~83% removal efficiency across all tests  
- 0% grape loss  
- Faster speeds reduce processing time  
- Paddle interacts only with surface layer  

---

## Observations

- Higher RPM increases water agitation  
- Potential risk of instability at scale  
- Marker caps (simulants) occasionally jammed  
- Real SLFs expected to perform better  

---

## Prototype Evolution

1. Cardboard → concept validation  
2. Wood → functional testing  
3. 3D printed → final prototype  

Each stage improved:
- Alignment  
- Structural integrity  
- Repeatability  

---

## Conclusion

The system successfully demonstrates that **density-based separation is a viable and effective method** for SLF removal.

- High efficiency  
- No grape loss  
- Simple mechanical design  

This validates the concept for further development.

---

## Recommendations / Next Steps

- Add controlled drainage valve  
- Improve water level stability  
- Optimize paddle geometry  
- Scale system for continuous operation  

---

## Bill of Materials

| Component | Cost |
|----------|-----|
| Tank | $45.23 |
| Lid | $9.19 |
| Paddle | $53.31 |
| Brackets + Crank | ~$7 |
| Adhesives | $0 |
| **Total** | **$115.09** |

---

## Final Takeaway

This project demonstrates a **low-cost, scalable mechanical solution** to a real agricultural problem. By leveraging basic physics (density separation), the system achieves strong performance with minimal complexity.
