---
title: Tutorial 2
date: 2026-05-12 18:28
description:
categories:
tags:
---
## True/False


| Nr  | Question                                                                                              | Answer | Reason                                                                            |
| --- | ----------------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------- |
| 8   | One ampere of current is present when one coulomb of charge passes through a conductor in one second. | True   |                                                                                   |
| 11  | Copper has the highest conductivity of any metal used in electronics.                                 | False  | (Silver has higher conductivity; copper is preferred due to cost and workability) |
| 17  | An instrument designed to read current is called an voltmeter.                                        | False  | Instrument designed to read current is called an **ammeter**                      |
## Multi Choice 

| Nr  | Question                                                                                                                                                       | Answer                                              | Reason |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | ------ |
| 3   | How much energy is expended in moving a 20 coulomb charge through a potential difference of 0.5 volts?                                                         | A - **10 joules**                                   |        |
| 4   | Determine the potential difference if it takes 300 mJ of energy to move a charge of 67 microcoulombs.                                                          | B - **4.5 kilovolts**                               |        |
| 5   | Reverse connection of a voltmeter in a dc circuit will cause                                                                                                   | D - **a reading that is below scale or negative.**  |        |
| 9   | What is the current (in amperes) if 10.0 coulombs of charge pass through a wire in 2.0 seconds?                                                                | B - **5 amperes**                                   |        |
| 13  | If 40 joules of energy are required to move 25 coulombs of charge, what would the voltage be?                                                                  | B - **1.6 volts**                                   |        |
| 14  | How must ammeters be connected in a circuit when used to measure current?                                                                                      | B - **In series with the component being measured** |        |
| 15  | What potential (voltage) exists between two power supply terminals if 5 joules of energy are required to move 10 coulombs of charge between the two terminals? | C -**0.5 V**                                        |        |
| 18  | What is the charge in coulombs if 8.5 mA of current flow through a surface every 90 ms?                                                                        | A - **770 microcoulombs**                           |        |
| 19  | What is the current in amperes if 0.71 coulomb of charge passes by a point every 8.9 ms?                                                                       | A - **80 amps**                                     |        |

## Missing Words 

| Nr  | Question                              | Answer             | Reason |
| --- | ------------------------------------- | ------------------ | ------ |
| 2   | DMM stands for __                     | Digital Multimeter |        |
| 10  | A Voltmeter is designed to measure __ | Voltage            |        |

## Calculation Problems 

### Question 1

One coulomb is the total charge associated with $6.242 × 10^{18}$ electrons.
How many electrons will pass through a conductor if 40 μA of current flows for 187 seconds? 
(**Answer example:** 6.2e+18 electrons ; Round your answer to 3 decimal places.)


First, calculate the total charge $Q$ that passes through the conductor:

$$ Q = I \times t $$
where:
- $I = 40 \, \mu\text{A} = 40 \times 10^{-6} \, \text{A}$ 
- $t = 187 \, \text{s}$
$$
\begin{aligned}
Q &= It \\
  &= 40 \times 10^{-6} \times 187 \\
  &=  7.48 \times 10^{-3} \, \text{C} \\
\end{aligned}
$$


The number of electrons $n$ is found using the charge per electron (or equivalently, electrons per coulomb):

using this part: 
*One coulomb is the total charge associated with $6.242 × 10^{18}$ electrons.*
$$ n = Q \times \left(6.242 \times 10^{18} \, \frac{\text{electrons}}{\text{C}}\right) $$

$$ n = 7.48 \times 10^{-3} \times 6.242 \times 10^{18} $$

$$ n = 4.669 \times 10^{16} \, \text{electrons} $$


**Answer:** 4.669e+16 electrons

---

### Question 12

An 96%  efficient; 4 horsepower electric motor pumps water through a height of 528 m. · Determine the rate it pumps water. 
**Answer in liter/min**

X - 96% (0.9) - trick
Y - 4 hp
Z - 528 m

> The efficient is a trick, it skip

1. Convert horsepower to watts (power) $$ P_\text{in} = 4 \times 746 = 2984 \, \text{W} $$

2. Mass flow rate (from potential energy rate) $$ P_\text{mech} = \dot{m} \cdot g \cdot h $$ $$ \dot{m} = \frac{P_\text{mech}}{g \cdot h} $$

Using textbook value **g = 9.81 m/s²**: 

$$
\begin{aligned}
\dot{m} &= \frac{2984}{9.81 \times 528} \\
\space \\
&= \frac{2984}{5179.68} \\
\space \\
&\approx 0.576097 \, \text{kg/s} \\
\end{aligned}
$$

4. Volume flow rate (1 kg water ≈ 1 L) 

$$
\begin{aligned}
\dot{V} &= 0.576097 \times 60\\

 &\approx 34.566 \, \text{L/min}
\end{aligned}
$$
**Answer:** 34.566 liter/min

---
### Question 3

How much energy is expended in moving a 20 coulomb charge through a potential difference of 0.5 volts?

$W=QV=20C \times 0.5V=10J$

**Answer:** 10 joules
### Question 4

Determine the potential difference if it takes 300 mJ of energy to move a charge of 67 microcoulombs.

$$V=\frac{W}{Q} = \frac{300\times10^{-3}}{67\times10^{-6}}=4,478kV$$




**Answer:** 4.5 kilovolt

---
### Question 6

A water pump driven by an electric motor pumps water through a height of 144 m at the rate of 1200 L/min. Calculate the power required if the motor efficiency is 89 %. 
**Answer in kW**


Step 1: Convert flow rate to mass flow rate Volume flow rate = 1200 L/min $$ \dot{V} = \frac{1200}{60} = 20 \, \text{L/s} $$ Since 1 L of water = 1 kg, **Mass flow rate** $\dot{m} = 20 \, \text{kg/s}$

Step 2: Calculate mechanical power required to lift the water $$ P_{\text{mech}} = \dot{m} \, g \, h $$ where $g = 9.81 \, \text{m/s}^2$, $h = 144 \, \text{m}$

$$ P_{\text{mech}} = 20 \times 9.81 \times 144 = 28\,252.8 \, \text{W} = 28.253 \, \text{kW} $$

Step 3: Calculate electrical input power (accounting for efficiency) Motor efficiency $\eta = 89\% = 0.89$

$$ P_{\text{elec}} = \frac{P_{\text{mech}}}{\eta} = \frac{28.253}{0.89} \approx 31.745 \, \text{kW} $$
**Answer:** 31.7 kW

---
### Question 7

An electric lamp consumes 154 W and the current flow through it is 5 A. 
Determine the work done in 18 min.

$$\begin{aligned}
W &= P \times t \\
&= 154 \times (18 \times 60) \\
&= 154 \times 1080 \\
&= 166320 \, \text{J}
\end{aligned}$$

**Answer:** 166.32 kJ

---
### Question 9

What is the current (in amperes) if 10.0 coulombs of charge pass through a wire in 2.0 seconds?

$$ I = \frac{Q}{t} = \frac{10.0}{2.0} = 5.0 \, \text{A} $$

**Answer:** 5 amperes


### Question 13

If 40 joules of energy are required to move 25 coulombs of charge, what would the voltage be?

$$ V = \frac{W}{Q} = \frac{40}{25} = 1.6 \, \text{V} $$

**Answer:** 1.6 volts
### Question 14

How must ammeters be connected in a circuit when used to measure current?

**Answer:** In series with the component being measured
### Question 15

What potential (voltage) exists between two power supply terminals if 5 joules of energy are required to move 10 coulombs of charge between the two terminals?

$$ V = \frac{W}{Q} = \frac{5}{10} = 0.5 \, \text{V} $$

**Answer:** 0.5 V
### Question 16

An electric lamp consumes 701 W and the current flow through it is 117 A. Determine the emf.

$$ V = \frac{P}{I} = \frac{701}{117} \approx 5.99 \, \text{V} $$

**Answer:** ≈ 6.0 V

### Question 18

What is the charge in coulombs if 8.5 mA of current flow through a surface every 90 ms?

$$ Q = I \times t = 8.5 \times 10^{-3} \times 90 \times 10^{-3}  \approx 770 \times 10^{-6} \, \text{C} $$

**Answer:** 770 microcoulombs

### Question 19

What is the current in amperes if 0.71 coulomb of charge passes by a point every 8.9 ms?


$$ I = \frac{Q}{t} = \frac{0.71}{8.9 \times 10^{-3}} \approx 80 \, \text{A} $$


**Answer**: 80 amps