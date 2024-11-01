# actuator-module PCB

This repository contains the hardware design and documentation for a custom PCB developed for the actuation of solenoid and servo valves in a biliquid rocket engine. Created by Fredrik Spalder through Propulse NTNU, this project provides the necessary hardware for controlled actuation in a high-stress, high-performance rocket propulsion environment. The design is the second iteration of a previous version.


## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Hardware Specifications](#hardware-specifications)
- [Schematics and PCB Layout](#schematics-and-pcb-layout)
- [Installation and Setup](#installation-and-setup)

## Overview

The purpose of this project is to develop a reliable, high-performance PCB for controlling solenoid and servo valves in a biliquid rocket engine. The board design focuses exclusively on hardware implementation, ensuring precision and durability for integration within the propulsion system developed by Propulse NTNU.

## Features

- Actuation control for both solenoid and servo valves
- Optimized layout for minimal noise and efficient power delivery
- Compatible with high-current solenoid actuation needs
- Designed for robustness in a high-vibration environment
- PCB dimensions and layout suitable for integration with the Engine Controller Unit (ECU)

## Hardware Specifications

- **Valve Compatibility:** Supports solenoid and servo valves
- **Power Supply:** Input of 12V & 24V
- **Power Output:** Delivers 12V to the servos and 24V to the solenoids
- **Solenoid Actuation:** Uses a 24V switch with actuation signals from the ECU to deliver power to the solenoids
- **Servo Actuation:** Uses PWM and 12V from the ECU to deliver power to the servos
- **Servo Position:** Provides ECU with servo position measurement based on magnetic encoding
- **Current draw:** Provides the ECU with data on the current drawn from each servo and solenoid separately
- **Protection:** Overcurrent and thermal protection features
- **PCB Layers:** The PCB contains power & ground planes
- **Connector Types:** WR-PHD Pin headers for connecting to the ECU. Servo and solenoid cabling is soldered directly on to the pcb

## Schematics and PCB Layout

Detailed schematics and PCB layout files are available in the `/hardware` directory. This directory includes:

- Schematic diagrams in PDF format
- PCB layout in Gerber files
- Bill of Materials (BOM) listing all components with part numbers and specifications

> **Note:** Files are designed for fabrication and can be sent to a PCB manufacturer directly.

![image](https://github.com/spalder/Actuator-PCB/blob/main/images/IMG_6322.PNG)
![Actuator Module Schematic.pdf](https://github.com/spalder/Actuator-PCB/blob/main/hardware/Actuator%20Module%20Schematic.pdf)

## Installation and Setup

To prepare the PCB for use:

1. **Fabrication:** Use provided Gerber files to manufacture the PCB.
   ![Actuator PCB 6306.jpg](https://github.com/spalder/Actuator-PCB/blob/main/images/Actuator%20PCB%206396.jpg)
2. **Assembly:** Solder components according to the BOM.
   ![IMG 6400.jpg](https://github.com/spalder/Actuator-PCB/blob/main/images/IMG%206400.jpg)
3. **Testing:** Follow testing procedures to verify board integrity before installation.
4. **Integration:** Connect the board to the ECU, ensuring proper connections for the solenoid and servo valves.
   ![IMG_6578.jpeg](https://github.com/spalder/Actuator-PCB/blob/main/images/IMG_6578.jpeg)

### Prerequisites

- Soldering tools and materials for assembly
- Power supply suitable for initial testing
- Multimeter and oscilloscope for verification
