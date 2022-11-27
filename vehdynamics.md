---
layout: default
title: Vehicle Dynamics
---

[Back to Master projects](./master.md)
# Preventing Vehicle Rollover
### Date of Project: 7 April 2019
<img src="/assets/img/Anti_rollbar_simulink.PNG" alt="vehdyn" width="300"/>\
The Simulink model of a passive anti-rollover bar.

## Goal
Research the rollover of a high center-of-gravity grocery delivery truck using MATLAB and Simulink to simulate the rollover dynamics for different vehicle properties. Find a solution to prevent rollover.

## Team
S. Bonhof, S. Molenaar, J. van der Sluis, J. Wijkhuizen, R. Dirks

## Process
* Rollover dynamics is researched for three different properties:
  - Different vehicle masses.
  - Different vehicle Centers of Gravity (CoG).
  - Three different anti-rollbars: No anti-rollbar, passive anti-rollbar, active anti-rollbar
* Rollover dynamics will be researched by comparing simulations of a vehicle performing a fish-hook manoeuvre for the different properties.
* The vehicle model includes lateral and longitudinal dynamics, roll and yaw dynamics, wheel and tire dynamics, wheel and side slip and lateral and longitudinal load transfer, because these factors are relevant to evaluate regarding roll behaviour of the vehicle. A planar vehicle model is used with 8 Degrees of Freedom (DoF), including all four wheels rotational degrees of freedom (4 DoF), the longitudinal and lateral displacement (2 DoF) and the yaw and roll angles (2 DoF). The [Dugoff](https://www.jstor.org/stable/44644491) tire model is used to model tire-ground dynamics.
* The effect on roll dynamics of different masses and CoGs is researched using no anti-rollbar. 
* The passive anti-rollbar is modeled by adding a spring with a certain stiffness in between the two front wheel suspensions. The higher the roll angle, the higher the spring torque in the opposite direction of the roll angle, reducing the roll movement.
* The active anti-rollbar is modeled by adding a torque to the model that counters the rollover movement. This torque is controlled by a PD-controller, making it an active component countering rollover.

## Results
<img src="/assets/img/swa_LateralSpeed.png" alt="res_fishhook" width="300"/>

<img src="/assets/img/Remaining_Roll_CoG_and_Masses.png" alt="res_mass_cog" width="300"/>

<img src="/assets/img/Roll_vs_time_antirollbars.png" alt="res_anti" width="300"/>
