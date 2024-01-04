# ESPHome Inkbird IHT-2PB Temperature Sensor Integration

This project allows you to integrate the Inkbird IHT-2PB temperature sensor with ESPHome, making the temperature data available in Home Assistant.

## Prerequisites

- [Home Assistant](https://www.home-assistant.io/) installed and running.
- [ESPHome](https://esphome.io/) installed and configured.

## Hardware Requirements

- Inkbird IHT-2PB temperature sensor
- An ESP32 board (tested with Espressif32 devkit-v4 and Seeed XIAO ESP32C3)
  - for use with ESP32-C3 (like: [Seeed XIAO ESP32C3](https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html) use the ESP32C3_Inkbird_IHT_2PB.yaml. As this uses the arduino-framework you might run into memory issues (Tested and works fine on Seeed XIAO ESP32C3). Be sure for first time flash to use a usb cable if you change from esp-idf to arduino (issues described [here](https://esphome.io/components/bluetooth_proxy.html?highlight=bluetooth) ).

## Installation

- Copy 'secrets_template.yaml' to 'secrets.yaml' and replace the placeholders by your value
- Use ESPHome command line or dashboard to install

## Data

It provides 4 entities to Home assistant:
- The temperatures of the 3 probes.
- The last probe data that was received.

## References
- https://gitlab.com/sensor-stuff/inkbird-iht-2pb-to-mqtt for the code to enable notification and parse the temperature values.
