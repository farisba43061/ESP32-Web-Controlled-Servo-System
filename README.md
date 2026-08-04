# ESP32 Servo Web Controller

This project uses an ESP32 to control a servo motor through a local web page. The ESP32 creates its own Wi-Fi network, so the system works without an internet connection.

## Features

- Web-controlled servo
- OPEN and CLOSE buttons
- Red and green status LEDs
- Modern mobile-friendly website
- Current system status display

## Components

- ESP32
- Servo motor
- Red LED
- Green LED
- Two 220 Ω resistors
- Breadboard and jumper wires
- USB cable

## Connections

| Component | ESP32 Pin |
|---|---|
| Servo signal | GPIO 22 |
| Green LED | GPIO 21 |
| Red LED | GPIO 16 |
| Servo power | 5V |
| Servo ground | GND |

## Required Library

Install:

```text
ESP32Servo
```

## Wi-Fi Details

```text
Network: ESP32-Servo
Password: 12345678
Website: http://192.168.4.1
```

## How It Works

### OPEN

- Servo moves to 90°
- Red LED turns on
- Green LED turns off
- Website status becomes `OPEN`

### CLOSE

- Servo moves to 0°
- Green LED turns on
- Red LED turns off
- Website status becomes `CLOSED`

## Project Media

### circuit

<img width="1600" height="900" alt="WhatsApp Image 2026-08-04 at 5 33 17 AM" src="https://github.com/user-attachments/assets/3e289af2-cdf4-454d-8da8-c0dcf82bb92c" />



### Video


https://github.com/user-attachments/assets/e9e15f2c-d26f-4ffa-aea3-6cf30720d5ca



## Important Notes

- Do not connect the servo to 3.3V.
- Use 5V or an external regulated 5V supply.
- The servo and ESP32 must share the same ground.
- Each LED should use a 220 Ω resistor.

## Author

**Faris Bahussain**
