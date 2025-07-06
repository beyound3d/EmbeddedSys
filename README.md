# Embedded System Software 

## 📦 Overview

This repository contains software components, configuration profiles, and tools for developing and deploying embedded system applications. It supports multiple target architectures (e.g., ARM Cortex-M, RISC-V) and integrates with real-time operating systems (RTOS), bare-metal environments, or custom hardware abstraction layers (HALs).

---

## 🛠️ Features

- ✅ Modular architecture (Drivers, Middleware, RTOS Abstraction)
- ✅ Support for multiple MCUs and development boards
- ✅ Real-time capabilities with optional RTOS integration (FreeRTOS, Zephyr, etc.)
- ✅ HAL/LL driver layer abstraction
- ✅ Firmware configuration and device profiles
- ✅ Peripheral support (I2C, SPI, UART, ADC, PWM, etc.)
- ✅ Build system compatibility: Make, CMake, and PlatformIO
- ✅ Unit testing and simulation stubs for host-side development

---

## 📁 Directory Structure



---

## 🚀 Getting Started

### Prerequisites

- GCC toolchain (e.g., arm-none-eabi-gcc)
- Python 3.x (for scripts and utilities)
- CMake or Make
- Optional: PlatformIO, Docker, QEMU for simulation

### Build Example (CMake)

```bash
mkdir build
cd build
cmake ..
make

### Flash to Device

```make flash
```

Make sure your device is connected and debugger (e.g., ST-Link, J-Link) is configured properly.


