# 🖐️ Gesture-Controlled Intensity of Light and Fan Speed Using Embedded Systems

🎓 **Final Year B.Tech Project** | Department of Electronics & Communication Engineering  
📍 Kaziranga University | 2025  
👤 Developed by: Ayan Sen

---

## 📌 Project Overview

This project is a contactless smart home automation system that enables the user to control **light intensity** and **fan speed** using specific hand gestures. Designed using **MediaPipe** and **OpenCV** for gesture detection and an **Arduino Uno** to generate PWM signals, it offers an intuitive and hygienic method of controlling devices.

PWM signals are transmitted based on the number of fingers detected. The system uses a **MOSFET** to control the DC fan and adjusts LED brightness using PWM. A **flyback diode** (1N4007) is used to protect the fan circuitry from voltage spikes caused by inductive load switching.

---

## 🔧 Technology Stack

| Category          | Tools/Components Used                      |
|------------------|---------------------------------------------|
| Gesture Detection | Python, OpenCV, MediaPipe                  |
| Microcontroller   | Arduino Uno                                |
| Communication     | USB Serial (PySerial)                      |
| Actuation         | IRFZ44N MOSFET, LED Bulb, DC Fan           |
| Protection        | 1N4007 Flyback Diode (across fan terminals)|
| Power Supply      | 12V SMPS (fan), USB 5V (Arduino)           |

---

## 🧠 Gesture-to-Action Mapping

| ✋ Finger Gesture | 🔦 LED Brightness       | 🌬 Fan Speed         |
|------------------|-------------------------|----------------------|
| ☝️ 1 Finger       | Dim                     | Off                  |
| ✌️ 2 Fingers      | Off                     | Low Speed            |
| 🤟 3 Fingers      | Full Brightness         | Off                  |
| ✌️✌️ 4 Fingers    | Off                     | High Speed           |
| ✋ 5 Fingers       | Full Brightness         | Full Speed           |

Gestures are processed via MediaPipe’s 21-point hand landmark detection, and the detected finger count is mapped to PWM signals sent to the Arduino Uno to drive connected appliances.

---

## 🧰 Circuit Design Highlights

- **MOSFET-Based Switching:** IRFZ44N controls the 12V DC fan using PWM from Arduino Uno.
- **LED Brightness Control:** Controlled via PWM pin with safe resistor configuration.
- **Flyback Diode Protection:** 1N4007 diode connected across fan terminals ensures safety from voltage spikes due to inductive load switching.
- **Modular Design:** All components are wired using a breadboard for clarity and portability.

---

## 📄 Repository Contents

- `README.md` – This project overview
- `project_summary.pdf` – System architecture and technical abstract
- `gesture_mapping_table.pdf` – Printable gesture-to-device mapping chart
- `demo_images/` – Folder containing snapshots of working prototype

> ⚠️ **Note:** Full source code (Python + Arduino) is private to protect intellectual property.  
> Available upon request for academic review or verification.

---

## 💡 Applications

- Assistive technology for physically challenged users
- Smart home and IoT applications
- Touchless control in medical or hygiene-critical environments
- Energy-efficient automation systems

---

## 🔐 Project Protection Notice

This project and its contents are the intellectual property of **Ayan Sen**.  
All rights are reserved. The source code, circuit design, and implementation logic  
are shared only for academic demonstration and are **not to be copied, reused, or modified**  
for commercial or academic submissions without written permission from the author.

