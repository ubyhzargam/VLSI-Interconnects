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

Circuit diagram : 

<img width="443" alt="Screenshot 2024-08-12 at 10 18 59 PM" src="https://github.com/user-attachments/assets/535561d8-18a2-4b5c-8037-3b6a179ef4c1">
<br><br>
<br><br>
Transient Analysis :

<img width="1469" alt="Screenshot 2024-08-12 at 10 18 16 PM" src="https://github.com/user-attachments/assets/ed9ea40f-9302-4b2a-9108-fce3a6a319a1">

<img width="1469" alt="Screenshot 2024-08-12 at 10 17 35 PM" src="https://github.com/user-attachments/assets/cc027319-579f-41dc-83eb-65d4cd09617f">
<br><br>
<br><br>
Delay (0 to 63% rise of Vout) :

<img width="1469" alt="Screenshot 2024-08-12 at 10 17 28 PM" src="https://github.com/user-attachments/assets/3cdbe502-83b9-433a-bbd3-6269e1cccf98">

As shown in the above image the delay comes out to be around 10ps which also the expected delay value theoretically.
<br><br>
<br><br>
<br><br>
<br><br>

(b) RC distributed model : 5 segments 

Circuit diagram :

<img width="840" alt="Screenshot 2024-08-13 at 9 24 05 PM" src="https://github.com/user-attachments/assets/a371f218-55bb-4137-81a3-1596f1c783e0">

<br><br>
<br><br>

Transient Analysis :

<img width="1470" alt="Screenshot 2024-08-13 at 9 24 28 PM" src="https://github.com/user-attachments/assets/228e2272-b107-4ac7-a9bd-836fc5b66ce5">
<img width="1470" alt="Screenshot 2024-08-13 at 9 24 14 PM" src="https://github.com/user-attachments/assets/3ee4f273-c604-45c2-b9d9-1e51416de00f">
<br><br>
<br><br>

Delay (0 to 63% rise of Vout) :

<img width="1470" alt="Screenshot 2024-08-13 at 9 27 11 PM" src="https://github.com/user-attachments/assets/6993efd5-aa8d-4b39-be5f-914c8ef1b7e4">
<br><br>
<br><br>
<br><br>
<br><br>

(c) RC distributed model : 10 segments 

Circuit diagram :

<img width="1434" alt="Screenshot 2024-08-13 at 9 43 01 PM" src="https://github.com/user-attachments/assets/c8131f29-b74a-4dbd-9a56-d1c10b3490ad">

<br><br>
<br><br>

Transient Analysis :
<img width="1470" alt="Screenshot 2024-08-13 at 9 44 44 PM" src="https://github.com/user-attachments/assets/ebaae9c7-c591-46b5-a5fa-121f3b20b584">
<img width="1470" alt="Screenshot 2024-08-13 at 9 43 55 PM" src="https://github.com/user-attachments/assets/170d0538-84f2-4ceb-b536-871f4353b90b">

<br><br>
<br><br>

Delay (0 to 63% rise of Vout) :

<img width="1470" alt="Screenshot 2024-08-13 at 9 45 49 PM" src="https://github.com/user-attachments/assets/d55bb80d-62c9-4d34-bcdb-a05300d7bb7e">

<br><br>
<br><br>
<br><br>
<br><br>

Theoretically, the delay for this circuit should be close to 5ps which is the Elmore delay. More the number of segments or fragments , closer is the delay to 5ps. For the above 2 cases the delay is of order of 6ps. If you increase the number of fragments , the delay converges to 5ps.
