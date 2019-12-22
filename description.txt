The whole arduino line follower robot can be divided into 3 sections: sensor section, control section and driver section.

Sensor section:

This section contains IR diodes, potentiometer, Comparator (Op-Amp) and LED’s. Potentiometer is used for setting reference 
voltage at comparator’s one terminal and IR sensors are used to sense the line and provide a change in voltage at comparator’s 
second terminal. Then comparator compares both voltages and generates a digital signal at output. Here in this line follower 
circuit we have used two comparator for two sensors. LM 358 is used as comparator. LM358 has inbuilt two low noise Op-amps.

Control Section:

Arduino Pro Mini is used for controlling whole the process of line follower robot. The outputs of comparators are connected 
to digital pin number 2 and 3 of arduino. Arduino read these signals and send commands to driver circuit to drive line follower. 

Driver section:

Driver section consists motor driver and two DC motors. Motor driver is used for driving motors because arduino does not supply 
enough voltage and current to motor. So we add a motor driver circuit to get enough voltage and current for motor. Arduino sends 
commands to this motor driver and then it drive motors.
