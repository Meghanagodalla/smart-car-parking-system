# smart-car-parking-system

## Overview
This project is an Arduino-based Smart Parking System that automates vehicle entry and exit using IR sensors, a servo motor, and a 16×2 I2C LCD. It displays the number of available parking slots in real time and prevents entry when the parking lot is full.

## Features
- Automatic vehicle detection using IR sensors
- Servo motor-controlled parking gate
- Real-time parking slot display
- Displays "Parking Full" when no slots are available
- Simple and low-cost automation solution

## Components Used
- Arduino Uno
- 16×2 I2C LCD
- Servo Motor
- 2 IR Sensors
- Jumper Wires
- Breadboard

## Circuit Connections
| Component | Arduino Pin |
|-----------|-------------|
| IR Sensor 1 | D2 |
| IR Sensor 2 | D3 |
| Servo Motor | D4 |
| LCD SDA | A4 |
| LCD SCL | A5 |

## Working
1. The entry IR sensor detects an incoming vehicle.
2. If a parking slot is available, the servo motor opens the gate.
3. The available slot count decreases by one.
4. If the parking lot is full, the gate remains closed and the LCD displays **"Parking Full"**.
5. When a vehicle exits, the exit sensor detects it, the gate opens, and the slot count increases.

## How to Run
1. Connect all components as per the circuit.
2. Upload the Arduino code using the Arduino IDE.
3. Power the Arduino board.
4. Monitor the LCD for available parking slots.

## Future Improvements
- RFID-based vehicle authentication
- IoT monitoring using ESP8266/ESP32
- Mobile application integration
- Cloud-based parking management

## Author
**Meghana**
