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

### Simulation Screenshots

```markdown
![Wokwi Simulation](images/wokwi-simulation.png)

![Simulation Website](images/simulation-website.png)
```

### Real-Life Screenshots

```markdown
![Real Circuit](images/real-circuit.jpg)

![Real Website](images/real-website.png)
```

### Videos

```markdown
[Watch the Simulation Video](YOUR_SIMULATION_VIDEO_LINK)

[Watch the Real-Life Demonstration](YOUR_REAL_VIDEO_LINK)
```

## Important Notes

- Do not connect the servo to 3.3V.
- Use 5V or an external regulated 5V supply.
- The servo and ESP32 must share the same ground.
- Each LED should use a 220 Ω resistor.

## Author

**Faris Bahussain**
