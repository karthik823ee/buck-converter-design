# DC-DC Buck Converter Design and Implementation

## Overview
Design, simulation, and physical implementation of a DC-DC Buck (step-down) converter 
as part of a power electronics course project. The converter was tested at two duty 
cycles — 0.25 and 0.5 — stepping down a 30V DC input, with results validated on both 
MATLAB/Simulink and a physical hardware circuit.

## Team Project
Built as part of a power electronics course at NIT Calicut.

## Objectives
- Design a buck converter for a 30V DC input
- Simulate the circuit in MATLAB/Simulink and analyse output waveforms
- Build and test the physical circuit and compare with simulation results
- Study the effect of varying duty cycle (D = 0.25 and D = 0.5) on output voltage

## Tools & Technologies
- **Simulation:** MATLAB / Simulink
- **Hardware:** MOSFET switch, diode, inductor, capacitor, load resistor
- **Input Voltage:** 30V DC
- **Duty Cycles Tested:** D = 0.25 → ~7.5V output | D = 0.5 → ~15V output
- **Concepts:** Power Electronics, PWM, Voltage Conversion, Switching Circuits

## How It Works
A buck converter steps down DC voltage using a high-frequency switching MOSFET, 
a freewheeling diode, and an LC filter. The output voltage is governed by:

**V_out = D × V_in**

At D = 0.25: V_out ≈ 7.5V  
At D = 0.5: V_out ≈ 15V  

The Simulink model was built first to validate waveforms and transient response, 
followed by physical circuit construction and measurement to verify real-world behaviour.

## Results
| Duty Cycle (D) | Theoretical V_out | Measured V_out |
|---|---|---|
| 0.25 | 7.5V | *(from report)* |
| 0.50 | 15.0V | *(from report)* |

- Simulink waveforms showed expected voltage ripple and settling behaviour
- Physical circuit output matched theoretical values closely
- Switching waveforms captured and documented

## What I Learned
- End-to-end power electronics design: theory → simulation → hardware
- Importance of component selection (inductor, capacitor sizing) for ripple reduction
- Hands-on experience with MOSFET-based switching and PWM control

> 📁 Simulink model files, output waveform screenshots, circuit diagram, and full team 
> report with hardware photos available in this repository.[PE _report final.pdf](https://github.com/user-attachments/files/28211536/PE._report.final.pdf)
