# 8051-based-smart-parking-system-
# 🚗 Smart Parking System using 8051

## 📌 Overview
This project implements a microcontroller-based smart parking system using the AT89C51 (8051). It automates vehicle entry and exit by controlling a gate mechanism based on sensor inputs. The system processes entry and exit signals, operates a motor through a driver circuit, and manages parking slot availability.

The project is designed and simulated in Proteus, with control logic developed using Embedded C in Keil µVision.

---

## 🎯 Objectives
- Automate parking gate control
- Detect vehicle entry and exit
- Control motor direction using a driver IC
- Demonstrate embedded system integration

---

## ⚙️ Features
- Automatic gate opening and closing
- Entry and exit detection using sensors
- Motor control using driver IC
- LED indication for system status
- Simple parking slot management logic

---

## 🧩 Components Used
- AT89C51 Microcontroller
- ULN2003A Motor Driver / L293D (depending on setup)
- DC Motor (Gate mechanism)
- Crystal Oscillator (11.0592 MHz)
- Capacitors (33pF, 10µF)
- Resistors (10kΩ, 220Ω)
- LED Indicator
- LogicState (for sensor simulation)
- Power Supply (5V)

---

## 🔧 Circuit Description
The AT89C51 microcontroller acts as the central processing unit. Entry and exit sensors are connected to Port 1 pins and provide input signals to the controller.

The microcontroller processes these signals and generates output through Port 2, which is connected to a motor driver IC (ULN2003A or L293D). The driver amplifies the current and drives the DC motor.

The motor simulates a gate mechanism, rotating to represent opening and closing of the parking gate. An LED is used to indicate system activity.

---

## ⚙️ Working Principle
1. When the entry sensor is activated:
   - The microcontroller checks slot availability
   - Gate opens (motor rotates)
   - Slot count decreases

2. When the exit sensor is activated:
   - Gate opens again
   - Slot count increases

3. The motor driver controls direction:
   - Forward → Gate opens
   - Reverse → Gate closes

---

## 💻 Software Used
- Proteus Design Suite (Simulation)
- Keil µVision (Code development)
- Embedded C (Programming language)

---

## ▶️ How to Run the Project
1. Open the Proteus file (`.pdsprj`)
2. Load the HEX file into the AT89C51
3. Ensure clock frequency is set to 11.0592 MHz
4. Run the simulation
5. Toggle entry/exit inputs to observe motor operation

---

## 📸 Output
- Motor rotates to simulate gate opening and closing
- LED indicates system activity
- Entry and exit signals control system behavior

---

## 🚀 Future Improvements
- Add LCD display for slot count
- Use real IR sensors instead of logic inputs
- Implement IoT-based monitoring system
- Add automatic timing for gate closing

---

## 📚 Applications
- Shopping mall parking systems
- Toll gates
- Residential parking automation
- Smart city infrastructure

---

## 🏁 Conclusion
The project successfully demonstrates the implementation of an automated parking system using a microcontroller. It integrates sensing, processing, and actuation to control gate operation efficiently, reducing manual effort and improving system reliability.

---

