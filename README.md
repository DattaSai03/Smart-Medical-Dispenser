
📦 SMART MEDICAL DISPENSER — IoT + AI + Arduino + Mobile App
🚑 A smart pill-reminder device with automatic lid opening, AI prescription assistant, missed-dose alerts, tablet count tracking & emergency calling.
⭐ Project Overview

The Smart Medical Dispenser is an Arduino-based system designed to help patients take medicines on time.
It uses:

⏱️ RTC (DS3231) for accurate time

🔄 Servo motors to open compartments

🔔 Buzzer + LEDs for alerts

📱 Bluetooth (HC-05) to sync with a mobile app

🤖 AI API for mini tablet prescription

📊 Tablet-log table inside app

🚨 Emergency Call button

📁 Repository Structure
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
├── AI_Backend/
│   └── prescription_api_example.py
│
├── Hardware/
│   ├── Circuit_Diagram.png
│   ├── Component_List.pdf
│   └── Wiring_Guide.pdf
│
└── README.md

🛠️ Hardware Components
Component	Qty	Description
Arduino UNO	1	Main controller
DS3231 RTC	1	Real-time clock
Servo SG90	1–4	Compartment opening
HC-05 Bluetooth	1	App communication
Buzzer	1	Alerts
LEDs	4	Slot indicators
Jumper wires	1 set	Connections
Tablet box	1	Container
5V/2A power supply	1	Servos and Arduino
🧩 Features
✔ Automatic compartment opening via servo
✔ LED + Buzzer pill-time notification
✔ Bluetooth message to mobile app
✔ AI-generated mini-prescription
✔ Tablet logs (taken/missed) table
✔ Alerts for missed doses
✔ Manual tablet count tracking
✔ Emergency call button

📱 Mobile App (MIT App Inventor)
App Features:

Bluetooth Connect

Pill-time popup

“Taken” / “Missed” buttons

Tablet count tracker

Table log (Name, Time, Status)

AI prescription window

Emergency call button

Important Blocks:

BluetoothClient.ReceiveText → Display tablet alert

Clock.Timer → Missed dose detection

TinyDB → Store logs

PhoneCall.MakePhoneCall → Emergency calling

Web Component → AI API call

🤖 AI Mini Prescription (Python API Example)

AI_Backend/prescription_api_example.py

import openai

openai.api_key = "YOUR_API_KEY"

query = "Give a short prescription summary of Paracetamol 500mg"

response = openai.ChatCompletion.create(
    model="gpt-4o-mini",
    messages=[{"role": "user", "content": query}]
)

print(response["choices"][0]["message"]["content"])

🔄 Working Flow
Step	Action
1	RTC matches the scheduled time
2	Servo opens compartment
3	LED + buzzer alert
4	Message sent to app via Bluetooth
5	App logs “Taken” or “Missed”
6	If missed → app sends notification
7	AI module shows prescription
8	Emergency button calls saved number
📸 Screenshots 
<img width="1039" height="652" alt="Screenshot 2026-05-23 112320" src="https://github.com/user-attachments/assets/fcf08d72-1c63-48c5-8d37-fb589448b086" />


<img width="681" height="627" alt="Screenshot 2026-05-23 112810" src="https://github.com/user-attachments/assets/b921037d-802e-4477-abbd-12cd9bf17376" />


<img width="931" height="694" alt="image" src="https://github.com/user-attachments/assets/e610053e-3fa4-4a81-a0fd-43dd98b75821" />



📱 App UI
🛠️ Wiring Diagram
📊 Tablet Log Table
🤖 Prescription Window

🚀 How to Run
1️⃣ Upload the Arduino .ino file to Uno
2️⃣ Install App (.apk) on Android
3️⃣ Pair HC-05 Bluetooth
4️⃣ Set tablet timings in the app
5️⃣ Enter emergency number
6️⃣ Test AI prescription feature
📜 License

MIT License – Owner: Srinivas

🧑‍💻 Author

Srinivas
B.Tech ECE
Smart Healthcare & Embedded AI Developer
