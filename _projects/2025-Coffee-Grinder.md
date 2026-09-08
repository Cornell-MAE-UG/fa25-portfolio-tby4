---
layout: project
title: Coffee Grinder
description: A hand-crank coffee grinder redesigned around off-the-shelf components, modeled and motion-verified in Fusion 360.
technologies: Fusion 360, McMaster-Carr Component Sourcing
image: /assets/images/Coffee-Grinder.png
---

## Overview

This project started from a 1930s Peugeot coffee grinder as a reference for the core mechanism — a crank handle, a pair of miter gears, and a pair of conical burrs — and asked a different question than most CAD exercises: **can this be built almost entirely from parts you can actually buy?**

Rather than modeling every part from scratch, the goal was to source real components from McMaster-Carr wherever possible, and reserve custom fabrication for the few parts that genuinely required it. That constraint changed the design process — instead of drawing a shaft at whatever diameter looked right, I had to design around the bore sizes, tooth counts, and lengths that actually exist in a supplier's catalog.

## Design Process

**1. Sketch the backbone.**
The core kinematic chain was fixed: crank handle → horizontal shaft → miter gear pair → vertical shaft → conical burr pair. My job was to design everything *around* that chain — a frame to support the shafts, a hopper for whole beans, and clearance for ground coffee to fall into a cup below.

![Initial sketch of the full grinder assembly](/assets/images/Sketch-Grinder-Full.jpeg)

![Sketch detailing the inner burr and bean entry](/assets/images/Sketch-Grinder-Inner.jpeg)

**2. Search, then redesign around what's available.**
I searched McMaster-Carr for every component in the chain and only accepted parts with downloadable CAD. This is a different workflow than pure top-down design — a few iterations were driven by "the miter gear I want doesn't come in a 6mm bore, so the shaft diameter changes," rather than the other way around. The sketch and shaft dimensions were adjusted several times as the component search progressed.

**3. Model the custom parts and verify motion in CAD.**
Three parts couldn't be sourced off-the-shelf and were modeled from scratch: the horizontal drive shaft, the vertical drive shaft (with a hex end machined for the burr and a threaded top for a retaining nut), and the base/frame. Everything else — the crank handle and the miter gear pair — is a real McMaster part number.

The conical burr set is the one exception to "buy or fabricate": it's a highly specialized geometry that isn't available from McMaster or campus manufacturing resources, so I used a reverse-engineered CAD file of the burr set (sourced from GrabCAD) rather than modeling it myself. Everything else in the assembly is either a cataloged part or my own design.

**4. Assemble and check for a working mechanism.**
The final assembly uses rigid joints only at true fastened interfaces (bolted/threaded connections) and revolute joints at the shafts, so turning the crank drives the miter gears, which drive the vertical shaft and inner burr — the full assembly moves as a real grinder would, with no interference between parts and nothing held up only by the CAD software's imagination.

## Component List

| Qty | Part | Source | Specs |
|---|---|---|---|
| 1 | Offset crank handle | McMaster-Carr 6544N11 | 80 mm length, 8 mm unthreaded hole |
| 2 | Carbon steel miter gear | McMaster-Carr 2600N1 | 8 mm bore, 20 teeth, 1 module, 1:1 ratio |
| 1 | Horizontal drive shaft | Custom (steel rod) | 8 mm OD, 50 mm length |
| 1 | Vertical drive shaft | Custom (steel rod) | 8 mm OD, hex end (3.753 mm side) for burr attachment, M8×1.25 threaded top |
| 1 | Base/frame | Custom | Houses shafts, gears, and burrs |
| 1 | Inner coffee burr | Reverse-engineered (GrabCAD) | Specialized geometry, not available from class resources |
| 1 | Outer coffee burr | Reverse-engineered (GrabCAD) | Specialized geometry, not available from class resources |

## Skills Demonstrated

- Component sourcing and design-around-catalog-parts workflow
- Mechanism design (miter gear coupling, shaft-burr motion transfer)
- Motion-verified assembly (joints, interference checking, gravity/support constraints)
- Working from and honestly attributing a reverse-engineered reference component
- Iterative sketch-to-CAD refinement driven by real supplier constraints
