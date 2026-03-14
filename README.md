# Smart Prosthetic Limb with Haptic Feedback

## Overview
This project aims to develop a cost-effective, multi-sensor prosthetic limb, integrating both myoelectric control and haptic (tactile) feedback. By bridging mechanical control with sensory experience, the project seeks to enhance user comfort, confidence, and interaction with their environment. The prototype serves as both a functional assistive device and an accessible educational resource.

## Circuit Diagram
Below is the circuit architecture showing the integration of the Arduino Uno, flex sensors, and servo motors.

![Circuit Diagram](https://github.com/ritesh190605/smart-prosthetic-limb/blob/ac66cbc456dcf106d1d14c1136eb9886e71c8dae/circuit_diagram.png)

## System Workflow
The system operates through a closed-loop architecture designed for minimal latency (below 100ms):

* **Sensing (EMG & Flex Sensing Module):** Captures user muscle activity or finger movement intent. Flex sensors detect the bending of fingers, creating a variable voltage read by the Arduino.
* **Processing:** An Arduino Uno R3 acts as the central controller, reading input signals, mapping the filtered sensor values, and executing commands. 
* **Actuation (Motor Control Module):** Five servo motors (one per finger) receive PWM signals from the Arduino to mimic natural, proportional finger movements.
* **Feedback (Grip & Haptic Modules):** Force Sensitive Resistors (FSRs) measure the force applied by each finger to prevent excessive grip. These grip values are converted into vibration signals via coin motors placed in the limb socket to directly stimulate the user's residual limb, successfully simulating the sensation of touch.

## Hardware Requirements
* Arduino Uno R3
* MyoWare EMG Sensor
* Flex Sensors
* Servo Motors
* Force Sensitive Resistors (FSRs) & Vibration Coin Motors
* Li-ion Battery
* 3D-Printed Socket/Frame
* Breadboard, Resistors, and Jumper Wires

## Software Requirements
* Embedded C/C++ (Arduino IDE)
* Tinkercad / Fusion 360 (for simulation and mechanical design)

## Future Enhancements
Future iterations of this project plan to implement:
* **AI-Based Adaptive Grasp:** Utilizing machine learning to predict user intent and adapt grip strength based on an object's shape and fragility.
* **Wireless Connectivity:** Bluetooth modules for real-time data transfer, remote diagnostics, and firmware updates.
* **Advanced Sensing:** Upgrading sensors to detect texture, temperature, and highly detailed pressure mapping.
