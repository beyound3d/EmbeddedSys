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

├── config/ # Board-specific configurations and profiles
├── drivers/ # Low-level peripheral drivers
├── middleware/ # Protocol stacks or libraries (e.g., MQTT, Modbus)
├── rtos/ # RTOS abstraction layer
├── utils/ # Logging, debugging, timebase, etc.
├── examples/ # Sample applications and test cases
├── docs/ # Documentation and design notes
├── tests/ # Unit tests and host simulation
├── CMakeLists.txt # Build configuration
└── README.md # Project overview (this file)

---

## 🚀 Getting Started

### Prerequisites

- GCC toolchain (e.g., arm-none-eabi-gcc)
- Python 3.x (for scripts and utilities)
- CMake or Make
- Optional: PlatformIO, Docker, QEMU for simulation

### Build Example (CMake)

```
mkdir build
cd build
cmake
```

### Flash to Device

```make flash
```

Make sure your device is connected and debugger (e.g., ST-Link, J-Link) is configured properly.

### 🧪 Testing
Unit tests can be run on host using stubs/mocks. Navigate to the tests/ directory:
```
cd tests
make test
```

### 📚 Documentation
Documentation is available in the docs/ folder. Key topics include:

- System Architecture
- Driver & HAL Layer Design
- RTOS Integration
- Debugging & Logging Setup
- Deployment Guide

### 🖥️ Supported Boards / MCUs
- STM32F103 (Blue Pill)
- STM32F4 Discovery
- ESP32 DevKit
- NXP LPC1768
- ✅ Add your own via /config/

### 🔧 Configuration Profiles
Configuration profiles are defined in the config/ directory. These include:
- Clock & PLL settings
- Peripheral enable/disable
- Linker script and memory layout
- Startup sequences

Use config/profile_selector.h to switch between board targets.

### 📄 License
This project is licensed under the MIT License.

### 🤝 Contributing
Contributions are welcome! Please:
- Fork the repo
- Create a feature branch
- Submit a pull request

See CONTRIBUTING.md for full guidelines.



