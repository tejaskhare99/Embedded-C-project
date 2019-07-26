# Embedded-C-project
Smart Parking System
Intoduction-
Smart parking Assistant is a user-friendly system which will help Driver to park the vehicle perfectly.
The project is based on the principle of Sonar and Infrared sensor. 
The IR module detects the presence of and obstacle and sends to the microcontroller. The microcontroller then sends a signal to rotate the stepper motor.
The HC-SR04 module has ultrasonic transmitter, receiver and control circuit on a single board. When a pulse of 10usec or more is given to the trig pin,8 pulses of 40khz are generated. After this, the echo pin is made high by the control circuit in the module.
Echo pin remains high till it gets echo signal of the transmitted pulses back.
The time for which the echo pin remains high i.e. the width of the echo pin gives the time taken for generated ultrasonic sounds to travel towards the object and return. Using this time and the speed of sound in air,we can find the distance of the object using a simple formula for distance using speed and time .
Similarly an IR proximity sensor works by applying a voltage to a pair of IR light emitting diodes (LED's) which in turn, emit infrared light. ... When the sensing unit becomes active, it sends a corresponding signal to the output terminal which can then be used to activate any number of devices.

Distance Calculation
Time taken by pulse is actually for to and from travel of ultrasonic signals, while we need only half of this. Therefore time is taken as time/2.
Distance = Speed * Time/2
Speed of sound at sea level = 343 m/s or 34300 cm/s
Thus, Distance = 17150 * Time (unit cm)
Thus this Distance is shown on the LCD 
Once the Distance is less than a set point the controller will activate the buzzer warning the driver about the obstacle too close to his vehicle. And thus this will avoid the damage to car . 


