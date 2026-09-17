# Smart Guard Alert Device

An IoT-based emergency alert system using **NodeMCU (ESP8266), GPS, and Telegram** to send emergency notifications along with the user's location.

## Project Overview

The Smart Guard Alert Device is designed to provide a quick and simple way to send emergency alerts during critical situations.

When the user presses an emergency button, the NodeMCU ESP8266 processes the input, obtains location information from the GPS module, and sends an emergency notification through Telegram.

The system is designed for applications such as campus safety, personal security, and emergency assistance.

## Key Features

- Emergency alert using physical push buttons
- Police and Medical emergency options
- GPS-based location information
- Telegram-based emergency notifications
- ESP8266 Wi-Fi connectivity
- Fast communication during emergency situations
- Simple and low-cost hardware implementation

## Hardware Components

- NodeMCU ESP8266
- NEO-6M GPS Module
- Push Buttons
- Breadboard
- Jumper Wires
- USB Cable

## Software & Technologies

- Arduino IDE
- C/C++ programming
- ESP8266
- GPS communication
- Telegram Bot API
- Serial communication
- GPIO

## System Architecture

```text
          ┌──────────────────┐
          │  Emergency       │
          │  Buttons         │
          │ Police / Medical │
          └────────┬─────────┘
                   │
                   ▼
          ┌──────────────────┐
          │   NodeMCU        │
          │   ESP8266        │
          │                  │
          │ GPIO Processing  │
          │ Decision Making  │
          └───────┬──────────┘
                  │
          ┌───────┴──────────┐
          │                  │
          ▼                  ▼
   ┌──────────────┐   ┌───────────────┐
   │  NEO-6M GPS  │   │   Wi-Fi /     │
   │              │   │   Telegram    │
   └──────────────┘   └───────┬───────┘
                               │
                               ▼
                      ┌────────────────┐
                      │ Emergency      │
                      │ Alert Message  │
                      │ + Location     │
                      └────────────────┘
