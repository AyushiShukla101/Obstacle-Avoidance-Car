# 🤖 Obstacle Avoidance Robot Car using Ultrasonic Sensor

This is an autonomous robot car that detects and avoids obstacles using an ultrasonic sensor. It uses a simple decision-making algorithm to change direction when an obstacle is detected within a threshold distance.

---

## 🚗 Features
- Detects obstacles in real-time using an ultrasonic sensor (HC-SR04)
- Avoids collisions by turning away from detected obstacles
- Controlled by a microcontroller (Arduino Uno or similar)
- DC motors driven via L298N/L293D motor driver
- Serial Monitor output for distance readings

---

## 🛠️ Components Used

| Component             | Quantity |
|----------------------|----------|
| Arduino Uno/Nano     | 1        |
| HC-SR04 Ultrasonic Sensor | 1   |
| L298N or L293D Motor Driver | 1  |
| DC Motors with Wheels| 2        |
| Robot Car Chassis    | 1        |
| Jumper Wires         | As needed|
| Battery (9V or 12V pack) | 1    |

---

## 🔌 Circuit Connections

- **Ultrasonic Sensor**
  - Trig ➡️ Pin 9
  - Echo ➡️ Pin 10

- **Motor Driver**
  - Motor A ➡️ Pins 2 & 3 (Left Motor)
  - Motor B ➡️ Pins 4 & 5 (Right Motor)

- Power supply connected to motor driver and Arduino.

---

## 💻 Code Overview

### 🔹 Main Logic:
- Move forward if the path is clear (distance > 15 cm)
- Stop and turn if an obstacle is detected closer than 15 cm

### 🔹 Core Functions:
- `getDistance()` - Measures distance using ultrasonic sensor
- `moveForward()`, `stopCar()`, `turnLeft()`, `turnRight()` - Control motor movement

---


