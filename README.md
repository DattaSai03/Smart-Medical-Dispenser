# 📦 Smart Medical Dispenser 🚑

A smart medicine reminder and dispensing system designed using Arduino and a mobile application to help users take medicines on time efficiently and safely.

---

# 📌 Project Overview

The Smart Medical Dispenser is an Arduino-based healthcare system that automates medicine reminders and compartment control using real-time scheduling and Bluetooth communication.

The system uses:

- ⏱️ DS3231 RTC Module for accurate scheduling
- 🔄 Servo Motors for automatic compartment opening
- 🔔 Buzzer + LEDs for medicine alerts
- 📱 HC-05 Bluetooth Module for mobile app connectivity
- 📊 Tablet log tracking system
- 🚨 Emergency call feature

This project demonstrates practical implementation of:

- Embedded Systems
- Arduino Programming
- Mobile App Development
- Smart Healthcare Technology

---

# 🎯 Objectives

- Remind users to take medicines on time
- Automate medicine compartment opening
- Provide missed-dose alerts
- Maintain medicine logs
- Track tablet count
- Enable emergency communication

---

# ✨ Features

- ✔ Automatic compartment opening using servo motors
- ✔ Real-time medicine reminders
- ✔ LED + Buzzer notification system
- ✔ Bluetooth communication with mobile app
- ✔ Tablet log tracking (Taken / Missed)
- ✔ Missed-dose notifications
- ✔ Manual tablet count tracking
- ✔ Emergency call button
- ✔ Mobile app integration
- ✔ Real-time clock scheduling

---

# 🛠️ Hardware Components

| Component | Quantity | Description |
|---|---|---|
| Arduino UNO | 1 | Main controller |
| DS3231 RTC Module | 1 | Real-time clock |
| Servo Motor SG90 | 1–4 | Compartment control |
| HC-05 Bluetooth Module | 1 | Mobile app communication |
| Buzzer | 1 | Audio alerts |
| LEDs | 4 | Slot indicators |
| Push Buttons | 5 | Manual control |
| LCD Display | 1 | Status display |
| Jumper Wires | Multiple | Connections |
| Breadboard | 1 | Circuit assembly |
| Tablet Box | 1 | Medicine storage |
| 5V Power Supply | 1 | System power |

---

# 🔌 System Architecture

The Smart Medical Dispenser is designed using multiple interconnected layers:

## 1. Input Layer
- Medication schedules entered through mobile app
- User commands and emergency inputs

## 2. Processing Layer
- Arduino UNO processes schedules and controls hardware
- RTC module provides accurate timing

## 3. Output Layer
- Servo motors open medicine compartments
- LEDs and buzzer provide alerts
- LCD displays status information

## 4. Communication Layer
- HC-05 Bluetooth module connects Arduino with mobile app

---

# ⚙️ Working Principle

1. RTC module continuously tracks current time.
2. Arduino compares current time with scheduled medicine timings.
3. At scheduled time:
   - Servo motor opens corresponding compartment
   - LED glows
   - Buzzer activates
4. Bluetooth module sends notification to mobile app.
5. User marks medicine as “Taken” or “Missed”.
6. App stores tablet logs.
7. Emergency button initiates phone call to saved contact.

---

# 📱 Mobile App Features

The mobile application was developed using MIT App Inventor.

## App Functions

- Bluetooth Connection
- Medicine Notifications
- Tablet Log Tracking
- Taken / Missed Status
- Tablet Count Tracking
- Emergency Call Button

---

# 🧠 Important MIT App Inventor Blocks

| Component | Function |
|---|---|
| BluetoothClient.ReceiveText | Receives medicine alerts |
| Clock.Timer | Detects missed doses |
| TinyDB | Stores logs |
| PhoneCall.MakePhoneCall | Emergency calling |

---

📸 Screenshots 
<img width="1039" height="652" alt="Screenshot 2026-05-23 112320" src="https://github.com/user-attachments/assets/fcf08d72-1c63-48c5-8d37-fb589448b086" />


<img width="681" height="627" alt="Screenshot 2026-05-23 112810" src="https://github.com/user-attachments/assets/b921037d-802e-4477-abbd-12cd9bf17376" />


<img width="931" height="694" alt="image" src="https://github.com/user-attachments/assets/e610053e-3fa4-4a81-a0fd-43dd98b75821" />



📱 App UI
🛠️ Wiring Diagram
📊 Tablet Log Table
🤖 Prescription Window

# 📂 Repository Structure

```text
Smart-Medical-Dispenser/
│
├── Arduino_Code/
│   └── smart_dispenser.ino
│
├── App/
│   ├── Screenshots/
│   ├── AIA_File/
│   │   └── SmartDispenser.aia
│   └── APK/
│       └── SmartDispenser.apk
│
├── Hardware/
│   ├── Circuit_Diagram.png
│   ├── Component_List.pdf
│   └── Wiring_Guide.pdf
│
└── README.md
```

---

# 🔄 Working Flow

```text
Start
   ↓
RTC Checks Scheduled Time
   ↓
Servo Opens Medicine Compartment
   ↓
LED + Buzzer Alert Activates
   ↓
Bluetooth Notification Sent to App
   ↓
User Selects Taken / Missed
   ↓
App Stores Tablet Log
   ↓
Emergency Calling Feature Available
   ↓
Repeat
```

---

# 💻 Software Used

- Arduino IDE
- MIT App Inventor
- Embedded C++
- Bluetooth Communication
- Wokwi Simulator

---

# 📷 Project Modules

The project includes:

- 📱 Mobile App UI
- 🛠️ Circuit Diagram
- 📊 Tablet Log Table
- 🔌 Wiring Diagram
- 📈 System Flowchart

---

# 🚀 How to Run

## 1️⃣ Upload Arduino Code
Upload the `.ino` file to Arduino UNO.

## 2️⃣ Install Android App
Install the provided APK file.

## 3️⃣ Pair Bluetooth
Connect HC-05 with mobile device.

## 4️⃣ Configure Timings
Set medicine timings in app.

## 5️⃣ Add Emergency Contact
Save emergency phone number.

---

# 📈 Results

The Smart Medical Dispenser successfully automated medicine reminders and compartment control using real-time scheduling. The Bluetooth-connected mobile application effectively tracked tablet logs and missed doses. The system demonstrated stable operation and improved medicine management for users.

---

# 🚀 Future Scope

- Add Wi-Fi based IoT monitoring
- Cloud database integration
- Voice assistant support
- Face recognition authentication
- Caregiver notification system
- Mobile push notifications

---

# 🧩 Skills Used

- Embedded Systems
- Arduino Programming
- Embedded C++
- Bluetooth Communication
- MIT App Inventor
- Sensor Interfacing
- Real-Time Systems
- Smart Healthcare Technology

---

# 👨‍💻 Author

## Srinivas

B.Tech – Electronics and Communication Engineering  
Smart Healthcare & Embedded Systems Developer

---

# 📜 License

MIT License – Owner: Srinivas

---
