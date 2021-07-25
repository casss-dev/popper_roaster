# popper_roaster

This sketch allows automated or manual control over the temperature of a modified popcorn popper coffee roaster.

## How it works
When in automatic mode, users can set a static time and temperature profile in seconds and the PID algorithm will attempt to adjust the voltage sent to the heating element based on a 0-100 scale.

## Features
- You can dynamically change the proportional, integral, or derivative terms throughout the roast to help dial-in the heat output
- You can dynamically label different phases of the roast (dry-end, first crack, first crack end, second crack, etc...)
- Outputs to CSV format for easy input into spreadsheets and graphs

Output is formatted as: Time (sec), BT (bean temperature ºF), PID (values), HeaterPower (%), RoR (Rate of rise), Data Labels

## Hardware used

- Nostalgia Air Popper
- Arduino Uno
- K-Type Thermocouple 1/8 inch diamter
- Max 6675 Module
- 40 DA Fokek Solid State Relay
- 16 awg wires

## Acknowledgements
#### This sketch makes use of the following open source libraries

- [Arduino PID Library](https://github.com/br3ttb/Arduino-PID-Library/)
- [Arduino Max 6675 Library](https://github.com/adafruit/MAX6675-library)
