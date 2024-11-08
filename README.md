java c
EEE211 
The Design of an Operational Amplifier using LTSpice 
Introduction: 
In this assignment, we design and simulate an operational amplifier circuit. In first part, you analyse three basic circuits. Integrating these circuits will be the next part.
This assignment is intended to reinforce lecture material in module EEE211 and reference to the relevant lecture notes is strongly advised. 
Assessment: 
You will need to finish all the tasks during the lab and show your results to TAs. 
Description: 
The amplifier can be constructed from four basic circuits and simulated using library models located in the library for the following devices:-
Q2N2222                  npn transistor
Q2N2907                  pnp transistor2
Lab Assignment 1 
Before commencing with the design, you should obtain a set of output characteristics for each of the two types of transistor to be used. Set up a circuit in LTSPICE to achieve this (details can be found in the Appendix). Obtain the characteristics over the collector current range 0 – 5mA and collector-emitter voltage range 0 - 20 volts. From these characteristics, determine the Early voltage for each transistor.
Task 1: Show your waveform. of IC(Q1), calculate the early voltages of Q2N2222 npn and Q2N2907 pnp transistors.
1. The common emitter amplifier 
This is the first circuit that you should simulate. The basic circuit is shown in Fig 1.

Fig 1 The common emitter amplifier circuit
The circuit should be supplied by a +9 to -9 volts split power supply that is balanced about ground as shown. Choose an initial value of (e.g. 1kΩ) for the collector resistor RC. The DC base bias current IBQ should be supplied from a DC current source and its value chosen to ensure that the quiescent collector voltage is at zero volts. (To find the bias needed for this condition, sweep the value of IBQ and measure the corresponding range of Vout).
Establish the appropriate DC bias condition first and then couple an ac voltage signal to the base via a coupling capacitor (say 0.1uF) so that the DC bias condition is not affected. Use a transient analysis to determine the voltage gain Av = vout/vin , noting that because the input voltage is being measured at the transistor base terminal, the volt drop across the coupling capacitor is not relevant to the calculation. However, it will be convenient to avoid a significant volt drop across the coupling capacitor so you should choose a signal frequency that ensures that the impedance of the capacitor is negligible compared to the input resistance of the transistor.
It can be shown that the maximum voltage gain that can be obtained from the circuit shown is:-

In this example, VCC is 9v, so the theoretical maximum voltage gain from this circuit is 360.
Task 2: RC is changing from 500Ω, 1kΩ, and 10kΩ. Measure the corresponding waveforms of voltage gains of the entire circuit. Ensure that in each case, the transistor bias IBQ is adjusted to maintain the DC collector voltage at zero volts.
Task 3: Consider to connect a RL to GND with the same value as RC (500Ω, 1kΩ, and 10kΩ.). Measure the corresponding waveforms of current gains for the entire circuit.
2. The current mirror circuit 
A popular circuit that provides an approximation to a constant current source is the ‘current mirror’. A pnp version of the basic circuit is shown in Fig 2. Assuming that the supplies are fixed at +9 and -9 volts, the current in the collector of Q3 is determined by the resistor R2.

Fig. 2 – A pnp current mirror circuit.
Simulate the circuit and verify that the circuit operates as a constant current source (approximately). Determine its output resistance and lower voltage limit over which it may be considered to approximate to a constant current source.
[Hint: To do this, connect a voltage source to the collector of Q3 and perform. a D.C. analysis in which that voltage source is swept from -9V代 写EEE211 The Design of an Operational Amplifier using LTSpice
代做程序编程语言 to 9V. You can then plot IC(Q3) as a function of output voltage to determine the effective output resistance of the circuit and its voltage limitation.]
Task 4: Measure the output resistance and find the voltage limits of the circuit, and show the corresponding waveforms.
The voltage gain of the common emitter circuit already simulated (Fig 1) can be increased above its maximum value of 40VCC if RC is replaced by a constant current source.
Using a combination of the circuits given in Figs 1 and 2, design a circuit to give a voltage gain of at least 1000 with a voltage supply of +9V to -9V. Remember to keep the current drawn from the supply well within the limit given in the specification to allow some current to be drawn by the remaining circuits that are still to be designed in next lab session (total current drawn from power supply MUST be less than 5mA).
Measure the voltage gain AV = vout/vin and the total current drawn from the supply, ICC.
Task 5: Establish your circuit in which current mirror acting as the collector load of the common emitter stage. Then, measure and show the waveforms of the voltage gain and the current drawn from the voltage supply of your circuit.
3 The emitter follower 
The circuit of an emitter follower is given in Fig 3. Note the following key equations that relate to this circuit:-

Fig. 3 – The emitter follower circuit.
Input impedance = rπ + (β + 1)R1
Output impedance = 
Where rπ = gm/β 
gm = 40IC 
and Rb = total equivalent resistance ‘seen by’ the base terminal.
Using these equations, design an emitter follower stage that when added to the amplifier already designed, will give an output impedance that meets the specification (i.e. less than 1kΩ). Note that the emitter follower will represent a load to the voltage amplifier. Consider the effect of this on the voltage gain when you design your emitter follower. Also remember to keep the total current drawn from the supply well below the upper limit in the specification. (There are two further stages to be designed in Assignment 2 to complete the full op-amp circuit).
Add the circuit to your previous design and measure the overall voltage gain, current drawn from the supply and the output resistance. [Hint: you can measure the output resistance by attaching a small ac voltage source to the output through a coupling capacitor (so that the DC bias of the circuit is not disturbed) and measuring the ac current.]
Task 6: Establish a correct circuit which can satisfy all the requirements. Then, measure and show the waveforms of the voltage gain, the current drawn from the voltage supply, and the output resistance of your circuit.
EEE211 
Lab Assignment 1 
Design of Basic Transistor Amplifiers 
TASK SHEET 
Task 1: Show your waveform. of IC(Q1), calculate the early voltages of Q2N2222 npn and Q2N2907 pnp transistors (10%).
Task 2: RC is changing from 500Ω, 1kΩ, and 10kΩ. Measure the corresponding waveforms of voltage gains of the entire circuit. Ensure that in each case, the transistor bias IBQ is adjusted to maintain the DC collector voltage at zero volts. (15%)
Task 3: Consider to connect a RL to GND with the same value as RC (500Ω, 1kΩ, and 10kΩ.). Measure the corresponding waveforms of current gains for the entire circuit. (15%)
Task 4: Measure the output resistance and find the voltage limits of the circuit, and show the corresponding waveforms. (10%)
Task 5: Establish your circuit in which current mirror acting as the collector load of the common emitter stage. Then, measure and show the waveforms of the voltage gain and the current drawn from the voltage supply of your circuit. (20%)
Task 6: Establish a correct circuit which can satisfy all the requirements. Then, measure and show the waveforms of the voltage gain, the current drawn from the voltage supply, and the output resistance of your circuit. (30%)



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
