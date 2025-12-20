---
layout: project
title: Water Pump Analysis 
description: This portfolio analyzes a submersible centrifugal water pump used to circulate water in small systems such as aquariums and tabletop fountains. 
technologies: VIVOSUN Submersible Pump
image: /assets/images/aquaPump.png
---


## 1. Device Selection and Real-World Context

### 1.1 Device Overview
The device analyzed in this portfolio is a **VIVOSUN 400 GPH Submersible Pump**, a commercially available small centrifugal pump designed to circulate water in tanks, fountains, and small process loops. According to the manufacturer, this pump is suitable for applications such as aquariums, hydroponic systems, and tabletop water circulation.

**Product reference:**
[VIVOSUN 400 GPH Submersible Pump Product Page](https://vivosun.com/vivosun-400gph-submersible-pump-for-fish-tank-p58820960379607248-v58820960379607238)

This pump is powered by an electric motor housed within a waterproof casing. The motor drives a centrifugal impeller that increases the mechanical energy of the water, thereby increasing its pressure and allowing it to flow through connected tubing against gravity and friction.

### 1.2 Real-World Examples of Pumps
Pumps similar to this one are used in many engineering and everyday contexts, including:

*   Building HVAC hydronic loops (circulator pumps)
*   Municipal and industrial water distribution
*   Cooling loops in power plants and machinery
*   Automotive cooling systems
*   Aquaculture and hobbyist water circulation

These applications all share the common thermodynamic principle that a pump is a **work-input device** that transfers mechanical work to a fluid to increase its mechanical energy.



## 2. System Diagram and Thermodynamic Analysis

### 2.1 Control Volume Description
The system is modeled as a **Steady-Flow Control Volume (CV)** enclosing the pump mechanism. The boundary cuts through the inlet pipe (suction side) and the discharge tubing (outlet side), as well as the electrical driveshaft.

![Pump System Schematic](/assets/images/system-diagram.png)
*Figure 1: Schematic of the pump control volume showing states and energy interactions.*



## 3. Qualitative Description of Operation

The VIVOSUN 400 GPH is a **centrifugal submersible pump**. Instead of using a piston to push water, it relies on rotational motion to create pressure.

**How it works:**
1.  **Energy Input:** An electric motor spins a shaft connected to an **impeller**.
2.  **Kinetic Energy:** Water enters the center (eye) of the impeller and is flung outward by centrifugal force, gaining high velocity.
3.  **Pressure Build:** The water hits the stationary casing (volute) and slows down. This deceleration converts the kinetic energy into **static pressure**, which pushes the water out of the discharge tube.

**Thermodynamic Reality:**
In an ideal scenario, all input work would create pressure. However, in this real-world device:
*   **Irreversibilities:** Friction and turbulence create energy losses.
*   **Entropy:** These losses increase the entropy of the fluid.
*   **Heat Transfer:** Since the pump is submersible, any waste heat from the motor or friction is dissipated directly into the water, though this temperature rise is usually negligible.



## 4. System Definition and Assumptions

### 4.1 Control Volume
The Control Volume (CV) is defined as the interior of the pump housing. It encompasses the impeller and the internal flow passages, cutting through the inlet and outlet ports. Mass enters continuously at the inlet and leaves at the outlet.

### 4.2 Key Assumptions
To simplify the thermodynamic analysis, the following assumptions are made:

1.  **Steady-flow operation:** The pump operates continuously; properties at the inlet and outlet do not change with time.
2.  **Single Inlet / Single Outlet:** There is one mass flow stream entering and one leaving ($\dot{m}_{in} = \dot{m}_{out}$).
3.  **Incompressible Flow:** Liquid water density is assumed constant ($\rho \approx 1000 \text{ kg/m}^3$).
4.  **Negligible Temperature Rise:** While real pumps generate some heat due to friction, the temperature change of the water is very small and is neglected here.
5.  **Adiabatic ($\dot{Q} \approx 0$):** Heat transfer to the surroundings is neglected in the primary energy balance calculations because it is small compared to the mechanical work transfer.

*These assumptions allow us to reduce the complex general energy equation into a solvable form for mechanical work.*



## 5. Mass Balance
For the steady-flow control volume:
$$ \dot{m}_{in} = \dot{m}_{out} $$

Because water is incompressible and flow is continuous:
$$ \dot{m} = \rho Q $$
*Where $Q$ is the volumetric flow rate.*

## 6. Energy Balance (First Law) — Steady Flow
The steady-flow energy equation is given by:
$$ \dot{Q} - \dot{W} + \dot{m}\left(h_1 + \frac{V_1^2}{2} + gz_1\right) = \dot{m}\left(h_2 + \frac{V_2^2}{2} + gz_2\right) $$

For the pump, shaft work is input to the fluid. Rearranging for work input ($\dot{W}_{in}$):
$$ \dot{W}_{in} \approx \dot{m} \left[ (h_2 - h_1) + \frac{V_2^2 - V_1^2}{2} + g(z_2 - z_1) \right] - \dot{Q} $$