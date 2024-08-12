# VLSI-Interconnects
This repository has simulations of various models of Interconnects and the delay due to interconnects. All the simulations are done on LT Spice

# RC MODEL - 

An RC interconnect has the following parameters:
Interconnect length / = 1000m
Resistance per unit-length R = 0.025/um
Capacitance per unit-length C = 0.5f F/um
Consider an input voltage clock of 2GHz, and peak voltage 1V, with 50% duty cycle.
(a) Simulate the output considering a single lumped RC model. Does the simulated 63% delay (the RC time constant) match with the theoretical value for the lumped model?
(b) Simulate the interconnect by dividing it in 5 sections to approximate the the distributed model.
(c) Simulate the interconnect by dividing it in 10 sections to approximate the the distributed model. Does the 63% delay converge to Elmore delay as you increase the number of sections?
(d) Simulate the interconnect with
(1) pi-equivalent model (ii) pi2-equivalent model
Does the equivalent i model give a better approximation of distributed model with lesser number of terms?

(a) RC lumped model - 

Circuit diagram
<img width="443" alt="Screenshot 2024-08-12 at 10 18 59 PM" src="https://github.com/user-attachments/assets/535561d8-18a2-4b5c-8037-3b6a179ef4c1">

Transient Analysis
<img width="1469" alt="Screenshot 2024-08-12 at 10 18 16 PM" src="https://github.com/user-attachments/assets/ed9ea40f-9302-4b2a-9108-fce3a6a319a1">
<img width="1469" alt="Screenshot 2024-08-12 at 10 17 35 PM" src="https://github.com/user-attachments/assets/cc027319-579f-41dc-83eb-65d4cd09617f">

Delay (0 to 63% rise of Vout) 
<img width="1469" alt="Screenshot 2024-08-12 at 10 17 28 PM" src="https://github.com/user-attachments/assets/3cdbe502-83b9-433a-bbd3-6269e1cccf98">



