
# STM32-Based 12V Lead-Acid Battery Analyzer

A microcontroller-based project for analyzing the condition of a 12V lead-acid battery using voltage measurements and internal resistance estimation.

## Overview

This project implements a battery analysis system based on the STM32F103C8T6 microcontroller. It is designed to evaluate key battery parameters and provide an estimation of its condition.

The system focuses on measuring battery voltage, estimating internal resistance, and calculating State of Charge (SoC) and State of Health (SoH).

## Features

- Battery voltage measurement
- Internal resistance estimation
- State of Charge (SoC) estimation
- State of Health (SoH) estimation
- STM32-based embedded firmware
- ADC-based measurement processing
- Measurement cycle initiated by the user

## Hardware Platform

- **Microcontroller:** STM32F103C8T6
- **Battery type:** 12V lead-acid battery
- **Development environment:** STM32CubeIDE
- **Firmware framework:** STM32 HAL

## Software

The firmware is developed in C and uses the STM32 HAL library.

The project includes:
- ADC configuration and measurement acquisition
- Measurement processing
- Battery parameter estimation
- Peripheral initialization and configuration

## Project Structure

| Directory / File | Description |
|---|---|
| `Core/` | Application source code and header files |
| `Drivers/` | STM32 HAL and CMSIS libraries |
| `EWARM/` | IAR Embedded Workbench project files |
| `Kursavaia.ioc` | STM32CubeMX configuration |
| `STM32F103C8TX_FLASH.ld` | Linker script |
| `.project`, `.cproject` | Eclipse-based project configuration |

## Getting Started

### Requirements

- STM32CubeIDE
- STM32F103C8T6 development board or compatible hardware
- ST-Link programmer/debugger (for programming and debugging)

### Opening the Project

1. Clone or download this repository.
2. Launch STM32CubeIDE.
3. Select a workspace.
4. Go to **File → Import**.
5. Select **General → Existing Projects into Workspace**.
6. Select the project root directory.
7. Select the detected project and click **Finish**.

### Building the Project

1. Open the imported project in STM32CubeIDE.
2. Make sure the project is selected in Project Explorer.
3. Click **Build** (hammer icon) or select **Project → Build Project**.
4. Check the Console for build errors.

### Programming the Microcontroller

1. Connect the STM32 board to the ST-Link debugger/programmer.
2. Configure the appropriate debug/programming connection.
3. Click **Run** or **Debug** in STM32CubeIDE.
4. Follow the IDE prompts to program the microcontroller.

The firmware execution and measurement functionality require the corresponding hardware and measurement circuit.

## Development

The project was developed as part of an academic engineering project involving embedded systems, microcontroller programming and battery parameter analysis.

## Limitations

The calculated battery parameters are estimates based on the implemented measurement and calculation model. The accuracy of the estimations depends on measurement conditions, calibration and the adopted model.

---

**Technologies:** C, STM32, STM32 HAL, STM32CubeIDE, STM32CubeMX, Embedded Systems.
