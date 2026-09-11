# RadiaX

RadiaX is an open-source desktop micro CT platform created from scratch using custom hardware, software, and mechanics.

![RadiaX CT](pictures/asemasem_2026-Aug-04_02-31-56AM-000_CustomizedView5246807532_jpg%20%282%29.jpg)

The system combines a custom FPGA platform, a custom ARM-based computing platform, a custom flat-panel X-ray detector, and a modular mechanical system into a single research-oriented CT platform.

## Hardware

### Custom ARM Computing Platform

RadiaX uses a custom-designed 8-layer single-board computer based on the Rockchip RK3566.

The board is designed from the schematic through PCB layout specifically for the RadiaX system and integrates the main computing, high-speed I/O, memory, and power infrastructure required by the scanner.

Key features include:

- Rockchip RK3566 ARM SoC
- LPDDR4-2133 memory
- eMMC storage
- PCIe 2.1 x1
- USB 3.x
- HDMI
- MIPI-DSI display interface
- Gigabit Ethernet
- Custom power architecture and power monitoring
- BGA fanout and via-in-pad
- Controlled-impedance high-speed routing

The RK3566 platform provides the main embedded computing interface between the scanner hardware, FPGA subsystem, detector and software stack.

### FPGA Platform

RadiaX uses a custom FPGA platform for high-speed data acquisition and processing.

### X-ray Detector

A custom flat-panel X-ray detector is being developed using a scintillator-based imaging architecture and CMOS image sensors.

### Mechanical System

The scanner uses a modular custom mechanical design developed specifically for the desktop CT architecture.

## Pictures

### RadiaX

![RadiaX CT](pictures/asemasem_2026-Aug-04_02-31-56AM-000_CustomizedView5246807532_jpg%20%282%29.jpg)

### RK3566 Computing Platform

![RK3566 SBC](pictures/Screenshot%202026-09-10%20222655.png)

![RK3566 SBC](pictures/Screenshot%202026-09-10%20222714.png)

## Project Status

RadiaX is actively under development.

Hardware, FPGA, detector, software and mechanical systems are being developed in parallel. Additional design files and technical documentation will be published as they are cleaned up and finalized.
