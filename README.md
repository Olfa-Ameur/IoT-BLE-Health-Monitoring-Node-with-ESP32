# 🩺 ESP32 BLE Health Monitoring System

Embedded IoT system for real-time heart rate monitoring and remote device control using Bluetooth Low Energy (BLE).

This project implements a BLE health monitoring node based on ESP32-C3, capable of measuring heart rate, displaying data on an LCD screen, and controlling a servo motor remotely via a mobile application.

---

## 📡 Project Overview

This project demonstrates how Bluetooth Low Energy (BLE) can be used in IoT healthcare applications.

The system performs three main tasks:

- Real-time heart rate acquisition  
- Wireless transmission of physiological data via BLE  
- Remote control of environmental devices using BLE commands  

The project also includes BLE packet analysis using **Wireshark** and an **nRF51 dongle**, enabling a deeper understanding of BLE communication.

---

## ⚙️ Features

- Real-time heart rate monitoring
- LCD display using I2C interface
- BLE communication using GATT services
- Remote servo motor control via BLE
- Mobile interaction using nRF Connect
- BLE packet sniffing and analysis using Wireshark

---

## 🧩 Hardware Components

- ESP32-C3 microcontroller
- Heart rate sensor
- LCD display (I2C)
- Servo motor
- nRF51 Dongle (BLE Sniffer)
- Smartphone with nRF Connect

---

## 💻 Software Architecture

The firmware was developed using **ESP-IDF (Espressif IoT Development Framework)**.

Key modules include:

- BLE stack using NimBLE
- ADC heart rate acquisition
- PWM servo control
- I2C LCD driver
- FreeRTOS tasks

---

## 📶 BLE Services

### Heart Rate Service

Provides heart rate measurements through a **readable GATT characteristic**.

Example data:
BPM: 73

### Servo Control Service

Allows remote servo motor control.

Command example:
Write: 90

The servo moves to **90° position**.

---

## 📊 BLE Packet Analysis

To analyze BLE communication:

- nRF51 dongle programmed as BLE sniffer
- Packets captured using Wireshark
- Filtering using **BTATT filter**

This allows observation of:

- Advertising packets
- GATT read operations
- GATT write commands
- BLE channel communication

---

## 🛠 Tools Used

- ESP-IDF
- Embedded C
- Wireshark
- nRF Connect
- NimBLE Stack
- FreeRTOS

---

## 🚀 Future Improvements

- Mobile application development
- Battery powered wearable device
- Cloud integration
- Data logging system
- Machine learning for health monitoring

---

## 👨‍💻 Author

Embedded Systems & IoT Developer

Special interests:

- Embedded systems
- Bluetooth Low Energy
- IoT devices
- Firmware development
