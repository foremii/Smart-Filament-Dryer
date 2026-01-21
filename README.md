# Smart-Filament-Dryer
ESPHOME project that automates a 3dprinting Filament dryer using an esp32. This was based around a Polydryer and it's original heater and power supply and maintains the original thermal fuse for safety. 

This uses a Bosch BME688 Temperature, Humidity and Gas sensor for a Climate Thermostat controlling a slow PWM pid controller to a relay for the stock 24V heating element in a PolyDryer. This allows you to data log humidity, temperature or the readings of any sensor you can think of that is compatible with ESPHome if you know how to connect it.

The Fan and Heater stay wired as OEM, but the Relay controls the power for the heater and the 5V regulator provides 5v power for the ESP32 from the 24V factory input. Slow PWM output is limited to 85% to protect the heater, not sure it's really needed. It's takes a while to heat a full 1kg spool up to 140F, but so did the factory one and it helps prevent warping. Once the spool is fully warmed up it helps to unplug the front filament feed hole for about 10min, then close it. It's best to let the spool cool off in a seal vacuum, so put the bottom plugs in to let it cool down. 

Next steps - 
Fan On/Off Control
Fan Tach sensing
Display

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

