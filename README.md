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


---
## Circuit

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

When the input is left floating, the inverter may switch due to environmental noise and gate capacitance, causing LED flickering.

---
## Images

##  Observations

- CMOS inverter shows rail-to-rail output.
- High input impedance makes the circuit noise-sensitive.
- Floating input leads to random switching.
- Threshold mismatch between IRF540 and SFS9634 shifts switching point.
- Demonstrates real device behavior beyond ideal CMOS models.

---

##  Educational Significance

This project demonstrates key CMOS concepts used in semiconductor design:

- Threshold voltage effects  
- NMOS vs PMOS mobility differences  
- Gate capacitance and leakage  
- Noise margins and floating node behavior  

These principles are fundamental to **CMOS device modeling and standard cell design**.

---



