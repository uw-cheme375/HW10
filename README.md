# ChemE 375: HW10

The assignment is due midnight **before** the beginning of the next class period.

Note: Turn in all Aspen files with this homework assignment. Please also add in comments using text boxes under the *Format* tab. **Some points will be given for following the for presentation (formatting)**.  For each problem please use a separate Aspen file!

## Problem 1 (20 points): Txy diagrams

Using the Analysis tools in Aspen, create a Txy diagram for the methanol-water system and the methanol chloroform system. Use the UNIFAC, UNIQUAC, and Peng-Robinson thermodynamics packages and compare the Txy diagrams for each system. Copy this data to Excel to plot the data in Excel. Also compare to Txy vapor-liquid equilibrium data found on line. Comment on any differences you see and explain.

## Problem 2 (20 points): Reactor design

Take a look at process flow diagram (PFD) for the toluene hydroalkylation process in the figure below.

<img src="https://github.com/uw-cheme375/HW10/raw/master/pfd.jpg">

<br>

<img src="https://github.com/uw-cheme375/HW10/raw/master/streamtable_2.jpg">

<br>

<img src="https://github.com/uw-cheme375/HW10/raw/master/streamtable_1.jpg">


The process converts toluene and hydrogen to benzene and methane via the following reaction:

<img src="https://latex.codecogs.com/gif.latex?C_7H_8&space;&plus;&space;H_2&space;\rightarrow&space;C_6H_6&space;&plus;&space;CH_4" title="C_7H_8 + H_2 \rightarrow C_6H_6 + CH_4" />

It is desired to estimate the volume of the reactor (R-101), for which it is necessary to have kinetic expressions. For the catalytic hydroalyklation of toluene, assume that the reaction is kinetically controlled with the following kinetics:

<img src="https://latex.codecogs.com/gif.latex?-r_{tol}&space;=&space;kc_{tol}c_{tol}^{0.5}&space;\&space;\&space;\&space;\frac{kmol}{m_{reactor}^3s}" title="-r_{tol} = kc_{tol}c_{tol}^{0.5} \ \ \ \frac{kmol}{m_{reactor}^3s}" />

where

<img src="https://latex.codecogs.com/gif.latex?k&space;=&space;2.833&space;\times&space;10^7&space;e^{-\frac{17814}{T(K)}}&space;\&space;\&space;\frac{m^{1.5}}{kmol^{0.5}s}" title="k = 2.833 \times 10^7 e^{-\frac{17814}{T(K)}} \ \ \frac{m^{1.5}}{kmol^{0.5}s}" />

With these kinetics, simulate the reactor as a two-stage packed-beck adiabatic reactor with a "cold shot" (Stream 7) injected at the inlet to the second bed. The maximum temperature in the reactor should not exceed 655°C, and this will occur at the exit of both beds; that is, design the system for this maximum outlet temperature for both packed beds.

In order to solve this problem, you must select an appropriate thermodynamics package. You can use the Methods Assistant in the Methods section that will help you given the components in your stream table. Also, be very careful when entering in the kinetics of this reaction. You will have to do some unit conversions first.

## Problem 3 (20 points): Distillation Columns

Take a look at the PFD for the catalytic dehydration of methanol to produce dimethyl ether (DME) below:

<img src="https://github.com/uw-cheme375/HW10/raw/master/pfd_dme.jpg">

<br>

<img src="https://github.com/uw-cheme375/HW10/raw/master/streamtable_dme.jpg">

For the system DME/methanol/water, determine the binary interaction parameters (BIPs) used Aspen for each of these thermodynamic models: NRTL, Wilson, and UNIQUAC. Simulate the distillation column T-202 using a shortcut module for each of these models, and compare the number of theoretical stages required for the specified recoveries and R/R_min = 1.5.
