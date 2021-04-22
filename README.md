# Datascience_iot_0990603!
# IoT measure lux with TSL 2591 using flora microcontroller and bluefruit LE module
![alt text](https://user-images.githubusercontent.com/74900539/115708604-82241700-a370-11eb-9170-b2160a3af96d.png)
This project measures lux with the TSL 2591 sensor. The data will be send to the bluefruit app on a phone using the bluefruit LE module (a bluetooth module made by adafruit). With the app in UART mode you can check if its dark or light in a room. It will send a message stating it if its dark or not and it also sends the current measured lux. 

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

## Reflection and context
![alt text](https://user-images.githubusercontent.com/74900539/115716421-7557f100-a379-11eb-9e35-aead221773af.png)
In the image above you can see the pipeline I used for this project. It shows the IoT device, the gateway and the IoT middleware. To provide some context, I'm a creative media and game technolgies student at the hogeschool Rotterdam. Im a first year, and we mainly focused on building and designing web applications. We had a brief introduction in working with sensors in the beginning of this year and we will work more with them next year. How to work with and using big amounts of data was relatively new to me. So for this project I mainly focused on using a working pipeline that included all three elements correctly (IoT device, the gateway and the IoT middleware). I didn't use thinkspeak for my project because I thought I could also use a bluetooth module to send data to my phone in an app. What I would do expand the project and make it bbetter is to find a better way to use big amounts of data. As of now I only check if its dark or not in a room, but maybe I could also use the sensor to check how light much light there is during the day. I could use this data to check how much this differs from day to day. I could also expand the project to checking how mich time of the day someone has the light turned on in their house. For this I could make very good use of thinkspeak. Thanks to this class I now have a better idea of IoT and how to use data efficiantly. If i had to do the project again I would expand on this one and add a broader context and use thinkspeak. 


