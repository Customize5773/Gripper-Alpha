# gripper-control

## Overview

`gripper-control` is an embedded control project focused on **robot gripper/jaws selection** and **resistive object detection**.
The system is designed to detect object presence and resistance during grasping, then use that information to guide gripper behavior and jaw selection logic.

The primary goal is to provide a simple, extensible control framework for experimental and educational robotic gripper systems.

---

## Core Concepts

* **Gripper / Jaws Selection**
  Logic to select or configure gripper jaws based on object interaction characteristics.

* **Resistive Object Detection**
  Detection of object presence and resistance using electrical or mechanical feedback (e.g. motor current, force-sensitive elements, or resistive sensors).

* **Embedded Control**
  Designed for microcontroller-based systems (e.g. Arduino, ESP32), emphasizing clarity and reliability over complexity.

---

## System Scope

This project focuses on:

* Low-level gripper control logic
* Sensor-based detection of object resistance
* Deterministic, embedded-friendly implementation

Out of scope (for now):

* High-level AI or vision systems
* Full robotic arm kinematics
* ROS integration

---

## Repository Structure

```
gripper-control/
├── README.md
├── docs/        # System overview, wiring, and BOM
├── firmware/    # Embedded control code
├── hardware/    # Schematics and mechanical design
└── tools/       # Calibration and helper utilities
```

---

## Hardware Assumptions

The system is designed to be hardware-agnostic but typically involves:

* A robotic gripper or jaw mechanism
* Actuator (servo, DC motor, or similar)
* Resistive or force-related sensing element
* Microcontroller-based control board

Exact components are documented in `/docs`.

---

## Project Status

* Development stage: **Concept / Early Implementation**
* Interfaces and control logic may change
* Stability is not yet guaranteed

---

## License
