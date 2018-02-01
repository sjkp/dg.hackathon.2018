# Wemos D1 
[Wemos D1](https://www.wemos.cc/) is a cheap (5$) ESP-8266 Wifi micro computer, that is arduino compatible, which means there's a lot of sample code to get started with. Since the sensor has Wifi it is fairly easy to get it online and use it for interesting bi-direction communication scenarios. 

The micro computer can be equipped with different sensor shields that allows it to interact with the surrounding world (without them it only has a little blue LED). We have a humidity & temperatur shield, and a few relay shields that can be used turn things on/off. 

A great thing about the Wemos is that you can program it by connecting it to a computer using a USB cable. So you are quicly up and running. 

## Prerequsites
* [Get started tutorial](https://wiki.wemos.cc/tutorials:get_started:get_started_in_arduino)
* [IoT hub Project](https://github.com/delegateas/Arduino-ESP8266-Secure-Http-Azure-IoT-Hub-Client)

### Things you will need to run the project
You need to change the package source in arduino studio to https://wiki.wemos.cc/tutorials:get_started:get_started_in_arduino the guide recommends the git installation, but I find it lot easier just to use the board manager inside arduino studio. 

You have to install this arduino package https://github.com/wemos/WEMOS_DHT12_Arduino_Library (i cannot be found from the package source, afaik, so you have to download it manually)

From the package source you can download `adafruit unified sensor` and the time library by Michael Margolis (there's a lot of libraries that starts with time)

With all this installed you should be able to program the micro computer if you select the right COM port in arduino studio. I have had most success with 115200 as the upload speed. 


## Project Idea
### Sensor Data to IoT Hub
Connect the Wemos Sensor to Azure IoT hub and create and application based on the sensor input. E.g. SMS alerting, or Alexa skill that you can ask to control/read sensor values. 

Bidirectional communication over the IoT hub would be cool, I haven't tried that myself. 