---
layout: default
title: Garbit
---

[Back to Bachelor projects](./bachelor.md)
# Garbit: The Brick Sorting Machine
### Date of project: 7 April 2017
<img src="/assets/img/garbit.PNG" alt="garbit_project" width="300"/>

## Goal
Build and design a sorting machine prototype for garbage separation. Instead of garbage, separate various colored blocks of different heights.

## Team
S. Rademaker,
J. van der Sluis,
J. van der Vlugt,
R. Dirks

## Process
Design the sorting machine according to the following criteria:
* Consists of a frame that contains coveyor belts, block storage, sensors, and motors
* Maintains a constant conveyor belt speed using a DC-motor and velocity sensor
* Uses color sensors to differentiate between colored blocks
* Uses ultrasonic sensors to differentiate between different sized blocks
* Uses servo-motors and ultrasonic sensors to detect, sort, and drop blocks in the assigned areas
* Uses Arduinos to process sensor data, make decisions, and control the motors
* Design a Finite-State Machine (FSM) schematic for the solution

A sorting machine frame is built using K'nex and lasercut material. The frame contains a drop off point for the blocks to enter the sorting machine and five storage areas. Four storages areas for the different colors, and the fifth for large-sized blocks. Two conveyour belts are built using fabric, positioned perpendicular to each other.

Each conveyor belt can be actuated using a DC-motor. The velocity is measured with a self-made tachometer using a laser, laser sensor, and a perforated disk.
The conveyor belts are kept at a constant speed using a PID-controller.

Blocks of different colors (Red, Green, Blue, Yellow) and different sizes (one block or two stacked blocks) will be dropped on a conveyer belt. An ultrasonic sensor will measure the height of the block and a color sensor will measure the color. Depending on the color, small sized blocks will be sorted in one of four storage areas. Ultrasonic sensors will detect if a block is at the right position. The servo-motors will push it in the right storage area. If a block is large-sized, it will end up in the fifth 'remaining' block storage area at the end of the conveyor belt. This process is comparable to separating different kinds of waste. 

A Finite-State Machine (FSM) schematic is designed to capture every state the sorting machine can be in and select the appropriate actions. This is programmed on two connected Arduinos that also receive the sensor data and control the motors.

## Result

The video below shows the final result of this project. It shows how the blocks get dropped onto the conveyor belt, how the conveyor belts are actuated at a constant speed, and how the different blocks are sorted.
<iframe width="560" height="315" src="https://www.youtube.com/embed/M2jEXQdBnBI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Skils
* Teamwork
* Mechatronics
* Arduino
* C programming
* Finite-State Machine design
* Sensors and motors
