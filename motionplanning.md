---
layout: default
title: Motion Planning
---

[Back to Master projects](./master.md)
# MPC Controller for Collision Avoidance
### Date of Project: 30 March 2020
<img src="/assets/img/Workspace.jpg" alt="workspace" width="300"/>
Workspace of the autonomous vehicle (green), with a road (black), a pedestrian obstacle (yellow), a vehicle obstacle (red), a center line (dashed), and two reference lines (continuous). The first reference line avoids objects, the second does not.

## Goal
Simulate a navigation task within a traffic environment that is locally planned by a Model Predictive Control module.

## Team
H. Li, Z. Wan, P. Gregoire, R. Dirks

## Process
* A bicycle model is chosen to model the Automonous Vehicle in MATLAB
* The Autonomous Vehicle is modeled to have a 360 degrees view of the traffic scene
* A Workspace is designed of the traffic scene with a moving pedestrian obstacle and a static vehicle obstacle (see Workspace image above)
* Based on the bicycle model and the Workspace, a configuration space is created in which all possible states of the Autonomous Vehicle are mapped, given its kinematic constraints and obstacle constraints.
* The Autonomous Vehicle is simulated in two different scenarios with different reference lines that it must follow as closely as possible while avoiding any collisions with the obstacles. The first reference line is designed so the Autonomous Vehicle will avoid the obstacles if it follows this line perfectly. The second reference line is designed to for the Autonomous Vehicle to keep following the right lane. If the controller works well, the obstacles should be avoided, despite the reference line going throuh the obstacles.
* The Autonomous Vehicle must use a Model Predictive Controller to follow the reference lines and avoid obstacles.
* 

### Video: Simulation of a car following a road while avoiding objects using Model Predictive Control
<video width="640" height="480" controls>
  <source src="./assets/img/RMPC_Group19_MPC_Car_new.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

