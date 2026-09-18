# RadiaX

**Open-source desktop micro-CT platform built from scratch by two students.**

RadiaX combines custom X-ray hardware, embedded computing, FPGA acceleration, a custom X-ray detector, and modular precision mechanics into a research-oriented CT platform.

![RadiaX CT](pictures/asemasem_2026-Aug-04_02-31-56AM-000_CustomizedView5246807532_jpg%20%282%29.jpg)

> **Built from scratch.** Custom electronics, X-ray system, detector, mechanics, FPGA platform, software and reconstruction pipeline.

## Hardware

### Computing & FPGA Platform

RadiaX uses a custom **Rockchip RK3566** computing platform for scanner control, data handling and the software stack.

The 8-layer custom PCB integrates LPDDR4, eMMC, PCIe, USB 3.x, HDMI, MIPI-DSI, Gigabit Ethernet and custom power monitoring.

![RK3566 SBC](pictures/Screenshot%202026-09-10%20222655.png)

A separate **Kintex-7 FPGA platform** is currently in development for high-speed detector acquisition, signal processing and hardware-accelerated reconstruction.

The FPGA architecture is intended to support future **AI acceleration and hardware/software co-processing**.

### X-ray System

RadiaX uses a custom **dual-tube X-ray architecture** designed for different imaging regimes.

The X-ray head and supporting electronics are developed in-house, including high-voltage generation, filament power, control electronics and mechanical integration.

The tube enclosure incorporates **high-voltage isolation and mineral-oil cooling**, combining dielectric insulation with passive thermal management.

![X-ray Head Internals](pictures/X-Ray_head_2026-Sep-12_04-07-46PM-000_CustomizedView2150125544_jpg.jpg)

A **monoblock magnetic filter** is being developed to reduce unwanted low-energy X-ray components before they reach the imaging system.

### Custom X-ray Detector

A custom scintillator-based X-ray detector is being developed specifically for RadiaX.

The detector combines **CIS/CMOS imaging circuitry, scintillator optics and custom mechanical integration** rather than relying on a conventional commercial CT detector.

A larger custom CIS-based scanner is currently in development.

### Modular Mechanics

The scanner uses a modular mechanical architecture designed specifically around the CT geometry.

The Mark 2 mechanical system incorporates:

* **3-axis kinematic object positioning**
* Motorized rotational and linear positioning
* Custom X-ray head and detector mounts
* Modular aluminum extrusion and panel construction
* Custom structural components and interfaces

Structural design is supported by **component-level, static and dynamic FEA**, including stress, deflection and modal analysis.

Natural-frequency simulations are used to investigate structural resonance and vibration from the motion system during long rotational scans.

Mass-center and load-distribution analysis is also used to maintain stable weight distribution across the rotating and stationary structures.

## AI & Reconstruction

RadiaX is being designed around a hardware-accelerated reconstruction pipeline.

The future FPGA platform is intended to accelerate computationally intensive parts of the imaging pipeline, with **AI-based image processing and reconstruction** planned alongside conventional reconstruction methods.

## Supported By

RadiaX has received support from **Radiacode**, contributing radiation-detectors.

[Radiacode](https://radiacode.com/)

## Project Status

RadiaX is actively under development.

| Subsystem                 | Status         |
| ------------------------- | -------------- |
| RK3566 computing platform | Prototype      |
| X-ray system              | Prototype      |
| Dual-tube architecture    | Prototype      |
| Custom detector           | In development |
| CIS scanner               | In development |
| Kintex-7 FPGA platform    | In development |
| Modular mechanical system | REV. 2         |
| FEA & structural analysis | Active         |
| AI / reconstruction       | In development |

Design files, measurements and technical documentation will be published as they are cleaned up and finalized.

---

## Built by

**Luka & Marco**

Two students developing the complete platform together — from X-ray hardware and custom electronics to the detector, FPGA, software, mechanical systems and structural analysis.
