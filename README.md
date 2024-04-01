# Project Title: Raspberry Pi Sensor Integration & AI Dashboard

## Overview
This project involves integrating three different sensors with a Raspberry Pi, each employing distinct communication protocols. The collected sensor data is then visualized on a dashboard, along with the integration of an AI model for object detection.

![Project Image](https://github.com/fikrimusa/CDLE-Mini-Project/raw/master/Picture/Project_description.png)

## Installation and Execution Guide

### Prerequisites
- Raspbian Operating System
- Required Hardware Components
- Software Dependencies: Node-RED

### Hardware Components
1. Raspberry Pi 4 Model B 8GB
2. Ultrasonic Sensor (US100)
3. Digital Intensity Sensor (BH1750FVI)
4. Temperature Sensor (TMP36)
5. RPi Approved Phidisk Class10 U1 MicroSD-64GB
6. MCP3008 - 8-Channel 10-Bit ADC With SPI Interface
7. Logitech USB Camera C270 Model
8. USB microSD Card Reader and Writer
9. Raspberry Pi 4 Power Switch Supply Cable USB C
10. Soldering Tools
11. Multimeter

### Software Requirements
1. Raspbian Operating System
2. Node-RED

## Setting Up Raspbian OS

1. **Manual Installation:**
   - Format SD card (FAT32)
   - Use BalenaEtcher to flash Raspbian OS onto the SD card.

2. **Automatic Installation:**
   - Utilize Raspberry Pi Imager for a hassle-free installation process.

3. **Update Raspbian:**
   - Update and upgrade Raspbian by running commands in the terminal.

## Installing Node-RED

1. Execute the provided script to install Node-RED on Raspberry Pi.
2. The script will handle installation, upgrading, and service setup automatically.
3. Utilize provided commands for managing the Node-RED service.

## Object Detection AI Model

- Employed an object detection model based on COCOSSD dataset for real-time object identification.
- Utilizes p5.js framework to display the model's output.

## Dashboard Features

### Real-Time Sensor Data

- Displays sensor readings with gauge, level, and text indicators for temperature, light intensity, and distance respectively.
- Line charts depict sensor readings over time.
- Includes Skymind logo and real-time clock.

### Real-Time Object Detection

- Utilizes p5.js for object detection visualization.
- Embeds the object detection webpage within an iframe for seamless integration.

![Dashboard Image](https://github.com/fikrimusa/CDLE-Mini-Project/raw/master/Picture/Step-by-step (1).png)

Enhanced with detailed installation instructions and clear delineation of features, this project aims to facilitate seamless integration of sensors and AI on Raspberry Pi, providing a comprehensive dashboard for data visualization and analysis.
