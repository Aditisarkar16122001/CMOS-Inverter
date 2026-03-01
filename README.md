# CMOS-Inverter
# Discrete CMOS Inverter Using IRF540 (NMOS) & SFS9634 (PMOS)

##  Overview
This project demonstrates a **CMOS inverter built using MOSFETs** on a breadboard.  
The circuit verifies complementary switching behavior .

Unlike logic IC implementations, this setup exposes actual MOSFET characteristics relevant to CMOS device modeling and VLSI design.

---

##  Objectives
- Implement a CMOS inverter using discrete NMOS and PMOS transistors
- Observe complementary switching using LED indicators


---

##  Components Used

| Component | Description |
|----------|------------|
| IRF540 | N-channel MOSFET |
| SFS9634 | P-channel MOSFET |
| LEDs | Input & Output indicators |
| Resistors | 330 Ω – 10 kΩ |
| Breadboard | Circuit assembly |
| 5 V Supply | Power source |



My Goal Was Logic Demonstration

I wanted to show:

- Inversion

- LED indication

- Switching behavior

Capacitor is not needed for this.

---
## Circuit
![ckt](https://github.com/Aditisarkar16122001/CMOS-Inverter/blob/main/circuit.webp)

- PMOS source → VDD  
- NMOS source → GND  
- Drains connected → VOUT  
- Gates tied together → VIN  

---

##  Working Principle

| VIN | PMOS | NMOS | VOUT | Output LED |
|-----|------|------|------|-----------|
| LOW | ON   | OFF  | HIGH | ON        |
| HIGH| OFF  | ON   | LOW  | OFF       |

NMOS is responsible for pulling the voltage from high to low that's why it is called "PULL DOWN DEVICE". And the PMOS is responsible for pulling the voltage up from low to high so it's known as "PULL UP DEVICE".

---
## Images
- Vin = 0, V_out = 1 (5V)
- ![fig1](https://github.com/Aditisarkar16122001/CMOS-Inverter/blob/main/Low%20to%20high.jpg)
- ----
- Vin = V_DD(5V), V_out = 0
- ![fig2](https://github.com/Aditisarkar16122001/CMOS-Inverter/blob/main/High%20to%20low.jpg)

##  Observations

- CMOS inverter shows rail-to-rail output.
- Floating input leads to random switching.

- Demonstrates real device behavior beyond ideal CMOS models.

---





