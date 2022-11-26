---
layout: default
title: CNC
---

[Back to Bachelor projects](./bachelor.md)
# The Engraving CNC-machine
### Date of project: 26 September 2016
<img src="/assets/img/CNC-machine_geheel_eind.png" alt="cnc-machine" width="300"/>

## Goal
Design and build a CNC-machine that can engrave a triangle in a sheet of PMMA plastic.

## Team
J. van der Blonk,
J. Linssen,
J. van der Sluis,
J. van der Vlugt,
S. Bonhof, 
R. Dirks,

## Process
Design the CNC-machine according to the following criteria:
* The machine must engrave a triangle (coordinates: \[150,20\]\[150,120\]\[50,120\]mm) on a 2mm thick sheet of A5 PMMA, depth of triangle is not specified. 
* It must take no longer than 5 minutes to set-up the machine before engraving starts.
* The engraving drill must move from a rest-position outside the 'workfield' to the provided coordinates and must return to the rest-position after without making contact with the 'workfield' other than to engrave the triangle.
* The CNC-machine must be actuated using 3 stepper motors.
* An Arduino must be used to perform computations and control the motors.
* The CNC-machine must be as fast and accurate as possible.
* No parts can be used from toy or game toolsets and no wooden parts.

To design the CNC-machine, the following design choices are made based on robustness, feasibility to assemble, and simplicity:
### Frame
* The frame will be made out of steel to prevent major deflections during engraving. To verify the sturdiness, a Finite Element Method (FEM) analysis will be done on the frame.
* The main components of the frame will be beams, bent sheet metal, rods and trapezium thread.
* Different components will mostly be joined using rivets.

### Axes
* Bearings will be 3D-printed in PLA, or rollerbearings are used.
* Each of the three stepper motors will be used to control a single axis movement of the engraving drill.
* The X and Y axes will be linked to the motors using a belt transmission.
* The Z axis (of the drill) will be controlled using a trapezium screw transmission.
* moving X-axis standard, Y and Z axis - drill will be moved

## Results

<iframe width="560" height="315" src="https://www.youtube.com/embed/4YJb8-Kvrg8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
