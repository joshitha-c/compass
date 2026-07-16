# STM32WB Electronic Compass

A compact electronic compass and environmental sensing board built around the **STM32WB35CEU6A** microcontroller. The design combines a 3-axis magnetometer, barometric pressure sensor, USB-C connectivity, and BLE capability into a low-power embedded platform.

---

## Features

- STM32WB35CEU6A ARM Cortex-M4 + BLE MCU
- LIS2MDL 3-axis magnetometer
- LPS22DF digital barometric pressure sensor
- USB Type-C interface
- 3.3V regulated power supply
- SWD programming/debug interface
- UART debug interface
- External high-speed and low-speed crystals
- Designed in KiCad

---

## Hardware Overview

### Microcontroller

**STM32WB35CEU6A**

- ARM Cortex-M4
- Integrated Bluetooth Low Energy radio
- USB Full-Speed
- Multiple UART, SPI and I²C peripherals
- Low-power operation

---

### Sensors

#### LIS2MDL Magnetometer

Provides:

- X/Y/Z magnetic field measurements
- Digital I²C interface
- Low power operation
- Electronic compass functionality

Typical applications:

- Heading estimation
- Navigation
- Orientation sensing

---

#### LPS22DF Pressure Sensor

Provides:

- Atmospheric pressure
- Temperature measurement
- Digital I²C interface

Applications:

- Altitude estimation
- Weather monitoring
- Environmental sensing

---

## Power Supply

Input power is supplied through:

- USB Type-C connector

Power regulation:

- MIC5365-3.3V LDO regulator
- 3.3 V system rail

The design includes multiple decoupling capacitors near the MCU and sensors for stable operation.

---

## Clock Sources

The board includes:

- 32 MHz external crystal
  - Main system clock
  - USB timing
  - BLE radio

- 32.768 kHz crystal
  - Real-Time Clock (RTC)
  - Low-power timing

---

## Interfaces

### USB

USB Type-C connector

Supports:

- Device communication
- Firmware updates
- Power input

---

### SWD

Programming interface:

| Signal | Description |
|---------|-------------|
| SWDIO | Debug data |
| SWCLK | Debug clock |
| NRST | Reset |
| 3.3V | Reference |
| GND | Ground |

Compatible with:

- ST-Link V2
- ST-Link V3

---

### UART

Dedicated UART header for:

- Debug output
- Logging
- Bootloader communication

---


## Pin Summary

| Peripheral | Interface |
|------------|-----------|
| LIS2MDL | I²C |
| LPS22DF | I²C |
| USB | USB FS |
| SWD | Programming |
| UART | Debug |

---

## Applications

- Electronic compass
- Digital navigation
- BLE sensor node
- Altimeter
- Environmental monitoring
- Portable embedded systems
- IoT devices

---

## Future Improvements

- Battery charger
- LiPo support
- On-board IMU (accelerometer + gyroscope)
- Status LEDs
- User push buttons
- QSPI Flash
- Battery fuel gauge

Schematics:
<img width="1917" height="1010" alt="image" src="https://github.com/user-attachments/assets/14df0dbe-92cd-4968-9d46-af5fe9fa477f" />
Pcb:
<img width="1235" height="806" alt="image" src="https://github.com/user-attachments/assets/8e69b60f-baa2-4a69-85d6-45bf9f63a9da" />
