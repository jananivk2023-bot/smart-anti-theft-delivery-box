# Smart Anti-Theft Delivery Box

An automated, tamper-resistant parcel containment solution designed to secure doorstep deliveries through real-time weight verification and IoT-enabled status monitoring.

## Overview

Unattended doorstep parcel deliveries are vulnerable to theft and false delivery claims. This project proposes a secure physical enclosure integrated with weight-sensing instrumentation and microcontroller-based automation. The system detects package placement, secures the enclosure after delivery, and identifies potential tampering or unauthorized parcel removal.

## Key Features

- **Precision Weight Verification:** Uses a strain-gauge load cell and HX711 24-bit ADC to detect package placement and measure parcel weight.
- **Automated Enclosure Locking:** Controls an electronic locking mechanism to secure the enclosure after a parcel is detected.
- **Tamper & Theft Detection:** Monitors weight readings and identifies sudden weight changes that may indicate unauthorized parcel removal.
- **Physical Prototype Design:** Focuses on enclosure stability, sensor protection, load cell mounting, and accurate weight measurement.
- **Embedded Control Architecture:** Implements state-machine logic for delivery detection, secure storage, and parcel collection.

## Tech Stack & Hardware Components

- **Microcontroller:** ESP32 (Dual-Core Wi-Fi Microcontroller)
- **Firmware Development:** Embedded C/C++ (Arduino Framework)
- **Sensors & Instrumentation:** Strain-Gauge Bar Load Cell, HX711 24-bit ADC Amplifier
- **Actuation & Access:** 12V Solenoid Lock / Relay Module
- **Mechanical Design:** Enclosure Assembly, Load Cell Mounting Plates, and Weighing Platform

## Circuit & Pin Configuration

| Hardware Unit | ESP32 Pin | Interface / Role |
|---------------|-----------|------------------|
| HX711 DT (Data) | GPIO 21 | Digital Serial Data |
| HX711 SCK (Clock) | GPIO 22 | Digital Serial Clock |
| Relay Module (Lock Actuator) | GPIO 26 | Digital Output (Active High) |
| Power Supply | 12V DC Adapter (Step-down to 5V/3.3V) | System Power |

## Documentation Status

CAD assembly files, calibration routines, circuit diagrams, and firmware source files will be uploaded upon completion of the final documentation.
