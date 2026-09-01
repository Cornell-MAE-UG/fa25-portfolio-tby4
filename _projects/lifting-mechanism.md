---
layout: project
title: Acuator Lifting Mechanism
description: Designing a frame to lift the maximum possible weight using a linear actuator.
technologies: Tolomatic IMA
image: /assets/images/acuator.jpg

---

## Project Overview

**The Challenge:** The objective was to design a lifting mechanism within a constrained 2D design space (150 cm long by 50 cm tall) capable of lifting the maximum possible weight to the highest possible height. The system had to utilize a specific linear actuator ([Tolomatic IMA Series](https://www.tolomatic.com/wp-content/uploads/2022/05/2700-4000_29_IMA_cat.pdf)) and a rigid bar pivoted on the ground.

### Constraints & Objectives

- **Design Space:** 150 cm (Length) x 50 cm (Height)
- **Actuator:** Tolomatic IMA55 (selected for its high peak thrust of 35.81 kN)
- **Objective:** Maximize the load (W) and the vertical displacement (h)

## Step 1: Rigid Body Design & Static Analysis

### Design Definitions

To maximize the mechanical advantage and fit within the boundary, I established the following geometric design parameters:

- **Pivot Location (Support 1):** Placed at x = 135 cm. This allows the bar to swing backwards through the majority of the design space.
- **Actuator Base (Support 2):** Placed at x = 45 cm. This creates a wide, stable base triangle.
- **Bar Length:** 130 cm.
- **Actuator Attachment Point:** The actuator connects to the bar 90 cm away from the main pivot.

### Static Analysis

Treating the bar as a rigid body, I performed a static equilibrium analysis to determine the maximum weight the system could lift. I summed the moments about the main pivot point (C) to ensure the system remained in equilibrium.

![Static equilibrium weight calculation]({{ "/assets/images/weightCalculation.jpg" | relative_url }})
*Maximum lifting weight derived from the moment balance about the main pivot.*

### Actuator Selection

- **Selected Model:** Tolomatic IMA55 (Integrated Motor Actuator, Size 55)
- **Justification:** According to page 6 of the catalog, the IMA55 with a Roller Nut (RN05 or RN10) provides the highest peak thrust of approximately 35.81 kN (8,050 lbf).
- **Stroke:** Selected 450 mm (~18 inches) to allow sufficient lifting range within the 50 cm height limit.

## Step 2: Deformable Body (Beam) Analysis

### Maximum Deflection Analysis

While Step 1 assumed the bar was rigid, in reality the lifting arm acts as a beam that will bend under the applied load. To ensure the design is safe and functional, I modeled the bar as a deformable body to calculate the maximum deflection.

**Assumptions:**

- **Beam Model:** Analyzed as a simply supported beam with an overhang.
  - The ground pivot (x = 0) acts as a pin support.
  - The actuator connection (x = 0.9 m) acts as a roller support.
  - The weight (x = 1.3 m) acts as a point load at the free tip.
- **Force Components:** Per the design requirements, only vertical forces acting perpendicular to the beam axis were considered, as these generate the bending moments.
- **Linear Elasticity:** The material is assumed to operate within its elastic limit (Hooke's Law applies), returning to its original shape when the load is removed.

### Calculation

Maximum deflection occurs at the very tip of the beam where the weight is applied, using the standard deflection formula for an overhanging beam simply supported at 0 and a.

![Beam deflection and moment of inertia calculations]({{ "/assets/images/Calculations.jpg" | relative_url }})
*Deflection, beam sizing, and moment of inertia calculations for the lifting arm.*

### Beam Design & Material Selection

The objective was to design a beam that is mass-efficient (lightweight) while ensuring the vertical deflection does not exceed 2% of the total length.

To satisfy the mass-efficient requirement, a solid bar was rejected in favor of a hollow tube. A hollow profile maximizes the moment of inertia (I) relative to its weight because the material is distributed further from the neutral axis.

- **Selected Material:** Aluminum 6061-T6 (high strength-to-weight ratio)
- **Selected Profile:** Rectangular tube 4" x 2" x 0.25"
  - Height (H): 4 in
  - Width (W): 2 in
  - Wall Thickness: 0.25 in

### Design Verification

I calculated the actual moment of inertia for this specific tube to ensure it meets the requirement (see calculations above).

## Conclusion

Since the actual inertia (221 cm⁴) is significantly higher than the required inertia (95.8 cm⁴), this beam design will deflect approximately 1.1% of its length — well within the 2% safety limit.
