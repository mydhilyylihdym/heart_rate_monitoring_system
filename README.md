# Heart Rate Monitoring System

## Overview
An ESP32-based smart health monitoring system capable of measuring heart rate, SpO2, and body temperature in real time using MAX30100 and LM35 sensors. The system displays data on an OLED screen and hosts a web server for wireless monitoring.

---

## Features
- Real-time heart rate monitoring
- SpO2 (blood oxygen) measurement
- Body temperature sensing
- OLED display output
- Wi-Fi based web monitoring
- HTTP server for remote access
- Health warning alerts
- Continuous sensor updates

---

## Components Used
- ESP32
- MAX30100 Pulse Oximeter Sensor
- LM35 Temperature Sensor
- SSD1306 OLED Display

---

## System Working
The ESP32 collects sensor data from the MAX30100 and LM35 sensors.  
The readings are processed and displayed on the OLED display while simultaneously being hosted through a Wi-Fi HTTP server.

The system generates warning messages when:
- Heart rate exceeds safe limits
- Heart rate falls below safe limits
- Temperature exceeds threshold values

---

## Wi-Fi Configuration
- SSID: `Health Monitor`
- HTTP Server Port: `80`

The ESP32 operates as a Wi-Fi Access Point, allowing nearby devices to access the health dashboard directly through a browser.

---

## Technologies Used
- Embedded C++
- ESP32 Wi-Fi
- HTTP Server
- OLED Graphics
- Sensor Data Processing

---

## Future Improvements
- Cloud integration
- Mobile app support
- Data logging
- TinyML-based anomaly detection
- Emergency alert system

---

## Project Structure

```text
heart-rate-monitoring-system/
│
├── code/
├── images/
├── circuit_diagram/
├── report/
└── README.md
