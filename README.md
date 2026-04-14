# ⚡ Smart Energy Meter using ESP32

A real-time IoT-based smart energy meter capable of monitoring overall and individual power consumption using ESP32 and multiple sensors. This project enables efficient energy tracking, visualization, and remote monitoring.

---

## 📌 Overview

Traditional energy meters lack real-time insights and detailed consumption analysis. This project introduces a **smart energy monitoring system** that provides:

- Real-time voltage, current, and power measurement
- Individual load monitoring (room-wise)
- Cloud-based data storage and visualization
- IoT-enabled remote access

---

## 🎯 Objectives

- Develop a **single-phase smart energy meter**
- Monitor **total and individual power consumption**
- Enable **real-time data visualization**
- Improve energy efficiency awareness

---

## 🏗️ System Architecture

The system consists of:

- Sensors → Data Acquisition → ESP32 Processing → Cloud → Visualization

The following diagram illustrates the internal architecture of the smart energy meter, including sensing, processing, and communication modules.

![System Architecture](https://github.com/user-attachments/assets/ec84373b-4bb4-43e5-a7d7-602802836b9b)

### 🔍 Description

- **Sensors**: ACS712, SCT-013, and ZMPT101B measure current and voltage  
- **Data Acquisition**: Analog signals are conditioned and fed to ESP32 ADC  
- **Processing**: ESP32 computes RMS values, power, and energy using EmonLib  
- **Cloud**: Data is transmitted via Wi-Fi to Firebase for storage  
- **Visualization**: Data is displayed on OLED and visualized using Python/Google Sheets 

### 🔌 Hardware Components

- **ESP32 DevKit V1**
  - Dual-core processor (up to 240 MHz)
  - Built-in Wi-Fi for IoT connectivity

- **Current Sensors**
  - ACS712 (up to 30A)
  - SCT-013 (up to 100A)

- **Voltage Sensor**
  - ZMPT101B (up to 250V)

- **Display**
  - 128x64 OLED (SPI)

---

## 💻 Software Stack

- **Embedded Development**
  - PlatformIO (ESP32 programming)

- **Cloud & Backend**
  - Firebase (real-time database)

- **Data Visualization**
  - Python (custom frontend)
  - Google Sheets (charts & graphs)

---

## ⚙️ Features

- 📡 Real-time energy monitoring  
- 🏠 Individual load tracking (room-wise)  
- ☁️ Cloud data storage (Firebase)  
- 📊 Live data visualization  
- 📟 OLED display output  

---

## 🔬 Implementation Details

### Phase 1: Hardware Setup
- Component selection and procurement
- Sensor calibration using oscilloscope
- Distribution board design (up to 5kW load)

### Phase 2: Firmware & Software
- ESP32 programming for sensor data acquisition
- Power calculation algorithms
- Python-based visualization interface

### Phase 3: Testing & Validation
- Tested with 100W load
- Scaled testing up to 5kW lab setup
- Compared expected vs measured values

---

## 📈 Results

- Successfully implemented a **single-phase smart energy meter**
- Real-time monitoring of voltage, current, and power
- Accurate performance at moderate loads
- Cloud-based visualization achieved

---

## ⚠️ Limitations

- Reduced accuracy for currents below 1A  
- ESP32 ADC limitations when Wi-Fi is enabled  
- Sensor instability for very low loads  
- Initial delay for stable readings  

---

## 🚀 Future Improvements

### 🔋 System Enhancements
- Three-phase energy monitoring
- Power factor calculation
- Improved low-current sensing accuracy

### 🤖 Smart Features
- AI-based energy consumption analysis
- Usage pattern prediction
- Energy optimization recommendations

### 🛠️ Product Development
- Custom PCB design
- Compact enclosure for deployment
  
---

## 🧰 Built With

- EmonLib – Arduino Energy Monitoring Library  
  https://github.com/openenergymonitor/EmonLib

---  

## 📸 Project Gallery

*(Add your images here — hardware setup, graphs, PCB design, etc.)*

