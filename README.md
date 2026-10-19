# 🚨 Arduino Ultrasonic Perimeter Intruder Detection & Alarm System

[![Platform: Arduino](https://img.shields.io/badge/Platform-Arduino-00979D.svg?logo=arduino&logoColor=white)](https://www.arduino.cc/)
[![Application: Security & Surveillance](https://img.shields.io/badge/Application-Perimeter%20Intrusion%20Detection-D32F2F.svg)]()
[![Sensor: Ultrasonic Radar](https://img.shields.io/badge/Sensor-HC--SR04%20Radar-orange.svg)]()
[![Language: C++](https://img.shields.io/badge/Language-C%2B%2B-00599C.svg?logo=c%2B%2B&logoColor=white)](https://en.wikipedia.org/wiki/C%2B%2B)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Status: Tested](https://img.shields.io/badge/Hardware%20Status-Tested%20%26%20Verified-brightgreen.svg)]()

An active ultrasonic security and perimeter breach alarm system for doorways, corridors, and restricted access zones. Measures spatial distance using an HC-SR04 ultrasonic transducer and visualizes intruder proximity via a 4-stage graduated LED threat ladder, providing real-time perimeter tripwire surveillance.

---

## 🛠️ Hardware Requirements & Bill of Materials (BOM)

| Component | Specification | Quantity |
| :--- | :--- | :--- |
| **Microcontroller** | Arduino Uno, Nano, or Pro Mini | 1 |
| **Ultrasonic Sensor** | HC-SR04 Transducer Module | 1 |
| **Threat Level LEDs** | 5mm LEDs (Green, Yellow, Orange, Red) | 4 |
| **Resistors** | 220Ω, 1/4W, 5% carbon film | 4 |
| **Piezo Buzzer (Optional)** | 5V Piezo Buzzer on Pin 5 | 1 |
| **Breadboard & Wires** | Half-size breadboard with Dupont jumpers | 1 set |

---

## 🔌 Circuit Pinout & Wiring

| Arduino Pin | Hardware Component | Resistor | Function |
| :--- | :--- | :--- | :--- |
| **Pin D9** | HC-SR04 Trig | Direct | 10µs ultrasonic pulse trigger |
| **Pin D10** | HC-SR04 Echo | Direct | Return echo capture |
| **Pin D2** | Threat Level LED 1 Anode | 220Ω in series | Outer perimeter alert |
| **Pin D3** | Threat Level LED 2 Anode | 220Ω in series | Mid-range proximity |
| **Pin D4** | Threat Level LED 3 Anode | 220Ω in series | Close approach |
| **Pin D5** | Threat Level LED 4 Anode | 220Ω in series | Immediate breach |
| **GND** | LED Cathodes, Sensor Ground | Direct | Common circuit ground |

---

## 🚀 Installation & Upload

1. Clone repository:
   ```bash
   git clone https://github.com/youniquestar/arduino-intruder-detection-alarm.git
   ```
2. Open [`intruder_detection_alarm_system/intruder_detection_alarm_system.ino`](intruder_detection_alarm_system/intruder_detection_alarm_system.ino) in Arduino IDE.
3. Select board and port, and click **Upload**.

---

## 📜 License

Licensed under the [MIT License](LICENSE).
