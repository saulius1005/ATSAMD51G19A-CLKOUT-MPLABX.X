# ATSAMD51G19A Basic GPIO / Clock Demo

## Overview

This is a minimal embedded project for the **ATSAMD51G19A** microcontroller demonstrating:

- Core clock initialization using:
  - 24 MHz external TCXO
  - 128 MHz DPLL0 based on XOSC1
- Basic GPIO initialization and toggling
- Low-level register manipulation for PORT and PMUX

The project serves as a starting template for exploring clock setup and GPIO control on ATSAMD51G19A.

---

## Features

- **Clock setup**
  - `cpu_24MHz_TCXO_init()`: sets CPU to 24 MHz using external crystal oscillator
  - `cpu_128Mhz_DPLL0_XOSC1_init()`: sets CPU to 128 MHz using DPLL0 sourced from XOSC1
- **GPIO control**
  - Configures PA14 for peripheral function (PMUX M)
  - Configures PA17 as simple output
  - Toggles PA17 in an infinite loop

---

## Hardware Requirements

- Microcontroller: **ATSAMD51**
- External 24 MHz oscillator (optional, for TCXO mode)
- Access to PA14 and PA17 pins for GPIO test

---

## Notes

- **Disclaimer:** This code is unofficial and may contain certain limitations.
- This is intended as a learning/demo project and not production-ready.

---
