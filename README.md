# DRV8313_simplefoc_PCB
A FOC driver board for controlling multiple BLDC motors using **SimpleFOC** and the **DRV8313** 3‑phase driver.

- Project: **FOC Motor Driver PCB**
- Driver IC: **Texas Instruments DRV8313**
- Firmware ecosystem: **SimpleFOC**

---

## Table of Contents
- [DRV8313_simplefoc_PCB](#drv8313_simplefoc_pcb)
  - [Overview](#overview)
  - [Features](#features)
  - [Repository Structure](#repository-structure)
  - [Hardware (PCB)](#hardware-pcb)
  - [Bill of Materials (BOM)](#bill-of-materials-bom)
  - [Installation and Setup](#installation-and-setup)

---

## Overview
**DRV8313_simplefoc_PCB** is a compact motor driver board intended for **Field Oriented Control (FOC)** of BLDC motors. The board is designed to be used with a microcontroller running **SimpleFOC**, and provides the power stage based on the **DRV8313**.

> Goal: make it easy to build multi-motor setups by repeating the same driver channel design and keeping wiring/bring-up straightforward.

---

## Features
- DRV8313-based **3-phase BLDC** driver stage
- Designed for **SimpleFOC compatibility**
- Multi-motor oriented layout (repeatable channels)
- Test points / headers for bring-up (PWM, enable, faults, power) *(edit to match your PCB)*
- Power input + motor phase outputs *(edit to match your PCB)*

---

## Repository Structure
> Adjust folder names to match your repo.

- `Hardware/` – schematics, PCB layout, fabrication outputs (Gerbers)
- `BOM/` – BOM files, part numbers, assembly notes
- `Docs/` – wiring diagrams, photos, notes

---

## Hardware (PCB)
**Driver:** DRV8313 (3 half-bridges, BLDC driver)

### Key specs (fill these in)
- Supply voltage: **12 V**
- Max phase current (design target): **3 A**
- PWM input: **3 PWM**
- Control interface: **STM32**

### Photos / renders
Add images like this (put your images in `Docs/` or use GitHub uploads):

![PCB render](Docs/pcb_render.png)  
![Assembled board](Docs/assembled.jpg)

---

## Bill of Materials (BOM)
List critical parts (example layout below):

1. **DRV8313** – 3-phase driver IC
2. **ASC712** – Hall-effect current sensor
3. **LMR36015S** – synchronous step-down buck converter
4. **Connectors**
   - Power input (VIN/GND)
   - Motor outputs (U/V/W)
   - Control header (PWM/EN/GND/FAULT, etc.)
   - current sense output 

---
