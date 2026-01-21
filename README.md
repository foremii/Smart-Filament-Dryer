# Smart-Filament-Dryer
ESPHOME project that automates a 3dprinting Filament dryer using an esp32. This was based around a Polydryer and it's original heater and power supply and maintains the original thermal fuse for safety. 

This uses a Bosch BME688 Temperature, Humidity and Gas sensor for a Climate Thermostat controlling a slow PWM pid controller to a relay for the stock 24V heating element in a PolyDryer. This allows you to data log humididy, temperature or the readings of any sensor you can think of that is compatible with ESPHome if you know how to connect it.
![Alt text](thermostat.png?raw=true "Thermostat")

# BOM
ESP32 Board
https://www.adafruit.com/product/5691

BME688 Temp/Humidity/Gas Sensor
https://www.adafruit.com/product/5046

5V Regulator to power ESP32
https://www.adafruit.com/product/1065

Relay for Heater
https://www.adafruit.com/product/3191

Fan Controller to monitor Fan
https://www.adafruit.com/product/4808

