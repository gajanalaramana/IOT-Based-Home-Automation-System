🏠 IoT-Based Home Automation System Using ESP8266

Home Automation report     https://github.com/gajanalaramana/IOT-Based-Home-Automation-System/blob/main/home%20ramana116%20(1).pdf 


Block Diagram     https://github.com/gajanalaramana/IOT-Based-Home-Automation-System/blob/main/block%20diagram.png   

Blynk and Wifi output    https://github.com/gajanalaramana/IOT-Based-Home-Automation-System/blob/main/blynk%20output%20and%20wifi%20connection.png

Hardware implementation circuit    https://github.com/gajanalaramana/IOT-Based-Home-Automation-System/blob/main/hardware%20circuit%20implementation.png

Arduino code for execution  https://github.com/gajanalaramana/IOT-Based-Home-Automation-System/blob/main/home.ino

 Output of Home Automation   
block diagram
An **IoT-based Home Automation System** developed using **NodeMCU (ESP8266)** and the **Blynk IoT platform** to remotely monitor and control household appliances. The system integrates multiple sensors for home security, environmental monitoring, gas leakage detection, fire detection, and water-level monitoring.

 📌 Project Overview

Home automation combines sensors, embedded systems, wireless communication, and IoT technology to provide convenient and intelligent control of household devices.

In this project, the **NodeMCU ESP8266** acts as the main controller and connects to the Internet through Wi-Fi. Sensor data is collected and displayed locally on an LCD as well as remotely through the **Blynk application**. Electrical appliances can be controlled using relay modules.

✨ Features

* 📱 Remote monitoring using Blynk
* 💡 Remote control of home appliances
* 🌡️ Temperature monitoring
* 💧 Humidity monitoring
* 🔥 Fire detection
* 🛢️ Gas leakage detection
* 🚶 Motion/security detection
* 🚰 Water-level monitoring
* 🔔 Buzzer-based safety alerts
* 📺 Real-time LCD display
* 📡 Wi-Fi-based IoT connectivity

🧰 Hardware Components

| Component                     | Purpose                                |
| ----------------------------- | -------------------------------------- |
| **NodeMCU ESP8266**           | Main controller and Wi-Fi connectivity |
| **2-Channel Relay Module**    | Controls electrical appliances         |
| **DHT11 Sensor**              | Measures temperature and humidity      |
| **MQ-2 Gas Sensor**           | Detects gas leakage                    |
| **Flame Sensor**              | Detects fire/flame                     |
| **PIR Sensor**                | Detects human motion                   |
| **HC-SR04 Ultrasonic Sensor** | Measures distance/water level          |
| **16×2 LCD + I2C**            | Displays sensor readings               |
| **Buzzer**                    | Provides warning alerts                |
| **LEDs**                      | Status indication                      |
| **Breadboard & Jumper Wires** | Circuit connections                    |

The project report specifies these components as the core hardware used in the system.

⚙️ Working Principle

The system works in the following sequence:

1. **NodeMCU ESP8266** connects to the Wi-Fi network.
2. Sensors continuously collect information from the home environment.
3. The ESP8266 processes the sensor readings.
4. Temperature and humidity values are obtained from the **DHT11**.
5. The **MQ-2 sensor** monitors gas levels.
6. The **flame sensor** detects fire conditions.
7. The **PIR sensor** detects motion for security monitoring.
8. The **ultrasonic sensor** measures distance/water level.
9. Sensor values are displayed on the **LCD**.
10. Data is transmitted to the **Blynk application** through Wi-Fi.
11. Relays can be used to switch connected appliances ON/OFF.
12. In abnormal conditions, the system activates the buzzer and sends alerts through Blynk.



💻 Software & Technologies

* **Arduino IDE**
* **Embedded C/C++**
* **ESP8266 Wi-Fi**
* **Blynk IoT**
* **IoT**
* **I²C Communication**

The project uses Arduino IDE for programming the NodeMCU and Blynk for remote monitoring and control.

```

## 🚀 Getting Started

### 1. Hardware Setup

Connect the ESP8266 NodeMCU with the sensors, relay module, LCD, and buzzer according to the circuit diagram.

### 2. Install Arduino IDE

Install the Arduino IDE and configure the ESP8266 board.

### 3. Install Required Libraries

Install the required libraries:

```text
ESP8266WiFi
Blynk
DHT
LiquidCrystal_I2C
```

### 4. Configure Wi-Fi

Update your Wi-Fi credentials in the Arduino program:

```cpp
char ssid[] = "YOUR_WIFI_NAME";
char pass[] = "YOUR_WIFI_PASSWORD";
```

### 5. Configure Blynk

Add your Blynk Template ID and Authentication Token:

```cpp
#define BLYNK_TEMPLATE_ID "YOUR_TEMPLATE_ID"
#define BLYNK_TEMPLATE_NAME "YOUR_TEMPLATE_NAME"
#define BLYNK_AUTH_TOKEN "YOUR_AUTH_TOKEN"
```

> ⚠️ **Security:** Never upload your real Wi-Fi password or Blynk authentication token to a public GitHub repository.

### 6. Upload the Code

Connect the NodeMCU to your computer, select the correct ESP8266 board and COM port in Arduino IDE, then upload the program.

## 📊 Monitoring

The Blynk application can be used to monitor:

* Temperature
* Humidity
* Gas level
* Water level
* Security/motion status
* Fire detection status

It can also provide notifications when abnormal conditions are detected.

## 🎯 Applications

* 🏠 Smart Home Automation
* 🔐 Home Security and Surveillance
* 🔥 Fire Detection
* 🛢️ Gas Leakage Detection
* 💧 Water Management
* ⚡ Energy Management
* 📱 Remote Monitoring and Control

The project report identifies security, energy management, leak detection, lighting, water management, and remote monitoring as major applications.

## ✅ Advantages

* Low-cost implementation
* Remote accessibility
* Convenient appliance control
* Improved safety and security
* Real-time monitoring
* Energy-efficient operation
* Saves time
* Easy integration with IoT technologies

## 🔮 Future Improvements

The system can be further enhanced by adding:

* Voice-controlled appliances
* Mobile-based automation rules
* AI-based activity detection
* Cloud data logging
* Smart energy-meter monitoring
* Automatic appliance scheduling
* Camera-based security
* Advanced fire and gas safety mechanisms

## 👨‍💻 Project

**Project:** IoT-Based Home Automation System
**Controller:** NodeMCU ESP8266
**Platform:** Blynk IoT
**Programming:** Arduino IDE / Embedded C++
**Domain:** IoT & Embedded Systems

## 📜 License

This project is intended for **educational and academic purposes**.
