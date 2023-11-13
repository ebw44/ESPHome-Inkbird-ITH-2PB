# ESPHome Inkbird IHT-2PB Temperature Sensor Integration

This project allows you to integrate the Inkbird IHT-2PB temperature sensor with ESPHome, making the temperature data available in Home Assistant.

## Prerequisites

- [Home Assistant](https://www.home-assistant.io/) installed and running.
- [ESPHome](https://esphome.io/) installed and configured.

## Hardware Requirements

- Inkbird IHT-2PB temperature sensor
- An ESP32 board (tested with Espressif32 devkit-v4)

## Installation

- Copy 'secrets_template.yaml' to 'secrets.yaml' and replace the placeholders by your value
- Use ESPHome command line or dashboard to install

## Data

It provides 4 entities to Home assistant:
- The temperatures of the 3 probes.
- The last probe data that was received.

## References
- https://gitlab.com/sensor-stuff/inkbird-iht-2pb-to-mqtt for the code to enable notification and parse the temperature values.
