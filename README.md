Gesture Controlled Robotic Arm using ESP32 & IMU (ESP-NOW)
This project implements a wireless gesture-controlled 3-axis robotic arm using an IMU mounted on the user’s wrist. Motion data is processed on an ESP32, filtered, mapped to servo angles, and transmitted via ESP-NOW to a receiver ESP32 controlling the arm.

Low latency. Smooth motion. Real-time mapping.

##System Architecture

Transmitter (Glove/Wrist Unit)
MPU6050 IMU
ESP32
Low-pass filtering
Angle mapping
ESP-NOW broadcast
Receiver (Robotic Arm Unit)
ESP32
Servo motors (3 DOF)
Smooth interpolation control

##Hardware Used##

ESP32 (x2)
MPU6050 IMU
3x Servo Motors
External 5–6V servo power supply
Common ground between ESP32 & servo supply

⚠️ Important: Do NOT power servos directly from ESP32 5V pin.

##Communication##

Protocol: ESP-NOW
Latency: ~10–20ms typical
Peer-to-peer communication
