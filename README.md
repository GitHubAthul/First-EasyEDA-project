# Temperature Sensor Characterization System

## Project Overview

This project focuses on the **design and development of a microcontroller-based system** to **measure, compare, and characterize different temperature sensors** over a controlled temperature range. The system evaluates sensor accuracy, response, and stability using a **calibrated digital temperature sensor (DS18B20)** as a reference.

---

## Objectives

* Measure and compare temperature readings from:

  * RTD (PT100)
  * NTC Thermistor (10kΩ)
  * K-type Thermocouple
* Use **DS18B20** as a reference temperature sensor
* Maintain controlled temperature conditions using **heating and cooling modules**
* Display real-time temperature data and system status
* Enable debugging and data logging via USB-to-UART

---

## System Specifications

### Power Supply

* Input: **12V, 10A SMPS**
* Regulated Outputs:

  * **5V** for logic and peripherals
  * **3.3V** for sensors (where required)

### Microcontroller

* **ATmega328P**
* Support circuits:

  * 16 MHz crystal oscillator
  * Reset circuit
  * Decoupling capacitors

---

## Sensor Interfaces

| Sensor Type          | Interface Details                  |
| -------------------- | ---------------------------------- |
| RTD (PT100)          | Signal conditioning with amplifier |
| NTC Thermistor (10k) | Voltage divider + ADC              |
| K-type Thermocouple  | Amplifier-based interface          |
| DS18B20              | 1-Wire digital interface           |

---

## Temperature Control

* **Resistive Heater** for heating
* **Peltier Module** for cooling
* Control using **two relay modules**
* Operational range: **10°C – 80°C**

---

## User Interface

* **20×4 LCD Display**

  * Sensor temperatures
  * System status
  * Control messages
* **Push Buttons**

  * 3 navigation/menu buttons
  * 1 reset button
* **LED Indicators**

  * Power
  * Heating
  * Cooling
  * Error
* **Audible Alert**

  * 5V buzzer for threshold alerts and faults

---

## Communication Interface

* **USB-to-UART bridge** (CH340G / FT232)
* Used for:

  * Debugging
  * Serial monitoring
  * Data logging

---

## Firmware Features

* Sensor data acquisition
* ADC processing
* Relay control logic
* LCD updates
* Button handling
* UART communication
* Error detection and alerts

---

## Testing & Validation

* Individual subsystem testing
* Temperature response validation
* Accuracy comparison against reference sensor
* Heating and cooling performance analysis

---

## Tools 

* **EDA:** EasyEDA
* **PCB Fabrication:** JLCPCB, Lion Circuits

---

## License

This project is intended for **academic and educational purposes**.

---

## Acknowledgment

This project was carried out as part of the **Summer Internship Program on Cyber Physical Systems**,
Department of **Electronics & Communication Engineering**,
**Government Engineering College Thrissur**.

---
