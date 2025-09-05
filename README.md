# Torque-Calculation
# Table of Contents

- [Overview](#overview)
- [Methods](#methods)
    - [Assumptions](#assumptions)
    - [Calculation](#calculation)
    - [Motor Selection](#motor-selection)
- [What If?](#what-if)
    - [Recalculation](#recalculation)
    - [Disadvantages](#disadvantages)
    - [Alternatives](#alternatives)

---

# Overview

This is Task Five in the Mechanical Engineering track, submitted to
Smart Methods Company for 2025 Summer Internship. This Task provides
torque calculations from three servo motors, each with its selection
with a purchase link to handle a weight of 1kg. Furthermore, the
capability of each motor to handle a larger weight of 2kg is also
discussed by adding some gears. Nevertheless, there are some cons and
alternatives to solve these challenges are provided.

---

# Methods

The following equation is used to calculate the torque for the robot
arm, illustrated in the table below:

Methods.png

## Assumptions

-   The force here is the weight force; F_(weight ) = m × g

-   The distances in the figure are not perpendicular, as well as no
    angle of each link is provided; therefore, assume each is
    horizontal, so ϴ = 0˚; hence, cos 0 = 1.

-   Assume g = 9.81m/s².

-   Assume the link connected to the base is link 1, the middle link is
    link 2, and the link near to the package is link 3.

---

## Calculation

1kg Load Calculation.png

## Motor Selection

Based on the previous calculations, each motor produces different
torque. Hence, the following table provides the appropriate servo
motor selection with its purchase link on Amazon Saudi:

| No. | Motor              | Details                | Purchase Link                              |
|-----|--------------------|------------------------|--------------------------------------------|
| 1   | Luqeeg High Torsion Servo Motor (35kg) | The motor torque is 3.43N.m, which can withstand 2.84N.m. | https://amzn.eu/d/inVrgOw                  |
| 2   | HIWONDER 25KG RC Servo Motor | The motor torque is 2.45N.m, which can withstand 1.37N.m. | https://amzn.eu/d/dBKoHk0                  |
| 3   | INJORA 7KG 2065 Digital Servo Motor | The motor torque is 0.69N.m, which can withstand 0.39N.m. | https://amzn.eu/d/hXMe2N8                  |

<p align="center"><b>Table 3: Motor Selection</b></p>

---

# What If?

What if the weight is changed to be 2kg instead of 1kg, will the
selected motors handle that weight by adding some gears to the motors?
And what are the disadvantages and alternatives?

First of all, doubling weight means doubling the torque; therefore, that
requires recalculation.


## Recalculation

2kg Load Calculation.png

Based on the calculations, the selected motors cannot handle these
loads. However, this issue can be solved by adding some gears to the
motors but to verify, find the gear ratio first.

| No. | Gear Ratio = $\frac{T_{output}}{T_{input\ }}$ | Evaluation   |
|-----|-----------------------------------------------|--------------|
| 1   | $$Gear\ Ratio = \ \frac{5.68}{3.43} = 1.65$$  | Can be used  |
| 2   | $$Gear\ Ratio = \ \frac{2.75}{2.45} = 1.12$$  | Can be used  |
| 3   | $$Gear\ Ratio = \ \frac{0.78}{0.69} = 1.13$$  | Can be used  |

<p align="center"><b>Table 5: Gear Ratio</b></p>

Based on the gear ratio for each motor, the motors can handle the load
by adding gears; however, there are some problems that will be shown.


## Disadvantages

-   Complex and more parts in the mechanical system.

-   Backlash which reduces precision.

-   Efficiency losses a form of heat.

-   As output torque increases, the output speed decreases by the same
    ratio.

-   Noise, vibration, and heavy weight.


## Alternatives

These advantages can be solved using the following alternative
solutions:

-   Use higher torque motors that can withstand both loads.

-   Use lighter material to decrease the required torque.

-   Use parallel motors, for example, two or more motors working
    together to achieve the desired function.
