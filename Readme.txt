Treppenlicht

An automatic staircase illumination system using an arduino and LED strips coupled with motion sensors

Content: 
Fritzing File: 	Here the schematic setup of the wiring and the components is shown 
Main Code: 	The code uploaded to the arduino Test Code: For all important components, 
		a testing file will be included Component list: All used components with important explanations

Generall Stuff: 
The idea is to have a motion triggered LED illumination of all steps in the staircase, which only can only be 
activated after a defined time of day. When the bottom motion sensor is activated, the stairs shall be illuminated 
from the bottom to the top and stay on for a defined duration. Afterwards the step lights are turned off in the 
same order as they turned on. Vice verca if the top sensor is activated first.

The working principle is based on the the HC-SR501 PIR Module as a motion sensor, which gives a signal to the 
arduino when activated. The arduino is connected to a PCA9685 16 Channel PWM Driver, which outputs the PMW signal 
for up to 16 steps. To activate the LEDs, they are connected to a logic level MOSFET (IRLZ44N) and respective 
pull-down resistor.


Notes:
- The 12V LEDs are quite bright, but with an additional resistor, the brightness is better suited. 
- Still need a 5V conversion - test the 7508 converter
- 