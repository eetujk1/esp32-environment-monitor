# ESP32 Environment Monitor

A custom-designed environmental monitoring board based on the ESP32-WROOM-32E-N4.

The goal of this project is to build a compact device for monitoring room temperature and relative humidity, with the possibility of expanding it into a Wi-Fi-connected monitoring system.

## Overview

The PCB integrates the main controller, sensor interface, USB programming circuitry, and power regulation into a single board.

### Hardware

* **MCU:** ESP32-WROOM-32E-N4
* **Sensor:** DHT20
* **USB-to-UART:** CH340C
* **Voltage regulator:** AP2112K-3.3
* **Power input:** USB-C, 5 V
* **Programming:** Automatic boot mode selection with BOOT and RESET buttons
* **Sensor interface:** I²C

## Design Goals

* Custom PCB design and assembly
* Reliable temperature and humidity measurements
* Simple USB-based firmware development
* Wi-Fi connectivity for future monitoring applications
* Expandable hardware and firmware architecture

## Development Status

| Area                         | Status         |
| ---------------------------- | -------------- |
| PCB design                   | Completed      |
| PCB assembly                 | Ordered        |
| ESP32 and DHT20 installation | Pending        |
| Firmware                     | In development |
| Sensor validation            | Pending        |

## Planned Development

1. Bring up the hardware and verify the 3.3 V power rail.
2. Test USB communication and ESP32 firmware uploading.
3. Implement DHT20 sensor readings over I²C.
4. Validate temperature and humidity measurements.
5. Explore Wi-Fi monitoring and data visualization.

## Repository Structure

```text
esp32-environment-monitor/
├── hardware/       # PCB and schematic files
├── firmware/       # ESP32 source code
├── docs/           # Design notes and documentation
└── README.md
```

## Project Notes

This project is currently in the hardware bring-up stage. Firmware, measurements, and additional documentation will be added as development progresses.
