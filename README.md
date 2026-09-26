# 🌿 Automated Aquaponic Garden PLC with Web Interface

![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)
![Course](https://img.shields.io/badge/CEG%204980-Team%2011-orange.svg)

> **CEG 4980 Team 11 Capstone Project**  
> A complete Programmable Logic Controller (PLC) and IoT system for an aquaponic garden, fully manageable via a responsive web-based interface.

## 📝 Project Overview
Aquaponics combines aquaculture (raising fish) and hydroponics (soil-less plant cultivation) into a symbiotic ecosystem. This project bridges edge hardware and modern software to automate the monitoring, maintenance, and environmental control of an aquaponic system using a central PLC (Programmable Logic Controller) or microcontroller, managed remotely through a centralized web dashboard.

## ✨ Key Features
- **Real-Time Sensor Monitoring:** Continuously tracks vital water metrics including Temperature, pH, Dissolved Oxygen (DO), and Water Levels.
- **Automated Actuator Control:** Intelligently triggers water pumps, grow lights, and automatic fish feeders based on customizable sensor thresholds.
- **Web-Based Dashboard:** A centralized UI for viewing historical data trends, current system status, and manually overriding automated controls.
- **Alert System:** Notifies users of critical system states (e.g., extremely low water levels, pump failure, or dangerous pH spikes).

## 🏗️ System Architecture
The repository encompasses both the edge logic (PLC) and the web stack:
1. **Hardware Layer:** Sensors and relays wired directly to the primary PLC unit.
2. **Backend Services:** A Python-based API server that interfaces with the PLC (via Modbus, MQTT, or serial), logs telemetry to a database, and processes web requests.
3. **Frontend Dashboard:** A UI that fetches real-time telemetry and sends user commands back down to the hardware via the backend.

## ⚙️ Hardware Requirements
- **Controller:** PLC or Microcontroller unit (e.g., ESP32, Raspberry Pi, Arduino)
- **Sensors:** 
  - Waterproof Temperature Sensor (e.g., DS18B20)
  - Analog pH Sensor
  - Ultrasonic Water Level Sensor
- **Actuators:**
  - Relay Module (for 120V/240V mains control)
  - Submersible Water Pump
  - LED Grow Lights
  - Stepper/Servo Motor (for fish feeder)

## 💻 Installation & Setup

### Prerequisites
- Python 3.8+
- PLC programming environment or Arduino IDE (if compiling C++ for microcontrollers)

### Quick Start
1. **Clone the repository**
```bash
   git clone [https://github.com/PythonProgramm3r/Automated-Aquaponic-Garden-PLC-using-a-web-based-interface.git](https://github.com/PythonProgramm3r/Automated-Aquaponic-Garden-PLC-using-a-web-based-interface.git)
   cd Automated-Aquaponic-Garden-PLC-using-a-web-based-interface
