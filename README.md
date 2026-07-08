# Goosepad

A custom 6-key macro pad powered by the Seeed XIAO RP2040 and running QMK Firmware.

Goosepad is a compact DIY hackpad designed for shortcuts, macros, and custom controls. It features six individually wired keys, an OLED status display, and a custom PCB with a 3D printed case.

---

## Features

- 6 programmable keys
- Seeed XIAO RP2040 controller
- QMK Firmware support
- 0.91" 128x32 OLED display
- Custom PCB
- Custom 3D printed case
- Direct GPIO button wiring (no matrix)


## CAD
Used fusion 360 to design the case.
The case is divided into three parts:
- Bottom.stl
- Middle.stl
- Top.stl
![Goosepad schematic](/screenshot_pcb.png)

## Schematic



*Schematic showing the XIAO RP2040, buttons, OLED, and connections.*

---

## PCB Design

![Goosepad PCB](images/pcb.png)

*Custom PCB layout made in KiCad.*

---

## Case Design

![Goosepad case](images/case.png)

*3D printed case design showing how the PCB fits inside.*

---

# Hardware

## BOM (Bill of Materials)

| Part | Quantity | Notes |
|---|---:|---|
| Seeed XIAO RP2040 | 1 | Main microcontroller |
| 0.91" 128x32 OLED (SSD1306 I2C) | 1 | Status display |
| Mechanical switches | 6 | Key switches |
| Keycaps | 6 | MX-compatible |
| PCB | 1 | Custom Goosepad PCB |
| 3D printed case | 1 | Custom enclosure |
| USB-C cable | 1 | Programming and power |
| Solder | - | Assembly |

---

# Pinout

| Key | XIAO RP2040 Pin |
|---|---|
| Key 1 | D10 |
| Key 2 | D9 |
| Key 3 | D8 |
| Key 4 | D7 |
| Key 5 | D2 |
| Key 6 | D1 |

OLED:

| OLED | XIAO RP2040 |
|---|---|
| VCC | 3V3 |
| GND | GND |
| SDA | D4 |
| SCL | D5 |

---

# Firmware

Goosepad uses **QMK Firmware**.

Firmware source:
