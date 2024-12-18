# PID-Based-Ball-Balancing-System
This project uses a PID control system to balance a ping-pong ball on a servo-controlled beam with a Sharp 2Y0A21 distance sensor. It employs an Arduino Nano for real-time feedback processing and PID tuning, achieving a balance error margin of ±3 mm.

## Features
- PID-controlled ball balancing
- Sharp 2Y0A21 distance sensor for accurate position measurement
- Arduino Nano for real-time feedback processing
- Servo motor control with smooth corrections (20° to 160°)
- System stability with a 50 ms refresh rate

## Hardware Requirements
- Arduino Nano
- Sharp 2Y0A21 distance sensor
- Servo motor
- Power supply
- Ping-pong ball
- Jumper wires & breadboard

## Software Requirements
- Arduino IDE
- Arduino C++ code implementing the PID control

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/mridul-iiitn/PID-Based-Ball-Balancing-System.git
2.Open the project in the Arduino IDE.
3.Connect your Arduino Nano to the computer via USB.
4.Select the correct board and port in the Tools menu of the Arduino IDE.
5.Upload the code to your Arduino Nano.

PID Tuning
The PID constants are pre-calibrated in the code as:

Kp = 8
Ki = 0.2
Kd = 3100
You may adjust these constants to fine-tune the balance system's response.

Working
The Sharp 2Y0A21 sensor continuously measures the position of the ping-pong ball.
The PID controller computes the necessary correction and adjusts the servo motor accordingly to keep the ball balanced within the system’s stable region.
The system operates with a loop frequency of 20 Hz and updates the servo's position every 50 ms.

Acknowledgements
Sharp 2Y0A21 distance sensor for precise distance measurement.
Arduino Nano for easy integration with sensors and servo motors.
