---
layout: project
title: "Nutcracker Design Project: Statics & Mechanics"
description: Designed a functional nutcracker to meet specified force and usability constraints using statics, moment equilibrium, and beam deflection analysis. The project included force modeling, geometric design, and cross-section optimization.
---

## Overview

This project focused on designing a usable nutcracker that could generate the required cracking force while satisfying geometric, material, and deflection constraints. The design used static equilibrium, moment analysis, and beam deflection calculations to determine the required handle geometry and material selection.

| Parameter | Value |
|---|---:|
| Required force to crack nut | 2220 N |
| Applied user force | 500 N |
| Nut radius | 1 cm |
| Maximum allowed deflection | ≤ 2% of beam length |
| Selected material | Structural steel |
| Elastic modulus | 200 GPa |

---

## Part 1: Force and Geometry Analysis
The first stage of the design used moment equilibrium about the nutcracker pin. This point was selected because it allowed the applied handle force and the nut reaction force to be related through their moment arms.

The distance from the pin to the nut was defined as \(x_1\), while the distance from the pin to the applied user force was defined as \(x_1 + x_2\). Using the required nut-cracking force and the maximum applied user force. Taking the moment about the pin would allow me to find the two values of x_1 and x_2 such that it would balance the forces sufficently. The handle length was selected so that the applied force could generate enough moment to crack the nut. With these lengths found I used the to create the diagram below.

This geometry produced a usable design because the user only needed to apply 500 N at each handle while maintaining a 1 cm nut gap.

![Nutcracker geometry diagram]({{ "/assets/images/nutcracker_diagram_1.png" | relative_url }}){: .project-image }

---

## Part 2: Beam Deflection and Material Selection

The second stage of the design analyzed the elastic deflection of the nutcracker handles. The objective was to select a beam cross-section and material that would keep the vertical deflection below 2% of the beam length while remaining as mass-efficient as possible.

The design requirements were:

1. Determine the location of maximum elastic deflection in the handles.
2. Select a beam cross-section and material that limits vertical deflection to less than 2% of the handle length.
3. Present the final nutcracker geometry and beam model.

### Deflection Analysis

A free-body diagram was created using three primary forces:

1. The applied user force of 500 N.
2. The reaction force from the nut.
3. The reaction force at the pin.

Using the beam deflection appendix from *Statics and Mechanics of Materials* by Beer, the point of maximum deflection was modeled as:

<div style="text-align: center; margin: 1rem 0; font-size: 16px;">
  x<sub>m</sub> = √((L<sup>2</sup> − a<sup>2</sup>) / 3)
</div>

Using the known handle length and \(a = 2 \text{ cm}\), the maximum deflection location was calculated as:
<div style="text-align: center; margin: 1rem 0; font-size: 16px;">
  x<sub>m</sub> = 3.214 cm
</div>

The maximum allowable deflection was limited to:

<div style="text-align: center; margin: 1rem 0; font-size: 16px;">
  Y<sub>max</sub> = 0.02L
</div>

The deflection equation was then used to solve for the required relationship between the elastic modulus \(E\) and the area moment of inertia \(I\). Since the applied force, beam length, and geometry were already defined, the material and cross-section selection depended primarily on \(E\) and \(I\).

Structural steel was selected because of its high elastic modulus, stiffness, and ability to resist deformation under the applied loading conditions. Using E = 200 GPa, the selected beam shape was a W18x106 section.

![Final nutcracker beam model]({{ "/assets/images/nutcracker_diagram_2.png" | relative_url }}){: .project-image }

---

## Technologies and Concepts Used

- Static equilibrium
- Moment analysis
- Beam deflection modeling
- Material selection
- Cross-section optimization
- Structural steel design
- Engineering design constraints

---

## Key Result

The final design satisfied the required nut-cracking force while keeping the handle deflection below the allowable 2% limit. The project demonstrated how statics and mechanics of materials can be used to convert force requirements into a functional mechanical design.
