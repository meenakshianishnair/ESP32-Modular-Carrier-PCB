 # ESP32 Modular Carrier PCB

## Overview
A custom-designed 80 mm x 96 mm carrier board built in KiCad to host an ESP32 DevKitC along with modular peripheral connections for an I2C OLED display, Time-of-Flight (ToF) sensor, capacitive touch input, and dedicated 5V power input.

## Specifications
- **Board Dimensions:** 80.0 mm x 96.0 mm
- **Copper Layers:** 2-layer (F.Cu for routing, B.Cu / GND plane)
- **Design Rules:** Zero DRC errors, 0.25 mm track width, standard 2.54 mm pin spacing.

## Bill of Materials (BOM)
| Item | Qty | Reference | Footprint | Description |
| :--- | :--- | :--- | :--- | :--- |
| **1** | 1 | `U1` | Module_ESP32_DevKitC | ESP32 DevKitC Development Board (Socket headers) |
| **2** | 1 | `OLED` | PinHeader_1x04_P2.54mm_Vertical | 0.96" I2C OLED Display Module (4-pin) |
| **3** | 1 | `TOF` | PinHeader_1x04_P2.54mm_Vertical | VL53L0X / VL53L1X Time-of-Flight Sensor (4-pin) |
| **4** | 1 | `TOUCH` | PinHeader_1x04_P2.54mm_Vertical | Capacitive Touch Sensor Module (3-pin) |
| **5** | 1 | `PWR` | PinHeader_1x02_P2.54mm_Vertical | 5V / GND Power Input Terminal (2-pin) |

## Assembly Instructions
1. Solder the 19-pin female header sockets onto the central `J_LEFT` and `J_RIGHT` positions to securely mount the ESP32 DevKitC.
2. Solder vertical 2.54mm pin headers for the OLED, ToF, Touch, and Power modules according to their designated silk screen labels.
3. Verify continuity between the 5V and GND input rails before powering on the board.