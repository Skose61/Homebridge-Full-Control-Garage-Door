# Homebridge-New-Simple-Garage-Door-Opener

This plugin is based on the work of Daniel Reiser and his homebridge plugin [Homebridge-Simple-Garage-Door-Opener](https://github.com/danielreiser/Homebridge-Simple-Garage-Door-Opener)

It has for purpose to update the code and make it compatible with the latest Raspberry pi.

I have replace the RPIO package by GPIOX.

It has been tested on a Pi 5.

Warning the value "doorSwitchPin" represents the GPIO number, not the pin number
![Raspberry-Pi-5-Pinout-](https://github.com/user-attachments/assets/7ba6f950-9ef1-449b-a0b1-69669288fc8e)
Example: To use the Pin GPIO 23 you need to enter 23 and not 16

# Configuration example

```
"accessories": [{
        "accessory": "SimpleGarageDoorOpener",
        "name": "SimpleGarageDoorOpener",
        "doorSwitchPin": 12,
        "simulateTimeOpening": 15,
        "simulateTimeOpen": 30,
        "simulateTimeClosing": 15
    }]
```
