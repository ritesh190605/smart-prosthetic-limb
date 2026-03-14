# Smart Prosthetic Limb with Haptic Feedback

**Author:** Pradeep Yadav

## Overview
[cite_start]This project aims to develop a cost-effective, multi-sensor prosthetic limb, integrating both myoelectric control and haptic (tactile) feedback[cite: 15]. [cite_start]By bridging mechanical control with sensory experience, the project seeks to enhance user comfort, confidence, and interaction with their environment[cite: 35]. [cite_start]The prototype serves as both a functional assistive device and an accessible educational resource[cite: 16].

## Circuit Diagram
Below is the circuit architecture showing the integration of the Arduino Uno, flex sensors, and servo motors.

![Circuit Diagram](Screenshot%202025-10-12%20at%2010.01.16%E2%80%AFPM.jpg)

## System Workflow
[cite_start]The system operates through a closed-loop architecture designed for minimal latency (below 100ms)[cite: 40]:

* [cite_start]**Sensing (EMG & Flex Sensing Module):** Captures user muscle activity or finger movement intent[cite: 163]. [cite_start]Flex sensors detect the bending of fingers, creating a variable voltage read by the Arduino[cite: 199, 200].
* [cite_start]**Processing:** An Arduino Uno R3 acts as the central controller, reading input signals, mapping the filtered sensor values, and executing commands[cite: 94, 95, 196]. 
* [cite_start]**Actuation (Motor Control Module):** Five servo motors (one per finger) receive PWM signals from the Arduino to mimic natural, proportional finger movements[cite: 96, 204, 205].
* [cite_start]**Feedback (Grip & Haptic Modules):** Force Sensitive Resistors (FSRs) measure the force applied by each finger to prevent excessive grip[cite: 167]. [cite_start]These grip values are converted into vibration signals via coin motors placed in the limb socket to directly stimulate the user's residual limb, successfully simulating the sensation of touch[cite: 47, 169, 170].

## Hardware Requirements
* [cite_start]Arduino Uno R3 [cite: 194]
* [cite_start]MyoWare EMG Sensor [cite: 194]
* [cite_start]Flex Sensors [cite: 194]
* [cite_start]Servo Motors [cite: 204]
* [cite_start]Force Sensitive Resistors (FSRs) & Vibration Coin Motors [cite: 97]
* [cite_start]Li-ion Battery [cite: 194]
* [cite_start]3D-Printed Socket/Frame [cite: 194]
* [cite_start]Breadboard, Resistors, and Jumper Wires [cite: 194]

## Software Requirements
* [cite_start]Embedded C/C++ (Arduino IDE) [cite: 210]
* [cite_start]Tinkercad / Fusion 360 (for simulation and mechanical design) [cite: 211]

## Future Enhancements
Future iterations of this project plan to implement:
* [cite_start]**AI-Based Adaptive Grasp:** Utilizing machine learning to predict user intent and adapt grip strength based on an object's shape and fragility[cite: 265, 266].
* [cite_start]**Wireless Connectivity:** Bluetooth modules for real-time data transfer, remote diagnostics, and firmware updates[cite: 267, 268].
* [cite_start]**Advanced Sensing:** Upgrading sensors to detect texture, temperature, and highly detailed pressure mapping[cite: 269].
