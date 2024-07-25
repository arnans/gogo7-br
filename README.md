# gogo7-sesi
Information about the GoGo Board version 7 for use in the SESI project in Brazil

<img src="https://github.com/arnans/gogo7-sesi/blob/main/GoGo%207C.png" width="250">

This repository contains manufacturing and testing information of the GoGo Board Educational Robotics Platform. The GoGo Board is created as a collaboration between  Chiang Mai University in Thailand and Columbia University in New York, USA. The GoGo Board is a physical computing platform with low a learn threshold, allowing learners ages 10 and higher to explore important ideas in STEAM and Computation Thinking. It is perticularly designed for Automation, Internet of Things (IoT), Data Analytics, and Artificail Intelligence (AI).

# Overview 

## The GoGo 7 Hardware

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/GoGo%207C%20Top%201.jpg" width=640>

### Components as shown above

- **Color Display**: 1.8 inch display. Allows basic control and readout of various input and outputs.
- **D-Pad**: A joystick for navigating the screen.
- **USB-C**: Used to supply power and communicate with the programming web application
- **On-Off switch**: Controls the power delivered to the board.
- **Sensor Inputs**: 4 analog sensor input ports
- **Output Ports**: 4 bi-directional ports are available using a JST connector. Each port is capable of driving 1A at 5V. 
- **Servo & Relay Ports**: 4 digital control ports. Can drive Servo Motors or Relays.
- **Extension Ports**: This includes the Multi-device, Configurable, Extension 1, 2, and the Output Extension Bus.

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/GoGo%207C%20Top%202.jpg" width=400>

### Components as shown above

- **Status LEDs**: Shows the run/stop state of the user code.
- **Built-in Sensors**: Digital Microphone (Loudness), IMU (Acceleration & Gyration), Bightness, Proximity
- **Infrared Transmitter and Receiver**

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/GoGo%207C%20Back.jpg" width=500>

### Components as shown above

- **ESP32-S3**: Main CPU. Runs the GoGo Board's operating system and user code.
- **ESP32-C3**: Auxilary CPU. Contains the Tasmota firmware by default. This core has a dedicated USB-C port for flashing the firmware.
- **Boot Buttons**: Used for flasing the corresponding CPUs via the USB-C port. 
- **H-Bridge Drivers, I2C Driver chip**: Used to drive the output ports. They are controlled via the I2C I/O Driver chip.
- **Buzzer**: A Piezo buzzer.
- **Current limiter**: Prevents in-rush current to the the servo motors.
- **I/O Expansion Pins**: Provides expansion capabilities for the GoGo Board
- **5 to 3.3 volt divider**: ADC interface to the CPU.

## The GoGo 7 Programming Environment

<img src="https://github.com/arnans/gogo7-sesi/blob/main/gogo%207%20diagram/code.gogoboard.png" width=800>

This webapplication has the following capabilities:
- [Access via https://code.gogoboard.org](https://code.gogoboard.org)
- Connects to the GoGo Board using USB, Wifi or remote lab.
- Offeres a modern block-based programming.
- Contains cards to monitor and configure various functionalities.
- Cloud storage. Code can be saved and shared on the cloud.
- Learning tools. Data Lab, Classroom, Web UI for remote control and more.

# Manufacturing Information

- [PCB Gerber Files](https://github.com/arnans/gogo7-sesi/blob/main/Gerber_PCB_GoGo_7C_2024-05-18.zip) - The GoGo Board 7 uses a 4-layer PCB.  
- [Pick and Place file](https://github.com/arnans/gogo7-sesi/blob/main/PickAndPlace_PCB_GoGo%207C_2024-05-18.xlsx)
- [Bill of Materials](https://github.com/arnans/gogo7-sesi/blob/main/BOM_GoGo%207_PCB_GoGo%207C_2024-05-18.xlsx)
- Photos: 3D Render [[Top](https://github.com/arnans/gogo7-sesi/blob/main/GoGo%207C%203D%20topview.png) | [Bottom](https://github.com/arnans/gogo7-sesi/blob/main/GoGo%207C%203D%20bottomview.png)] , Assembled board photo [Top | Bottom]
- Firmware: [Main CPU (ESP32-S3)] | [Tasmota Core (ESP32-C3)]
- [Test and QC procedure]

# License

This work is licensed under a Creative Commons Attribution-NonCommercial (CC BY-NC) license. You are free to share, copy, and redistribute the material in any medium or format. However, any commercial use of this work is strictly prohibited without prior written consent from the author.

<img src="https://mirrors.creativecommons.org/presskit/buttons/88x31/png/by-nc.png" width="100">

