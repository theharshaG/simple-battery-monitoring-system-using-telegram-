# simple-battery-monitoring-system-using-telegram

ESP32 Battery Monitoring System (IoT Project)
## Overview

This project is an IoT-based Battery Monitoring System using ESP32. It reads battery voltage using an analog sensor and sends real-time updates to a Telegram bot. The system notifies the user about battery status (Full, Medium, Low) and sends alerts when voltage changes or reaches a low level.

## Features

Real-time battery voltage monitoring
Send data to Telegram bot
Battery status detection (Full, Medium, Low)
Automatic alerts on voltage change
Periodic updates (every 1 minute)
Low battery warning system

## Technologies Used

ESP32 (Arduino IDE)
WiFi module
HTTPClient library
Telegram Bot API
Analog voltage sensor

## Project Structure

esp32-battery-monitor-telegram/
│
├── main.ino
└── README.md

## How to Run

install Arduino IDE
Install ESP32 board support
Update WiFi credentials in code
Add Telegram bot token and chat ID
Upload code to ESP32

## How It Works

ESP32 connects to WiFi network

Voltage is read from analog pin (GPIO 34)
Analog value is converted into actual voltage

Battery status is determined based on voltage levels:
Above 12.5V → Full
Between 11.5V and 12.5V → Medium
Below 11.5V → Low

The system sends data to Telegram using HTTP request

Messages are sent when:
Voltage changes significantly
Time interval (1 minute) is reached

If battery is low:
Immediate alert is sent

## Future Improvements

Add solar charging integration
Store data in cloud database
Add web dashboard for monitoring
Use secure HTTPS certificate instead of insecure client
Add mobile app interface
Improve voltage calibration

## Author
Harsha G
Learning Python | Embedded Syste
