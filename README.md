# 4-Way-Traffic-Light-System
control system for an The objective of this project is to design and implement a 4-way traffic light intersection using digital logic components.
The system uses a counter (7490), 7476 JK flip-flops, a 555 Timer, and a combination of logic gates (AND, OR, NOT).
This setup ensures smooth and accurate sequencing of green, yellow, and red lights for both North-South and East-West directions

Circuit Components:
1.	555 Timer IC (NE555):
o	Configured in astable mode to generate a clock signal. This signal toggles the states of the lights in sequence.
o	The resistors (R1, R2) and capacitor (C2) set the timing interval of the clock signal.
2.	Counter(7490):
o	A counter is used to generate a sequence based on the clock signal from the 555 Timer.
o	The output from the counter is fed into logic gates to control the timing of the traffic lights.
3.	Logic Gates (AND, OR, NOT):
o	These gates are used to decode the binary counter output and determine which light should turn ON or OFF at any given time.
4.	LED Indicators (Traffic Lights):
o	LEDs or traffic light representations indicate the output for four directions.
o	Typically includes Red, Yellow, and Green lights.
5.	Flip-Flops(7476):
o	Store and control states for specific light signals.
o	Used for managing more complex traffic light behaviors.
6.	Connections to Traffic Lights:
o	Separate clusters of logic control the Red, Yellow, and Green lights for each traffic lane.
7.	Resistors & Capacitors: 
o	Set the clock frequency and manage intensity for the led and rest of circuit.



