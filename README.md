# Smart Soil Moisture Monitoring and Rain Prediction System 🌱

## 📌 Project Overview

The **Smart Soil Moisture Monitoring and Rain Prediction System** is an Arduino-based project concept designed to monitor soil moisture and help determine when plants need watering. It uses a soil moisture sensor and LED indicators to identify dry and adequately moist soil conditions.

The project also proposes plant-specific moisture guidance and weather-based rain prediction to support better irrigation decisions and reduce unnecessary water usage.

> **Project status:** This repository documents the project based on the original presentation. The original source code and physical hardware implementation are not currently available in this repository.

## 🎯 Objectives

- Monitor soil moisture using an analog soil moisture sensor.
- Indicate dry and adequately moist soil conditions using LEDs.
- Encourage efficient water usage through moisture-based decisions.
- Provide plant-specific soil moisture guidance.
- Incorporate weather forecasts and rainfall probability into watering recommendations.

## 🛠️ Hardware Components

| Component | Purpose |
|---|---|
| Arduino Uno | Reads the soil moisture sensor |
| Analog soil moisture sensor | Measures soil moisture level |
| Red LED | Indicates dry soil |
| Green LED | Indicates adequately moist soil |
| 220Ω resistors | Limit LED current |
| Jumper wires | Connect the components |

## 🔌 Circuit Connections

| Component Pin | Arduino Uno Connection |
|---|---|
| Soil sensor AO | A0 |
| Soil sensor VCC | 5V |
| Soil sensor GND | GND |
| Red LED | Digital pin 8 |
| Green LED | Digital pin 9 |

**Note:** The LED connections should include suitable current-limiting resistors.

## ⚙️ Working Principle

1. The soil moisture sensor measures the moisture level in the soil.
2. The Arduino Uno reads the sensor's analog output through pin A0.
3. The reading is compared with a threshold value of **500**, as specified in the original presentation.
4. If the reading is greater than 500, the system indicates dry soil by turning on the red LED.
5. Otherwise, it indicates moist soil by turning on the green LED.

The threshold may need calibration depending on the sensor, soil type, and operating conditions.

## 🌿 Plant-Specific Moisture Guidance

The proposed companion concept provides recommended moisture ranges for different plants.

| Plant | Example Moisture Range |
|---|---:|
| Rose | 400–550 |
| Cactus | 100–250 |
| Basil | 500–650 |
| Wheat | 350–500 |

These are example values from the project presentation, not universally validated moisture requirements. Sensor readings depend on the sensor and soil conditions.

## 🌦️ Rain Prediction Concept

The proposed system can use weather forecasts and rainfall probability to help users decide whether to postpone watering.

Potential recommendations include:
- Water when soil moisture is low and rain is unlikely.
- Consider postponing watering when rainfall is expected.
- Use plant-specific guidance when deciding watering frequency and quantity.

**Implementation note:** A working weather API integration is not included in this documentation repository.

## 🚧 Limitations

- The original source code is not currently available.
- Physical hardware testing and validation are not documented here.
- The basic concept indicates soil conditions using LEDs; it does not directly control a water pump.
- Sensor thresholds require calibration for reliable readings.
- Weather-based recommendations require a suitable forecast data source and software integration.

## 🚀 Future Enhancements

- Automatic water pump control.
- IoT-based remote soil monitoring.
- Mobile notifications for watering recommendations.
- Weather API integration.
- Plant-specific irrigation recommendations.
- Data logging and analysis for improved irrigation decisions.

## 📚 Project Documentation

The original project presentation can be added to the `docs/` folder for reference.

## 👨‍💻 Project Information

**Domain:** Internet of Things (IoT) and Embedded Systems  
**Controller:** Arduino Uno  
**Application:** Smart irrigation and soil moisture monitoring

---

*This repository presents the project's concept, design approach, and proposed improvements for educational and reference purposes.*
