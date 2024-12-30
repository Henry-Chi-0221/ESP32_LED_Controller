# ESP32 LED Controller

## Overview

This project provides a comprehensive solution for smart LED control and includes the following components:

1. **PCB Design** - A custom schematic and layout specifically tailored for the ESP32-based LED controller.
2. **3D Modeling** - A detailed enclosure design that protects the hardware and simplifies installation.
3. **Code** - A configuration script designed for seamless ESPHome integration with Home Assistant, enabling quick deployment and customization.



---

## 1. PCB Design

![Schematic_esp32_LED_controller_2024-12-30](https://github.com/user-attachments/assets/752eadc4-90a1-4f4c-a153-562208cef747)
The hardware design is centered around the ESP32-S2 microcontroller, which provides robust features for IoT applications. Key elements include:

- A reliable power supply circuit featuring AC-DC conversion (12V) for stable performance.
- USB-C interface for programming, debugging, and potential firmware updates.
- IR LED output for infrared communication, along with MOSFET drivers for driving high-power LED strips effectively.
- Flexible input/output pins allowing future expansions and additional peripheral connections.

**Schematic**: Refer to `Schematic_esp32_LED_controller.pdf` for the detailed circuit diagram and connections.

---

## 2. 3D Modeling

The 3D enclosure model is crafted to provide structural integrity and ease of use. Key features include:

- A compact and durable design to protect the PCB and associated components from physical damage and dust.
- Built-in ventilation slots to ensure proper airflow and heat dissipation, preventing overheating.
- Predefined mounting points and slots for secure installations, making it suitable for wall mounting or embedding into other systems.
- Modular design to accommodate future upgrades or expansions without requiring major redesigns.

---

## 3. Code

The software is built using ESPHome and integrates seamlessly with Home Assistant, enabling smart control and monitoring. The YAML configuration script is customized to simplify setup and operation.

### Key Features:

- Wi-Fi connectivity with automatic fallback hotspot for easy setup and troubleshooting.
- Light control via GPIO pins to manage LED outputs directly.
- IR emitter functionality for controlling external devices, such as appliances and entertainment systems.
- Flexible automation through Home Assistant, allowing users to create complex scenes and schedules.

**Code File**: `controller.yaml`

### Dependencies:

- [Home Assistant](https://www.home-assistant.io/) - An open-source platform for smart home integration.
- [ESPHome Plugin](https://esphome.io/) - A tool for ESP-based device configuration and deployment.

### Setup:

1. Install the ESPHome plugin in Home Assistant by following the official documentation.
2. Upload the provided `controller.yaml` configuration file to ESPHome.
3. Compile the firmware and flash it onto the ESP32 board using a USB connection.
4. Configure Wi-Fi credentials and verify the connection to the Home Assistant dashboard.
5. Customize device behaviors and automation routines within the Home Assistant interface.
6. Perform periodic updates to ensure compatibility with the latest features and bug fixes.
