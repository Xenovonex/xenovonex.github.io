[Back to Bachelor projects](./bachelor.md)
# Rover: The Autonomous Car
### Date of project: 1 June 2018
<img src="/assets/img/rover_av.PNG" alt="roverav" width="300"/>

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
* **Design a PID controller for the thrust and steering wheel motors**
  - **Use the Rover's position data over time with respect to the reference position as input to the PID controller**
  - **Output the new steering angle and thust intensity**
  - **Test and adjust the controller to acquire the correct PID constant values**
* Combine the autonomous vehicle pipeline modules on a Raspberry Pi
  - Create publishers and subscribers in Robot Operating System (ROS) for communcation between Sensor and Controller modules 
  - Connect the controller output to the PixHawk microcontroller
* **Simulate and visualize the Rover**
  - **Simulate the camera sensor capturing te vehicle wheels in MATLAB** 
  - **Simulate the Rover and the Vehicle in MATLAB using the bicycle model**
  - **Simulate the PID controller module to perform the goal task in MATLAB**

* **Test the Rover in a real world situation**

**Bolded:** My main contributions to the project

## Results
The simulation of the Rover shows it succeeds to recognize the wheels of the real vehicle and to stably follow the the real vehicle provided it uses the correct PID constants.

Below: Image of the Rover's camera sensor detecting the real vehicle's two front wheels. Blue squares: Area between wheels. Green lines: Reference positions of wheels to center the Rover underneath vehicle. Red lines: Actual position of the wheels. \
<img src="/assets/img/wheel_detection.PNG" alt="roverav" width="300"/>

The Rover succeeded to follow a real vehicle at 10-20 km/h on a trajectory with both straight parts and curves.

### Video of the Rover driving underneath a van
<video width="640" height="480" controls>
  <source src="./assets/img/rover_demonstration_LQ.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


## Skills
* Teamwork and communication
* Time management
* MATLAB
* Python
* Robot Operating System (ROS)
* OpenCV
* Control Theory
* Dynamic Simulations
* Product design and testing
