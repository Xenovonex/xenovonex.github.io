# Rover: The Autonomous Car
Date of project: 1 June 2018

## Goal
Design and program a Radio-Controlled toy car, called the Rover, to follow and drive underneath a real vehicle 
for the Netherlands Organisation for Applied Scientific Research (TNO).

## Team
* J. van der Blonk
* J. Linssen
* J. van der Sluis
* J. van der Vlugt
* R. Dirks

* J. Fransman (supervisor)
* J. Sijs (supervisor)

## Process
* Design and adjust the Rover according to the following criteria:
  - Fits underneath a real car
  - Contains a camera pointed forward
  - Contains a Raspberry Pi Computer
  - Contains a PixHawk microcontroller that controls the thrust and steering motors
  - Holds a battery to provide power to the vehicle
  - Adjustments can be 3D-printed
* Use camera sensor data to locate the Rover underneath the real car
  - Detect the real car's wheels using OpenCV
  - **Determine Rover's position based the wheels' locations with respect to the camera center**
* Design a PID controller for the thrust and steering wheel motors
  - **Use the Rover's position data over time with respect to the reference position as input to the PID controller**
  - **Output the new steering angle and thust intensity**
  - **Test and adjust the controller to acquire the correct PID constant values**
* Combine the Sensor and Controller modules and connect the controller output to the PixHawk microcontroller using a Raspberry PI with Robot Operating System (ROS). 
* **Simulate and visualize the Rover's camera and controller modules to perform the task in MATLAB**
* **Test the Rover in a real world situation**

**Bolded:** My main contributions to the project

## Results
The simulation of the Rover shows it succeeds to stably follow the car provided the correct PID constants.
The Rover succeeded to follow a real car at 10 km/h on a trajectory with both straight parts and curves.



## Skills
