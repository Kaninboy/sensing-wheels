<div align="center">
  <a href="https://github.com/Kaninboy/sensing-wheels">
    <img src="/logo.png" alt="Logo" width="140" height="80">
  </a>
<h3 align="center">Sensing Wheels</h3>
  <p align="center">
    Make Riding Journey <b>SAFE</b>
  </p>
</div>

## Introduction
Sensing Wheels is an IoT-based smart bike safety system designed to improve the cycling experience by enhancing rider safety through sensor-based monitoring and control. 
The system integrates various sensors such as gyroscope, thermometer, ultrasonic sensor, and light sensor, to detect potential hazards and respond to environmental changes. 
The goal is to help cyclists avoid accidents, manage instability, and ride safely in varying conditions such as low light, high temperature, and close proximity to obstacles.

This project is a part of the course 2147336 Internet of Things

## Demo Video

https://github.com/user-attachments/assets/a92c75ce-c58a-4fe6-a0bb-2ba09f3b745f




## Features
- **Automatic Light Detection**: The front light of the bicycle turns on automatically when ambient light is low, using the BH1750 light sensor.
- **Obstacles Detection**: The ultrasonic sensor (SR04) detects obstacles and vehicles and triggers a warning light and sound if they are too close.
- **Tilt Detection**: The gyroscope (MPU6050) detects instability and tilts, triggering alert lights and warning sounds when the bike tilts beyond safe angles.
- **Heat Detection**: The temperature sensor in the MPU6050 detects if the temperature exceeds 32°C and triggers an alert to avoid heatstroke.
- **Real-Time Monitoring**: Outputs sensor data via UART for real-time monitoring of temperature, light, distance, and tilt angles.

## Hardware List
- STM32 Microcontroller (NUCLEO-F411RE)
- Ultrasonic Sensor (HC-SR04)
- Lux Sensor (BH1750)
- Temperature Sensor (MPU6050)
- Gyroscope (MPU6050)
- Breadboard and wires
- LED/Traffic Lights
- Buzzer

## Prerequisites
- **STM32CubeIDE**: Download and install the IDE from the [official STM32CubeIDE page](https://www.st.com/en/development-tools/stm32cubeide.html).

## Libraries Used
The following libraries are used in the Sensing Wheels project to interface with the various sensors:

1. **MPU6050**: For gyroscope and temperature readings from the MPU6050 sensor.
2. **BH1750**: For light intensity measurements from the BH1750 sensor.
3. **SR04**: [ashkorehennessy/sr04](https://github.com/ashkorehennessy/sr04) For distance measurements using the HC-SR04 ultrasonic sensor.

## Installation
1. Clone the repository into the **STM32CubeIDE** workspace.

```bash
git clone https://github.com/Kaninboy/sensing-wheels.git
```

2. Click 'Open Projects from File System' to import the project
3. Set up the hardware
4. Click 'Run' to run the project
5. Observe the results

## Our Team!
- Rujapa Wasanasongchusakul
- Ravit Chutivisuth
- Tunyagorn Siriariyasub
- Thammathat Sarasinpitak
- Thanayut Tiratatri
- Kanin Sukittivarapunt
