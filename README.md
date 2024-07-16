# Homebridge-New-Simple-Garage-Door-Opener

This plugin is based on the work of Daniel Reiser and his homebridge plugin [Homebridge-Simple-Garage-Door-Opener](https://github.com/danielreiser/Homebridge-Simple-Garage-Door-Opener)

I have update the code to replace the RPIO package who seems to not be updated anymore by GPIOX

It has been tested on a Pi 5.

### Pi 5 GPIO Layout

![Raspberry-Pi-5-Pinout-](https://github.com/user-attachments/assets/7ba6f950-9ef1-449b-a0b1-69669288fc8e)

### Configuration example

```
"accessories": [{
        "accessory": "SimpleGarageDoorOpener",
        "name": "SimpleGarageDoorOpener",
        "doorSwitchPin": 23,
        "simulateTimeOpening": 15,
        "simulateTimeOpen": 30,
        "simulateTimeClosing": 15
    }]
```

### Warning

The value "doorSwitchPin" represents the GPIO number, not the pin number

Example: To use the Pin GPIO 23 you need to enter 23 and not 16
