# Overview
The spindle-control PWM signal coming out of GRBL has saturation between 0% and 100% which is perfect for most lasers, motors etc.

If you want to use a RC-style Brushless motor with an ESC for a custom-built spindle, it requires a different type of PWM signal.
The PWM controlling those has a pulse length of 0.5~2.5ms.

This project uses a cheap Arduino Nano to convert the 0-100% PWM coming out of GRBL in order to control your RC Brushless motor. 

# Pinout
Here's how to connect it. This schematic assumes that you have common GND for both GRBL arduino and the arduino nano used for this conversion
![Schematic](https://github.com/kirilnedev/grbl-rc-pwm/blob/master/grbl-rc-pwm-schematic.jpg)
