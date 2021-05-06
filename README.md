# OpenWeather32
Open Source ESP32 based weather and air quality station, designed around sensors supported by ESPHome

![GitHub](https://img.shields.io/github/license/adub08/OpenWeather32) ![GitHub last commit](https://img.shields.io/github/last-commit/adub08/OpenWeather32)
# What?
OpenWeather32 is designed to be a flexible DIY friendly weather and air quality monitoring system (with many additional features!)

# Features: 
- DIY friendly thru-hole design with most pins labelled 
- Based around a NodeMCU ESP32 & designed to work with ESPHome
- Battery monitoring using Vin voltage divider 
- 5V OR 6.5 - 32V DC input (when populated with TSR12450)
- Optional dedicated Voltage regulator for QWIIC/Grove i2c bus for a high number of QWIIC devices
- QWIIC compatible (Dedicated i2c Bus-A)
- Grove compatible (Dedicated i2c Bus-A)
- Mosfet controlled pump or solenoid output
- RJ-11 (or 2.54 dupoint) Rain guage and anemometer inputs **[Untested]**
- 5 spare GPIO pins (5 support ADC functions, 2 support DAC, 3 support capacitive touch)

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
- Any QWIIC or Grove compatible sensor board

**PCB Design Features**
- All 2.54 headers placed on a 2.54mm grid for easy soldering 
- Beginner friendly all thru hole soldering (minus the QWIIC connector)

# Why?
Although there are many other open source weather stations out there, not many are based around the ESP32 and most are just weather stations without any air quality or soil moisture sensing capabilities. There also seemed to be a huge lack of any designed around sensors supported by ESPHome I also wanted it to be flexible enough for most people's needs (which is why the variety of connector headers).

# How to use it?
I've exported the gerbers and odb++ files for the PCB layout, to make it just upload these files to your favourite PCB fab. I made the PCB 100x100mm, 2 layers, so that it would be suitable for being produced at dirtyPCB as a prototype run. If you wish to edit the PCB i suggest using diptrace, which is what i used to make this, the PCB is well within the limitations of the free version of DipTrace. I have also included an eagle .brd but i can't speak for the usability of this file since it's exported from DipTrace.

The esphome yaml config has been included but you will almost certainly need to change i2c addresses to match the individual sensor boards used along with wifi and device details.


# Render & Photos:
**Render of the Revision 1.1 board**
![TOP - Render](https://user-images.githubusercontent.com/20442610/116513412-1f94c300-a8fc-11eb-8c42-d6f277ac053c.PNG)
![Bottom - Render](https://user-images.githubusercontent.com/20442610/116962627-111e2100-acd9-11eb-8ab0-24e9d59bfa34.PNG)

**Photos of the Revision 1.0 board**
![Board](https://user-images.githubusercontent.com/20442610/116514205-4acbe200-a8fd-11eb-8ee6-03e759af5f3b.jpg)
![Board](https://user-images.githubusercontent.com/20442610/116515415-da25c500-a8fe-11eb-9569-b1468a5386dc.jpg)

# How to help:
If you like to say thanks for the design, feel free to use my dirtypcb shares link when ordering.
https://dirtypcbs.com/store/designer/details/a_dub/6520/openweather32
In the future i may also sell single boards on Tindie. 

# Disclaimer:
**The Eagle file is an export from diptrace, i have no idea how good an export it is**I have not tested all features on this PCB yet, inparticular the wind and rain meters. I also have not tested the adafruit BME280 & The SparkFun AS3935 header. **Check Board layout and if headers are suitable before use. I Make no promises about anything being correct!**

**Enjoy!**
