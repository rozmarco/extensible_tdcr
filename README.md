# Extensible Tendon-Driven Continuum Robot
This project includes the design files and link to assembly instructions for a tendon-driven continuum robot with an extensible degree of freedom.

The assembly instructions can be found here: https://docs.google.com/document/d/1z8M8oU-02HvgHBQCzrGDHriGV1tVsbQjVGHuQ0tKlOw/edit?usp=sharing.

## Design Overview

The full robot system consists of the following main components:

- **(A) Entire system** – The fully assembled robot including both segments and the control electronics.  
- **(B) Control components** – Actuators, motor drivers, microcontroller (e.g., OpenCM), and power supply.  
- **(C) Extensible or distal segment** – The upper segment capable of both spatial bending (3 tendons) and active extension.  
- **(D) Base or proximal segment** – The lower segment with 5 tendons enabling full spatial bending.  
- **(E) Pulley and manipulator support platform** – Holds and routes tendons near the distal end-effector and organizes tension distribution.  
- **(F) Motor support platform** – Houses the DYNAMIXEL actuators responsible for driving the tendons.  
- **(G) Driven pulley support platform** – Guides tendons as they pass from motors to the backbone, helping maintain consistent routing.  
- **(H) Driver pulley motor and belt** – The mechanism that enables extension of the distal segment by driving a belt-pulley setup.
- 
![TDCR Full System](docs/images/system_overview.jpg)


## Demo

The demonstration is the TDCR navigating two pipe-based task spaces arranged in a planar and three-dimensional configurations. Based on the location and stationary nature of the robot, the extensible degree of freedom is necessary to successfully enter and inspect the pipe.

[![TDCR Demo](https://img.youtube.com/vi/u-8E7-xkPwE/0.jpg)](https://youtu.be/u-8E7-xkPwE)  
▶️ [Watch the demo](https://youtu.be/u-8E7-xkPwE)
