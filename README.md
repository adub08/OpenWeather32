# OpenWeather32
Open Source ESP32 based weather and air quality station, designed around sensors supported by esphome

![GitHub](https://img.shields.io/github/license/adub08/OpenWeather32) ![GitHub last commit](https://img.shields.io/github/last-commit/adub08/OpenWeather32) ![GitHub repo file count](https://img.shields.io/github/directory-file-count/adub08/OpenWeather32)
# What?
OpenWeather32 is designed to be a flexible DIY friendly weather and air quality monitoring system (with many additional features!)

# Features: 
- DIY friendly thru-hole design with most pins labelled 
- Based around a NodeMCU ESP32
- Designed to work with ESPHOME
- 5V OR 6.5 - 32V DC input (when populated with TSR12450)
- QWIIC compatible (Dedicated i2c Bus-A)
- Grove compatible (Dedicated i2c Bus-A)
- Mosfet controlled pump or solenoid output
- RJ-11 (or 2.54 dupoint) Rain guage and anemometer
**Supported Sensors:**
- Supports a wide variety of temperature and humidity sensors including:
  - BME280 (Adafruit or other pin-outs)
  - AM2303 (otherwise known as the DHT22)
  - SI7021
- Support the CCS811 CO2 and VOC (volatile organic compound) sensor
- Supports the SDS011 particulate Matter Sensor
- Supports the BH1750 Ambient Light Sensor
- AMS AS3935 Franklin Lightning Sensor [Connected via SPI]
- Four capacitive soil moisture sensors 
