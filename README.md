# Water-level-Controller
A water level controller is a device that manages the water level on variety of systemssuch as water tank, pumps,swimming pools.  The basic function of water level controlleris to regulate Water flow and optimize System Performance.  Here we are designing thecircuit which is used to detect and control the water level automatically in overhead tankusing 8051 microcontroller.

Componenets used:
4 resistor (1kohm)
4 resistor (10 kohm)  
5V relay module  
NPN  Transistor 
Connecting wires 
breadboard 
lcd display
8051 micro controller
header pins
10kohm ka potentiometer/ preset

Working:
This  system  mainly  works  on  a  principle  that  “water  conducts  electricity”.   The  fourwires which are dipped into the tank will indicate the different water levels.  Based on theoutputs of these wires, microcontroller displays water level on LCD as well as controls themotor.Initially when the tank is empty, LCD will display the message LOW and motor runsautomatically.  When water level reaches to half level, now LCD displays HALF and stillmotor runs.When the tank is full,  LCD displays FULL and motor automatically stops.  Again,the motor runs when water level in the tank becomes LOW.The  heart  of  the  Water  Level  Controller  using  8051  Microcontroller  project  is  theAT89C51 Microcontroller.  The water level probes are connected to the P0.0, P0.1 andP0.2 through the transistors (they are connected to the base of the transistors throughcorresponding current limiting resistors).  P0.0 for LOW level, P0.1 for HALF Level andP0.2 for HIGH Level.The  Collector  terminals  of  the  Transistors  are  connected  to  VCC  and  the  Emitterterminals are connected to PORT0 terminals (P0.0, P0.1 and P0.2).PORT1 of the microcontroller is connected to the data pins of LCD and the controlpins  RS,  RW  and  EN  of  the  LCD  Display  are  connected  to  the  P3.6,  GND  and  P3.7respectively.For demonstration purpose, we have used a simple DC Motor Pump.  It is connectedto the Relay and the input to the relay is fed from P0.7 through a transistor.

For code please open folder project code from master branch.
