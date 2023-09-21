---
layout: page
title: Software
permalink: /softe/
---
# Hardware
The brain of the system is an Arduino UNO. I plan to upgrade this to the RPi-pico-w and remove the need for the slip-ring in the future while still being able to record data to allow for development and tuning.  
The sensors consist of the standard MPU6050 Accelerometer/Gyro and a quadrature encoder from the reaction mass' DC motor. Motor controller is the all too common in hobby projects L298N. I have so many of these lying around they end up in all my projects. They're a fun challenge to work with given the ridiculously high deadband they cause the system to have because of the voltage drop across the BJTs.  

# GUI
See the [GUI Page]({{ site.baseurl }}{% link gui.md %})
# Comms Protocol
The system currently uses a g-code style communications protocol that happens over the serial interface. This has worked for many of my controls projects in the past but I plan to move towards a more robust and useful solution, the serial-packets library, which a has been built as part of robotics-crash-course. See [serial-packets](https://github.com/robotics-crash-course/serial-packets) on github.