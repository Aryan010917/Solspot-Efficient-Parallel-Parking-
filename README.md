# Solar Parallel Car Parking System

## 📚 Overview
This project implements a **solar-powered parallel car parking system** using an ESP32 microcontroller, L298N motor driver, servos, and solar panels for sustainable power. The system enables real-time car movement control via a web-based interface using ESP32's WiFi capabilities.

## ⚡ Features
- Real-time control of car movement (forward, backward, left, right) through web interface.
- Adjustable speed and turning angle via slider controls.
- Solar panel integration with UBEC module to recharge batteries.
- Four servo motors (right front, right back, left front, left back) for precise maneuvering.
- Uses L298N motor driver to control left and right motors.

## 📐 Circuit Diagram
![Circuit Diagram](Circuit%20diagram.png)

## 🔌 Pin Connections
| **ESP32 Pins** | **L298N Driver Pins** |
| -------------- | --------------------- |
| IO22           | enA                   |
| IO16           | IN1                   |
| IO17           | IN2                   |
| IO18           | IN3                   |
| IO19           | IN4                   |
| IO23           | enB                   |

## 📄 Files
- **ESP32_Car_Control_Code.ino**: Full source code for ESP32 controlling servos and motors via WebSocket.
- **Circuit diagram.png**: Full wiring diagram showing connections between ESP32, L298N, motors, servos, UBEC, and solar panels.

## 📝 How to Run
1. Upload `ESP32_Car_Control_Code.ino` to your ESP32 board using Arduino IDE.
2. Connect the hardware according to the circuit diagram provided.
3. Power the system (preferably with the solar setup for eco-friendly use).
4. Connect to the ESP32 WiFi hotspot and open the web interface to control the car.

## 📦 Libraries Required
- `ESPAsyncWebServer`
- `AsyncTCP`
- `ESP32Servo`

## 🚀 Future Improvements
- Integrate camera module (ESP32-CAM) for live video feed.
- Enhance AI-based obstacle detection and autonomous parking.
- Optimize power management and add battery monitoring system.

---

Created by Aryan Kumar.
