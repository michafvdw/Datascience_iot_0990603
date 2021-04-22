# Datascience_iot_0990603!
# IoT measure lux with TSL 2591 using flora microcontroller and bluefruit LE module
![alt text](https://user-images.githubusercontent.com/74900539/115708604-82241700-a370-11eb-9170-b2160a3af96d.png)
This projet measures lux with the TSL 2591 sensor. The data will be send to the bluefruit app on a phone using the bluefruit LE module (a bluetooth module made by adafruit). With the app in UART mode you can check if its dark or light in a room. It will send a message stating it if its dark or not and it also sends the current measured lux. 

## lux
Lux is the SI derived unit of illuminance, measuring luminous flux per unit area. It is used to measure the intensity (as perceived by the human eye) of light that hits or passes a surface. In other words, the TSL 2591 measures the light intensity in a room. 

*Retrieved from: https://en.wikipedia.org/wiki/Lux*

## How to build this project
### Hardware
- Flora microcontroller
- TSL 2591
- Bluefruit LE

### Software
- Arduino IDE
- BluefruitConnect app on your phone (preferably ios)

### Wiring
In the images below is showed how you wire the bluefruit LE and the TSL 2591 to your flora

![alt text](https://user-images.githubusercontent.com/74900539/115710946-3cb51900-a373-11eb-92dd-88ff8ed1b3c5.png)
![alt text](https://user-images.githubusercontent.com/74900539/115711003-4b033500-a373-11eb-9d3b-0ef1d89e1c1b.png)

### Install libraries for the TSL 2591
link: https://learn.adafruit.com/adafruit-tsl2591/wiring-and-test

### Install libraries for the bluefruit LE
Link: https://learn.adafruit.com/adafruit-flora-bluefruit-le/installing-software

### Download BluefruitConnect app
Download the BluefruitConnect app on your phone. You can find this in the ios app store. If you are unsure how to use the app use this link: https://learn.adafruit.com/bluefruit-le-connect

### Download code from this repository 
Besides the libraries you need the code main.ino and BluefruitConfig.h to test this project. They can be found in this repository. Make sure to use this BluefruitConfig.h and not the one from the adafruit library because this one was written specifically for the floram without the project wont work. 

