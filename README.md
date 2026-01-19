# Extensible Tendon-Driven Continuum Robot (TDCR)
This project provides open-source mechanical design files and assembly documentation for a two-segment tendon-driven continuum robot (TDCR) with an extensible distal segment. Axial extension is achieved using a concentric tube–rod backbone with passive magnetic spacer disks, enabling additional dexterity for navigation in constrained environments.


![Manipulator Configurations](docs/images/overlay.jpg)

Detailed mechanical assembly instructions, including part lists and tooling notes, are provided here:  
https://docs.google.com/document/d/1z8M8oU-02HvgHBQCzrGDHriGV1tVsbQjVGHuQ0tKlOw/edit?usp=sharing

## Design Philosophy

The system is designed to keep low-level mechanics simple while enabling richer high-level behaviors. Passive magnetic spacer disks are used to maintain approximately uniform disk spacing during axial extension, avoiding active spacing mechanisms and additional actuators. Tendon routing is symmetric to reduce control complexity, and modular rail-mounted actuation enables rapid reconfiguration and iteration.


## Design Overview

The full robot system is modular and organized around a rail-mounted actuation unit coupled to a two-segment continuum manipulator:

- **(A) Entire system** – The fully assembled robot including both segments and the control electronics.  
- **(B) Control components** – Motor driver and controller for teleoperation of TDCR segments.  
- **(C) Extensible or distal segment** – The upper segment capable of both spatial bending (3 tendons) and active extension.  
- **(D) Base or proximal segment** – The lower segment with 5 tendons enabling full spatial bending.  
- **(E) Pulley and manipulator support platform** – Holds base of the manipulator and pulleys for routing tendons from end-effector to motors.  
- **(F) Motor support platform** – Mounts the DYNAMIXEL actuators used for driving the tendons onto the rail.  
- **(G) Driven pulley support platform** – Attaches the driven belt pulley onto the rail.  
- **(H) Driver pulley motor and belt** – The system's belt, along with the attachment fixture used to connect the backbone rod to the belt, and the platform that mounts the driver motor onto the rail.

![TDCR Full System](docs/images/system_overview.jpg)


## Demo

The demonstration is the TDCR navigating two pipe-based task spaces arranged in a planar and three-dimensional configurations. Based on the stationary mounting of the robot, the extensible degree of freedom is required to advance the end-effector through the task space without repositioning the base, enabling inspection of both planar and spatial pipe geometries.


[![TDCR Demo](https://img.youtube.com/vi/u-8E7-xkPwE/0.jpg)](https://youtu.be/u-8E7-xkPwE)  
▶️ [Watch the demo](https://youtu.be/u-8E7-xkPwE)
