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

Blocks of different colors will be placed on a conveyer belt. A distance sensor will measure the height of the block. If the block is too high it will be thrown away by an actuator. Otherwise (so when the block is of the standard height), the block will continue over the belt. This is similar to separating metal from the other waste with a magnet in a real garbage sorting center. After this the block will roll on another belt. Here the color of the block will be decided with a color sensor. Based on this measurement the block will later be placed in a different box with an actuator. This is comparable to separating different kinds of waste.

## Result
<iframe width="560" height="315" src="https://www.youtube.com/embed/M2jEXQdBnBI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Skils
