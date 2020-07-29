# Density-based-Traffic-control-system

This project's objective to it implement a Desity based traffic control system which can channel traffic automatically on based of desity of traffic in a lane.

REQUIREMENT SPECIFICATION

 Arduino uno
 4 bread boards
 LED’s for the traffic lights
 3 ultrasonic sensors
 jumper wires
 220 ohm resistors.



Arduino is the main part of this project and it will be used to read from
ultrasonic sensor HC-SR04 and calculate the distance. This distance will tell us
if any vehicle is near the signal or not and according to that the traffic signals
will be controlled.

The main task was to avoid use of delay because we have to continuously read
from the ultrasonic sensors and also at the same time, we have to control
signals which requires the use of delay function.
So we have used the timerone library which is used to repetitively measure a
period of time in microseconds and at the end of each period, an interrupt
function will be called. In this function, we will read from the sensors and in
the loop function, we will control the traffic signals.
