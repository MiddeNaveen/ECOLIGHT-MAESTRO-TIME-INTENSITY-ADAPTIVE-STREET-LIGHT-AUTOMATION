# ECOLIGHT-MAESTRO-TIME-INTENSITY-ADAPTIVE-STREET-LIGHT-AUTOMATION
The main objective of EcoLight Maestro is to automatically control street lights (LED’s) based on fixed time schedules and real-time ambient light intensity
# EcoLight Maestro – Time & Intensity Adaptive Street Light Automation

EcoLight Maestro is an embedded automation system designed to intelligently control
street lighting based on **Real-Time Clock (RTC) schedules** and **ambient light
intensity**. It enhances power efficiency by dimming or switching off lights when
not required and ensuring proper illumination when needed.

---

## 🎯 Objective

- Automate street lighting without human intervention.
- Control LED street lights using:
  - **Fixed time schedules** via RTC.
  - **Dynamic brightness** using ambient light intensity sensing.
- Improve energy efficiency and system reliability.

---

## 🧩 System Architecture

### ✔️ Functional Overview

1. The system continuously reads **current time** from the RTC.
2. LEDs are controlled according to predefined schedules.
3. A light sensor (LDR) monitors the surrounding light intensity.
4. Based on darkness level:
   - LEDs switch **ON** during night.
   - LEDs **dim** or **switch OFF** when sufficient light exists.
5. The user can modify RTC time using:
   - **4×4 Keypad**
   - **LCD Menu Interface**
6. System validates user input and updates RTC values accordingly.

---

## 🛠️ Hardware Requirements

- LPC2148 ARM7 Microcontroller
- RTC Module
- 16x2 LCD Display
- 4×4 Keypad
- LDR / Light Sensor
- LED Street Light Array
- Power Supply
- Driver Circuit / Transistors
- Supporting Resistors & Components

---

## 🧾 Software Requirements

- Keil uVision IDE
- Flash Magic (Programming Tool)
- Embedded C
- Proteus (Optional – Simulation)

---

## 🗂️ Project Workflow

1. **System Initialization**
   - LCD is initialized
   - RTC is configured
   - Ports and peripherals are set

2. **Main Control Loop**
   - Continuously reads:
     - RTC (Hour, Minute, Second, Date, Month, Year)
     - LDR analog value

3. **Decision Logic**
   - If time matches configured schedule → control LEDs
   - If darkness detected → LEDs ON
   - If sufficient light → LEDs OFF / Dim

4. **User Interaction**
   - LCD displays Main Menu:
     - `1. Edit RTC Info`
     - `2. Exit`
   - If Edit selected:
     - Modify:
       - Hour
       - Minute
       - Second
       - Day
       - Date
       - Month
       - Year
   - Input validation:
     - Hours → 0–23
     - Minutes/Seconds → 0–59
     - Date validity based on Month & Leap Year
   - Invalid inputs show error message
   - Valid inputs update RTC
   - User exits menu → LCD confirms RTC Updated

---

## 📟 LCD Display Interface

- Displays live system status
- Shows real-time clock
- Provides menu navigation
- Displays error / confirmation messages

---

## 🎛️ Keypad Functions

- Navigate menu
- Edit RTC fields
- Confirm / Cancel inputs

---

## 🔌 LED Control Logic

- LEDs controlled via GPIO pins
- Brightness / ON-OFF based on:
  - Time conditions
  - Light intensity values

---

## ✔️ Key Features

- Fully automated
- Time-based scheduling
- Ambient-light adaptive control
- User-configurable RTC
- Input validation for reliability
- LCD guided user interface

---

## 🚀 Applications

- Smart City Projects
- Highway Street Lighting
- College / University Projects
- Industrial Automation
- Public Illumination Systems

---

## 👨‍💻 Developed Using

- Embedded C
- ARM7 Microcontroller
- Keil µVision
- Flash Magic
- Proteus Simulation (optional)

---

## ✅ Conclusion

EcoLight Maestro provides an efficient, automated, and adaptive
street lighting solution by utilizing real-time clock scheduling
and ambient light sensing. The system reduces power wastage,
improves lifespan of street lights, and supports smart-infrastructure
development.

---

### ⭐ Thank You
