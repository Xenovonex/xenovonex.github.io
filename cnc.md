---
layout: default
title: CNC
---

[Back to Bachelor projects](./bachelor.md)
# The Engraving CNC-machine
### Date of project: 26 September 2016
<img src="/assets/img/CNC-machine_geheel_eind.png" alt="cnc-machine" width="400"/>
A SolidWorks model of the CNC-machine.

## Goal
Design and build a CNC-machine that can engrave a triangle in a sheet of PMMA plastic.

## Team
J. van der Blonk,
J. Linssen,
J. van der Sluis,
J. van der Vlugt,
S. Bonhof, 
R. Dirks

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
* Each of the three stepper motors will be used to control a single axis movement of the engraving drill.
* The X and Y axes will be linked to the motors using a belt transmission.
* The Z axis (of the drill) will be controlled using a trapezium screw transmission.
* Movement in the X-axis is done by actuating part of the frame: a sheet metal plate supported by two rods gliding on linear ball bearings, and connected to the motor with a belt transmission. On this sheet metal plate, the PMMA sheet will be placed for engraving.  
* Movement in the Y-axis and Z-axis will be controlled by actuating the drill. The drill is built into a sheet metal frame with a linear trapezium screw ball bearing connected to a trapezium thread which is actuated by the stepper motor to move the Z-axis. The drill frame is connected to two rods with linear ball bearings and connected to the stepper motor with a belt transmission to move the Y-axis. 

### Arduino
* The Arduino is programmed in C using the AccelStepper library to control the stepper motors to engrave the triangle according to the criteria.

## Results
A SolidWorks model of the CNC-machine is designed to perform FEM analysis on in COMSOL and for laserprinting of the sheet metal. Based on the FEM analysis, the frame will have a maximum deflection of 6nm, which is an acceptable value for the purpose of engraving a triangle in PMMA. 

<img src="/assets/img/CNC-machine_comsol.png" alt="cnc-comsol" width="400"/>

Below is a video of the CNC-machine engraving a triangle in PMMA. The engraving speed is 20 seconds for the whole triangle.
<iframe width="560" height="315" src="https://www.youtube.com/embed/4YJb8-Kvrg8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Skills
* Teamwork
* Mechatronics
* Mechanical Design
* SolidWorks
* FEM analysis
* Arduino
* Programming
