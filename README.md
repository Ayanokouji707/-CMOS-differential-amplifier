# Differential Amplifier – Simulation and Layout

## Overview

This project focuses on the **design, simulation, and physical layout** of a **differential amplifier** using:

- **NGSpice** for circuit simulation
- **Microwind** for IC layout design

It demonstrates core analog design principles such as differential signal amplification, biasing, and layout techniques using 90nm CMOS technology.

## Project Files

- `netlist (2).cir`: NGSpice-compatible netlist describing the differential amplifier circuit.
- `Differential Amplifier (2).MSK`: Microwind layout file showing the mask design for the amplifier.

## Tools Used

- **NGSpice** (Open-source SPICE simulator)  
- **Microwind** (VLSI design and layout tool)  
- **Technology Node**: 90nm CMOS

## How to Run

### 1. Circuit Simulation (NGSpice)
- Open a terminal and run:
  ```bash
  ngspice "netlist (2).cir"
  ```
- Observe waveforms like input differential pair behavior, output swing, and gain using NGSpice’s plotting tools or output file.

### 2. Layout Design (Microwind)
- Open `Differential Amplifier (2).MSK` in **Microwind 3.1**.
- Use **DRC** (Design Rule Check) to ensure layout compliance.
- Optionally perform electrical simulation (if supported) or export GDS for fabrication.

## Design Highlights

- **Differential Input**: Two NMOS input transistors for handling VIN+ and VIN−.
- **Current Mirror**: Used for active load or biasing.
- **Gain Stage**: Tuned for sufficient voltage gain.
- **Matching Layout**: Transistor symmetry and common-centroid layout followed (if applicable).

## Applications

- Analog front-end circuits
- Operational amplifiers
- Signal conditioning stages

## Author

**[Saurabh Kamble]**  
[Indian Institute of Infromation Technology, nagpur]  

