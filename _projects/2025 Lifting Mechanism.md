---
layout: project
title: Acuator Lifting Mechanism
description: Designing a fram to lift max possible weight
technologies: Tolomatic IMA
image: /assets/images/acuator.jpg
image: /assets/images/weightCalculation
image: /assets/images/Calculations

---

Project Overview: 

The Challenge: The objective was to design a lifting mechanism within a constrained 2D design space (150 cm long by 50 cm tall) capable of lifting the maximum possible weight to the highest possible height. The system had to utilize a specific linear actuator (Tolomatic IMA Series) and a rigid bar pivoted on the ground (https://www.tolomatic.com/wp-content/uploads/2022/05/2700-4000_29_IMA_cat.pdf).

Constraints & Objectives: 
    Design Space: 150 cm (Length) x 50 cm (Height)
    Actuator: Tolomatic IMA55 (Selected for its high peak thrust of 35.81 kN).  
    Objective: Maximize the Load (W) and the Vertical Displacement (h). 


Step 1: Rigid Body Design & Static Analysis

Design Definitions:
To maximize the mechanical advantage and fit within the boundary, I established the following geometric design parameters:
    Pivot Location (Support 1): Placed at x = 135 cm. This allows the bar to swing backwards through the majority of the design space.
    Actuator Base (Support 2): Placed at x = 45 cm. This creates a wide, stable base triangle.
    Bar Length: 130 cm.
    Actuator Attachment Point: The actuator connects to the bar 90 cm away from the main pivot.

Static Anlaysis:
Treating the bar as a rigid body, I performed a static equilibrium analysis to determine the maximum weight the system could lift. I summed the moments about the main pivot point (C) to ensure the system remained in equilibrium. The calculations are in weightCalculation.jpg

Actuator: 
    Selected Model: Tolomatic IMA55 (Integrated Motor Actuator, Size 55).
    Justification: According to Page 6 of the catalog, the IMA55 with a Roller Nut (RN05 or RN10) provides the highest Peak Thrust of approximately 35.81 kN (8,050 lbf).
    Stroke: Selected 450mm (~18 inches) to allow sufficient lifting range within the 50cm height limit.


Step 2: Deformable Body (Beam) Analysis

Maximum Deflection Analysis:
While the first step assumed the bar was rigid, in reality, the lifting arm acts as a beam that will bend under the applied load. To ensure the design is safe and functional, I modeled the bar as a deformable body to calculate the maximum deflection.

Assumptions: 
Beam Model: I analyzed the system as a simply supported beam with an overhang.
    The ground pivot (x=0) acts as a Pin Support.
    The actuator connection (x=0.9m) acts as a roller support.
    The weight (x=1.3m) acts as a point load at the free tip.
Force Components: As per the design requirements, I considered only the vertical forces acting perpendicular to the beam axis, as these generate the bending moments.
Linear Elasticity: I assumed the material operates within its elastic limit (Hooke’s Law applies), meaning it will return to its original shape when the load is removed.

Calculation:
Maximum deflection occurs at the very tip of the beam where the weight is applied. Using the standard deflection formula for an overhanging beam simply supported at 0 and a. 
Calculations in Calculations.jpg

Beam Design and Selection:
The objective was to design a beam that is mass-efficient (lightweight) while ensuring the vertical deflection does not exceed 2% of the total length
Calculations in calculations.jpg

Material & Cross-Section Selection:
To satisfy the "mass-efficient" requirement, a solid bar was rejected in favor of a hollow tube. A hollow profile maximizes the Moment of Inertia (I) relative to its weight because the material is distributed further from the neutral axis.

Selected Material: Aluminum 6061-T6 (High strength-to-weight ratio)
Selected Profile: Rectangular Tube 4'' x 2'' x 0.25''
    Height (H): 4in
    Width (W): 2in
    Wall Thickness: 0.25in

Design Verification: 
I calculated the actual Moment of Inertia for this specific tube to ensure it meets the requirement. 
Calculations in Calculations.jpg

Conclusion:
Since the actual inertia (221cm^4) is significantly higher than the required inertia (95.8cm^4), this beam design will deflect approximately 1.1% of its length, well within the 2% safety limit.