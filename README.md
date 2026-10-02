# DIY Mini Vacuum Cleaner Robot

This repository contains the full open-source design, wiring layouts, and control firmware for building a compact, autonomous desk vacuum robot.

## Project Overview
The robot uses a differential drive system (two independent wheels and a passive caster) to navigate surfaces. A high-RPM DC motor acts as an impeller fan to pull dust and debris into an integrated, filter-backed storage compartment. It uses an ultrasonic sensor to actively scan for and dodge obstacles.

## Bill of Materials (BOM)

### Mechanical & Chassis
* 3D Printed Chassis (Files located in hardware/3d-models/)
* 1x Passive Caster Wheel
* 2x Drive Wheels (Rubber tread preferred)
* 1x Fine Mesh Filter Material (or cut mesh from a surgical mask)

### Electronics & Power
* Microcontroller: Arduino Nano or ESP32 Development Board
* Motor Driver: L298N Mini or TB6612FNG Dual H-Bridge
* Drive Motors: 2x 6V N20 Micro Gear Motors (100–200 RPM)
* Vacuum Motor: 1x High-Speed Coreless DC Motor (with 3D printed impeller fan)
* Distance Sensor: 1x HC-SR04 Ultrasonic Sensor
* Power Source: 1x 18650 Li-ion Battery with a 5V boost converter step-up board
* Switch: 1x SPST Rocker Toggle Switch

## Assembly and Setup
1. 3D print the structural parts found in the `hardware/3d-models/` folder.
2. Wire the components according to the schematic diagram in `hardware/electronics/`.
3. Open the `firmware/` directory in your IDE (VS Code with PlatformIO or the Arduino IDE).
4. Flash the `main.cpp` code to your microcontroller.
