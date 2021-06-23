# Ring-Oscillator


Ring oscillators are the basic sustained-oscillation generating devices. They are essentially a simple chain of odd numbered inverters connected in a ring. The resistance and input capacitance of inverter determine the frequency of operation. Sizing the transistors, varying input capacitances and modifying threshold voltage are a few ways to play with the frequency. It is also affected by change in ambient temperatures. 

The circuit is drawn in Cadence Virtuoso at 180nm node. The schematic created is as follows.

<img width="707" alt="Schematic" src="https://user-images.githubusercontent.com/59061427/123156625-2157ae80-d487-11eb-9217-fd5e5c8c3262.PNG">

The obtained output waveform is shown below.

<img width="760" alt="Output Waveform" src="https://user-images.githubusercontent.com/59061427/123156729-41876d80-d487-11eb-81ac-4337c4b2837d.PNG">

Typically, Frequency,f=2*N*Tp, where N is the number of inverters in the chain and Tp is the propagation delay.

Going forward, temperature dependence is noted by performing a temperature sweep for transient analysis. The obtained results are as shown below.

<img width="534" alt="Temperature Sweep" src="https://user-images.githubusercontent.com/59061427/123157163-d0948580-d487-11eb-8f02-ce8edf56ff54.PNG">
The corresponding temperature references are as presented.
<img width="79" alt="Reference" src="https://user-images.githubusercontent.com/59061427/123157250-eb66fa00-d487-11eb-9ddb-8f92ba327389.PNG">

A very remarkable point can be noted here, with the rise of temperatures, the frequency of oscilations decrease. It can be well explained theortically: Vt Decreases-Vov Decreases-Driving current Decreases-Time to charge/discharge Increases-Frequency Decreases.

ALternate Analysis in LTSPICE:

The Schematic:

![image](https://user-images.githubusercontent.com/59061427/123157848-ad1e0a80-d488-11eb-9e4f-be7458ac596a.png)

The output waveform:

![image](https://user-images.githubusercontent.com/59061427/123157985-d9398b80-d488-11eb-857b-442f280988c5.png)





