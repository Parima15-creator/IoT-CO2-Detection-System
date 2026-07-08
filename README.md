# IoT-Based CO2 Detection System using MQ-135 Gas Sensor

[cite_start]Poor indoor air quality is a growing concern in schools, laboratories, homes, and offices[cite: 15]. [cite_start]When CO₂ levels rise above safe limits, occupants can experience fatigue, headaches, and reduced cognitive function[cite: 17]. 

[cite_start]This project provides a low-cost IoT solution to identify and address this issue[cite: 24]. [cite_start]It utilizes an MQ-135 gas sensor interfaced with an Arduino UNO R4 WiFi to read analog gas concentrations and classify them into three levels: Clean, Moderate, and High CO₂[cite: 24, 25]. [cite_start]The system provides simple visual indications on the onboard 8x12 LED matrix using intuitive symbols (✔ for fresh air, ⚠ for moderate, and ❌ for high CO₂) without requiring a computer screen[cite: 20, 25]. [cite_start]Data is also logged to the Serial Monitor for analysis[cite: 26].

## 🛠️ Hardware Requirements
* [cite_start]Arduino UNO R4 WiFi [cite: 30]
* [cite_start]MQ-135 Gas Sensor [cite: 40]
* Breadboard & Jumper Wires

## 🔌 Circuit Connections
[cite_start]Make the following connections between your MQ-135 sensor and the Arduino UNO R4 WiFi[cite: 46]:

| MQ-135 Pin | Arduino Pin | Reason |
| :--- | :--- | :--- |
| **VCC** | 5V | [cite_start]Powers the sensor heater element (~150mA draw) [cite: 46] |
| **GND** | GND | [cite_start]Common ground connection [cite: 46] |
| **A0 (Analog Out)** | A0 (Analog In) | [cite_start]Outputs 0-5V proportional to gas concentration [cite: 46] |
| **D0 (Digital Out)**| *Not connected* | [cite_start]Onboard comparator; unused in this project [cite: 46] |

*(Replace the link below with your Fritzing circuit diagram screenshot)*
![Circuit Diagram](link-to-your-circuit-screenshot.png)

## 💻 Software Requirements
* [cite_start]**Arduino IDE 2.x:** Code editor, compiler, and uploader[cite: 49].
* [cite_start]**Arduino_LED_Matrix.h:** Built-in library to control the 8x12 LED matrix on the Arduino UNO R4 WiFi[cite: 49].

## 🚀 How to Use the Code

This repository contains two separate code versions calibrated for different testing environments. 

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/Parima15-creator/IoT-CO2-Detection-System.git](https://github.com/Parima15-creator/IoT-CO2-Detection-System.git)
