# 🚧 Automatic Gate Demo Kit

This project demonstrates an **automatic gate system** using an Arduino Uno, showcasing how a microcontroller makes decisions based on sensor input to control hardware components like a servo motor, LEDs, and a buzzer.

## 📋 Features

- ✅ Detects distance using an **ultrasonic sensor**
- ✅ Opens the gate (servo to 105°) when an object is within **50 cm**
- ✅ Closes the gate (servo to 7°) after **4 seconds** if no object is detected
- ✅ **Red LED ON** when the gate is **closed**
- ✅ **Blue LED ON** when the gate is **open**
- ✅ **Buzzer beeps continuously** while the gate is open (with 40ms ON, 360ms OFF cycle)

## 🧠 Components Used

- Arduino Uno
- HC-SR04 Ultrasonic Sensor
- Servo Motor (SG90)
- Red and Blue LEDs (with cathode wiring)
- Buzzer
- Resistors & Jumper Wires

## 🛠️ How It Works

1. The ultrasonic sensor measures the distance.
2. If an object is detected within 50 cm:
   - The servo rotates to **open** the gate.
   - Red LED turns **OFF**, Blue LED turns **ON**.
   - Buzzer starts **beeping** in short pulses.
3. If no object is detected for 4 seconds:
   - The servo rotates to **close** the gate.
   - Red LED turns **ON**, Blue LED turns **OFF**.
   - Buzzer turns **OFF**.

## 📁 File

- `automatic_gate.ino` – Main Arduino code.

## 📦 Setup Instructions

1. Connect components according to the pin assignments in the code.
2. Upload `automatic_gate.ino` to your Arduino Uno using the Arduino IDE.
3. Power your circuit and observe the gate system behavior.

---

