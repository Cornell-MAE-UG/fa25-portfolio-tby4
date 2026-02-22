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

![Pump System Schematic](https://cornell-mae-ug.github.io/fa25-portfolio-tby4/assets/images/system-diagram.png)
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
2.  **Single Inlet / Single Outlet:** There is one mass flow stream entering and one leaving (**m_dot_in = m_dot_out**).
3.  **Incompressible Flow:** Liquid water density is assumed constant (**rho ≈ 1000 kg/m³**).
4.  **Negligible Temperature Rise:** While real pumps generate some heat due to friction, the temperature change of the water is very small and is neglected here.
5.  **Adiabatic (Q_dot ≈ 0):** Heat transfer to the surroundings is neglected in the primary energy balance calculations because it is small compared to the mechanical work transfer.

*These assumptions allow us to reduce the complex general energy equation into a solvable form for mechanical work.*



## 5. Mass Balance
For the steady-flow control volume:
**m_dot_in = m_dot_out**

Because water is incompressible and flow is continuous:
**m_dot = ρ * Q**
*(Where Q is the volumetric flow rate)*




## 6. Energy Balance (First Law) — Steady Flow
The steady-flow energy equation:
**Q_dot - W_dot + m_dot * (h1 + V1²/2 + gz1) = m_dot * (h2 + V2²/2 + gz2)**

For the pump, shaft work is input to the fluid, so we define:
**W_dot_in ≈ m_dot * [ (h2 - h1) + (V2² - V1²)/2 + g(z2 - z1) ] - Q_dot**



## 7. Pump Performance (Efficiency)

Pump performance is characterized using **efficiency**, defined as the ratio of the useful mechanical energy gained by the fluid to the electrical energy supplied to the pump:

**Efficiency (η) = ( m_dot * [ (h2 - h1) + (V2^2 - V1^2)/2 + g(z2 - z1) ] ) / W_dot_elec**

Where:
*   **m_dot** is the mass flow rate.
*   **W_dot_elec** is the electrical power input.

This efficiency metric is the key factor used to evaluate how changes in operating conditions affect the overall pump performance.



## 8. Entropy Balance and Irreversibility

The pump is modeled as a steady-flow control volume. The entropy balance is:

**0 = m_dot * (s1 - s2) + (Q_dot / Tb) + S_dot_gen**

For normal operation, entropy generation (**S_dot_gen**) is positive due to friction, turbulence, and internal losses within the pump. These irreversibilities reduce the fraction of electrical energy converted into useful mechanical energy of the fluid.



## 9. Change in Operating Conditions

To evaluate performance changes, the effect of **restricting the outlet tubing** is considered.

Increasing flow resistance reduces the mass flow rate through the pump and increases losses within the system. As a result, a smaller fraction of the electrical power input contributes to increasing the fluid’s mechanical energy, leading to a **decrease in pump efficiency**. This behavior is consistent with increased irreversibility and entropy generation under higher resistance conditions.



## 10. Discussion of Assumptions

The pump is treated as operating at steady state with negligible heat transfer in the energy balance. In reality, because the pump is submersible, inefficiencies in the motor and fluid flow are dissipated as thermal energy into the surrounding water. This deviation from ideal assumptions does not significantly affect the primary mechanical energy analysis but explains why efficiency is less than unity.