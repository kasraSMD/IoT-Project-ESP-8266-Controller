# IoT-Project-ESP-8266-Controller

<div align="center">

# ⚙️ ESP8266 Controller

**کدهای ساده و کاربردی برای کار با میکروکنترلر ESP8266**

[Overview](#-overview) • [Structure](#-project-structure) • [Getting Started](#-getting-started) • [Collaborators](#-collaborators)

</div>

<br>

## 📍 Overview

This repository provides a simple codebase for multiple functionalities of the ESP8266 microcontroller. It serves as an excellent starting point for beginners who want to understand how to interact with the ESP8266. It has four distinct parts:

| # | Part | Description |
|:-:|------|-------------|
| 1 | **Onboard LED Control** | Control the onboard LED of the ESP8266. |
| 2 | **RGB Sensor** | Interact with an RGB sensor to detect and display colors. |
| 3 | **Django Web Server** | Set up a Django-based web server that allows you to send requests to the ESP8266 and control its functions through a web interface. |
| 4 | **Telegram Bot Integration** | Integrate a Telegram bot for remote control of the ESP8266's functions. |

<br>

## 📂 Project Structure

```text
.
├── README.md
├── report.pdf
├── board-programs-LED/
│   ├── part1-webserver.ino
│   └── part2-client.ino
├── board-programs-RGB/
│   ├── extra-rgb.ino
│   ├── pyserial-3.5.tar.gz
│   └── req.py
├── django_webserver/
└── telegram_bot/
    └── bot.py
```

<br>

## 🚀 Getting Started

> For starting the Onboard LED Control feature, follow these steps:

### 1️⃣ Hardware Setup
Ensure you have an ESP8266 development board, an RGB sensor, and the necessary components for your project. Connect the hardware according to the documentation provided with your components.

### 2️⃣ Software Installation
- Install the Arduino IDE if you haven't already.
- Install the ESP8266 board support package in the Arduino IDE.
- Clone or download this repository to your computer.

### 3️⃣ Upload Code
- Open the Arduino sketch (.ino) file in the Arduino IDE.
- Configure your WiFi network credentials, RGB sensor pins, and other settings in the code.
- Compile and upload the code to your ESP8266 microcontroller.

### 4️⃣ Set Up Django Server
- Navigate to the `django_server` directory.
- Run the Django web server.
- Configure the web server IP address in the [part2-client.ino](./board-programs-LED/part2-client.ino) file.

### 5️⃣ Telegram Bot Integration
- Create a Telegram bot and obtain the API token.
- Configure the bot token in the [bot.py](./telegram_bot/bot.py) file.

### 6️⃣ Access the Web Interface
- If you use ESP8266 as a web server, once the code is uploaded, open the serial monitor to find the ESP8266's IP address. Access the web server by entering this IP address in a web browser to control the functions remotely.
- If you use ESP8266 as a client, access the Django web server by entering its IP address in a web browser to control the functions remotely.

### 7️⃣ Telegram Bot Control
Search for your Telegram bot in the Telegram app and start a chat. Use the Telegram bot commands to control the ESP8266 functions.

<br>

## 🤝 Collaborators

<!-- Add collaborators here -->
