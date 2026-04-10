# Smart Irrigation System

![Arduino](https://img.shields.io/badge/Platform-Arduino-00979D?style=flat-square&logo=arduino)
![C++](https://img.shields.io/badge/Language-C++-00599C?style=flat-square&logo=cplusplus)
![Arduino IDE](https://img.shields.io/badge/IDE-Arduino_IDE-teal?style=flat-square)

![Soil Sensor](https://img.shields.io/badge/Sensor-Soil_Moisture-green?style=flat-square)
![Rain Sensor](https://img.shields.io/badge/Sensor-Rain_Detection-blue?style=flat-square)
![Water Level](https://img.shields.io/badge/Sensor-Water_Level-lightblue?style=flat-square)
![Relay](https://img.shields.io/badge/Actuator-Relay_Module-red?style=flat-square)
![Pump](https://img.shields.io/badge/Actuator-Submersible_Pump-navy?style=flat-square)

An Arduino-based automated irrigation system that monitors soil conditions in real time and controls a water pump automatically — no manual intervention needed. Built as an independent project to explore sensor integration, control logic, and autonomous system design.

---

## 🌱 How It Works

The system continuously reads data from three sensors. Pump activation follows a simple but robust logic:

| Condition | Result |
|-----------|--------|
| Soil is dry + no rain detected + reservoir has water | ✅ Pump ON |
| Soil is wet | ❌ Pump OFF |
| Rain detected | ❌ Pump OFF |
| Reservoir empty | ❌ Pump OFF (prevents dry run) |

---

## ⚙️ Hardware

| Component | Role |
|-----------|------|
| Arduino MEGA | Main microcontroller |
| Soil moisture sensor | Reads soil water content (analog) |
| Rain detection sensor | Detects active rainfall (digital) |
| Water level sensor | Monitors reservoir level (analog) |
| Relay module | Switches pump on/off from Arduino signal |
| Submersible water pump | Delivers water to plants |

---

## 💻 Software

- **C++ control logic** written in Arduino IDE
- Polling-based sensor reading loop with threshold comparisons
- Relay control via digital output pins
- Serial monitor output for debugging and sensor readouts

---

## 🧠 What I Learned

- Analog and digital sensor integration on Arduino
- Writing reliable control logic in C++ for embedded systems
- Dealing with real-world issues like sensor drift and false readings
- Designing a system that runs autonomously over long periods without supervision
- Basic relay circuit wiring and pump control

---

## 📅 Timeline

**April 2021 – October 2021** | Independent Project
