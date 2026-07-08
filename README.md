# 🌿 IoT-Based CO₂ Detection System using MQ-135 Gas Sensor

Poor indoor air quality is a growing concern in schools, laboratories, homes, and offices. When CO₂ levels rise above safe limits, occupants can experience fatigue, headaches, and reduced cognitive function.

This project provides a low-cost IoT solution for monitoring indoor air quality using an **MQ-135 Gas Sensor** and an **Arduino UNO R4 WiFi**. The sensor continuously measures air quality and classifies it into three categories:

- ✔ **Clean Air**
- ⚠ **Moderate CO₂**
- ❌ **High CO₂**

The result is displayed directly on the **built-in 8×12 LED Matrix** of the Arduino UNO R4 WiFi, eliminating the need for an external display. Sensor readings are also printed to the **Serial Monitor** for logging and analysis.

---

## 🛠️ Hardware Requirements

- 1 Arduino UNO R4 WiFi
- 1 MQ-135 Gas Sensor
- 1 Breadboard
- 3-6 Jumper Wires

---

## 🔌 Circuit Connections

Connect the MQ-135 sensor to the Arduino UNO R4 WiFi as follows:

| MQ-135 Pin | Arduino Pin | Purpose |
|------------|-------------|---------|
| **VCC** | **5V** | Powers the sensor |
| **GND** | **GND** | Common ground |
| **A0 (Analog Out)** | **A0** | Reads analog gas values |
| **D0 (Digital Out)** | *Not Connected* | Not used in this project |

## Circuit diagram
<img width="931" height="564" alt="image" src="https://github.com/user-attachments/assets/167c4cfa-11c5-4b24-9e63-e17695e78016" />

---

## 💻 Software Requirements

- Arduino IDE 2.x
- Arduino_LED_Matrix library (built into Arduino UNO R4 WiFi board package)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Parima15-creator/IoT-CO2-Detection-System.git
```

### 2. Open the Project

Open the required `.ino` file in the Arduino IDE.

### 3. Select the Board

- **Board:** Arduino UNO R4 WiFi
- **Port:** Select the COM port connected to your Arduino.

### 4. Upload the Code

Click **Upload** and wait for the sketch to be flashed onto the board.

### 5. Monitor the Output

- Open the **Serial Monitor** (9600 baud).
- Observe the LED Matrix for real-time air quality status.

---

## 📊 Air Quality Indicators

| LED Symbol | Status | Description |
|------------|--------|-------------|
| ✔ | Clean | Fresh air quality |
| ⚠ | Moderate | Ventilation recommended |
| ❌ | High CO₂ | Poor air quality; improve ventilation immediately |

---

## 📁 Project Structure

```
IoT-CO2-Detection-System/
│
├── Code/
│   ├── Mouth Breath CO2 testing
│   └── Other Substances
│
├── docs/
│
├── README.md
└── LICENSE
```

---

## 👨‍💻 Author

**Parima Tendulkar**
