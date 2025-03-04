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

How it works:

1.  Clock Generation: 
o	The 555 Timer generates a continuous clock signal in astable mode.
o	The clock signal is fed into the counter and the 7476 flip-flops.
2.  Decade Counter Operation:
•	The counter has 10 outputs (Q0 to Q9), which activate sequentially as the clock pulses are received.
•	For the traffic light system:
o	Specific outputs can represent the states of the lights for North-South or East-West directions.
o	The remaining outputs may be unused or reset the counter after a full cycle.
3. Flip Flops: 
o	The 7476 JK flip-flops play a critical role in the system by managing the directional toggling between North-South and East-West signals.
4.  Logic Decoding:
•	The outputs of the counter and the flip-flops are combined using logic gates to determine the active LEDs.
•	For example:
o	When Q0 is active, the logic gates ensure that:
	North-South: Green.
	East-West: Red.
o	When Q1 is active:
	North-South: Yellow.
	East-West: Red.
o	The flip-flops ensure that after Q3, the sequence switches to East-West green, yellow, and red.
LED Outputs
•	Each set of LEDs (red, yellow, green) represents the traffic light signals for one direction.
•	Resistors limit the current to prevent damage to the LEDs.
5.  Traffic Light Outputs:
•	LEDs (or physical traffic lights) are connected to the outputs of the logic gates.
•	These outputs correspond to the lights being ON/OFF for North-South and East-West directions in a specific sequence.


Simulation:



![image alt](https://github.com/aya175/4-Way-Traffic-Light-System-/blob/a688ff8844da92662944ea4639dd0f46177c1c36/test.png)
