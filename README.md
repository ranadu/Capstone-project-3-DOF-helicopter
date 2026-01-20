# 3-DOF Helicopter Control and Trajectory Tracking

Closed-loop PID control of a laboratory 3-DOF helicopter achieving stable multi-axis trajectory tracking under actuator constraints.

---

## Overview

This capstone project models, designs, and validates a complete closed-loop control system for a **3-Degree-of-Freedom (3-DOF) laboratory helicopter** using **MATLAB and Simulink**. Independent PID controllers were developed for the **travel**, **elevation**, and **pitch** axes to achieve stable trajectory tracking while respecting realistic actuator limits.

The project emphasizes **system-level control architecture**, **realistic constraints**, and **time-domain validation**, closely reflecting how flight control systems are developed and tested in aerospace applications.

---

## System Description

The helicopter dynamics are separated into three primary rotational axes:

- **Travel (Yaw):** Horizontal rotation and heading control  
- **Elevation:** Vertical positioning and lift control  
- **Pitch:** Attitude stabilization and transient response shaping  

Each axis is controlled using an independent closed-loop PID controller. The control outputs are combined and routed through a shared plant model that represents the physical helicopter and actuator behavior.

---

## Control Architecture

- Independent PID loops for travel, elevation, and pitch
- Closed-loop feedback using measured states
- Actuator saturation limits applied to control voltages
- Central junction block for plant input coordination
- Modular Simulink subsystems for clarity and scalability

This structure mirrors real-world aerospace control systems where multiple controllers interact with a common plant.

---

## Engineering Focus

- Multi-axis PID controller design and tuning  
- Trajectory tracking and reference following  
- Closed-loop stability and transient response analysis  
- Actuator saturation and safety constraints  
- System integration and signal routing in Simulink  

---

## Math & Control Theory

- Linear system modeling  
- PID control theory  
- Time-domain response analysis  
- Stability and steady-state error evaluation  

---

## Validation

Controller performance was validated through simulation by applying step and trajectory inputs and observing:

- Reference vs measured response tracking  
- Stable convergence without sustained oscillations  
- Bounded control effort within actuator limits  

The results demonstrate stable closed-loop behavior and effective trajectory tracking across all three axes.

---

## Tools Used

- MATLAB  
- Simulink  
- Control Systems Toolbox  

---
