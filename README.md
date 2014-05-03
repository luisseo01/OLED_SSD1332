OLED_SSD1332
============
This it's a Hyper Fast library for drive solomon tech SSD1332 OLED displays. It's compatible with Arduino, Arduino DUE and Teensy 3.x and uses native SPI.
The features are:
 - Hyper Fast speed. On Teensy 3.x it uses SPI DMA at 24Mhz.
 - Compatible with Adafruit protocol, it uses Adafruit GFX library and it's fully supported.
 - Works with serial SPI protocol so only 5 or 4 pin are needed (2 of them still shareable).
 - Massive use of hardware accellerated commands for SSD chip.


Version History:
 - 0.5b1: First working release with full tested 24Mhz/DMA SPI on Teensy 3.
 - 
 
Here's the library in action with Teensy3.

[![Video](https://github.com/sumotoy/OLED_SSD1332/blob/master/Docs/CIMG6538.JPG)](https://www.youtube.com/watch?v=jM31tLOtBT4)

Here's the connection for SPI with a module found on ebay:

![image](http://i1189.photobucket.com/albums/z437/theamra/03c4fefe-7e34-4f7d-b710-67a1f05cb7eb.jpg "ssd1332")<br>

Do not use the 3V3 supply on this module, due a strange design the 3V3 pin will not drive correctly the internal higher voltage converter for the OLED so use the 5V pin.
You can safely drive this OLED module with Teensy3 since the module accept 3V3 correctly and I don't use any input on MCU.
Note that this module it's not configured for SPI as default so probably you need to set BS1 and BS0 jumper onboard to 0 (as showed).

Please wait I publish more data before use it. It will happen in max a couple of days.
