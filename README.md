# Real-Time Rolling Stock and Timetable Rescheduling in Urban Rail Transit Systems

The software and data in this repository are a snapshot of the software and data
that were used in the research reported on in the paper "Real-Time Rolling Stock and Timetable Rescheduling in Urban Rail Transit Systems" by J. Yin, L. Yang, Z.Liang, et al.
## Description

This repository includes the computational results, source codes and source data (with no conflict of interest) for the experiments presented in the paper. 

## Requirements
For these experiments, the following requirements should be satisfied
* a PC with at least 16 GB RAM
* C++ run on Windows 10 (with SDK higher than 10.0.150630.0)
* CPLEX 12.80 Academic version.

![Algorithm 1. BRC algorithm to compute the optimal cost of big arcs](https://github.com/JerryYINJIATENG/RSTO-platform/blob/master/Materials/ILS.png)


![Algorithm 2. Improved label setting algorithm](https://github.com/JerryYINJIATENG/RSTO-platform/blob/master/Materials/LabelCorrecting.jpg)

## Results
The results for each instance, involving the fleet size of rolling stocks, ATT (unit: second), value of objective function, CPU time and optimality gap, are involved in [results](results) by "NO BRS", "Randomly solution", "LSM" and "ILM", as presented in Table 11 in the paper.

| 列1 | 列2 | 列3 |
| Instance|NS|S1|S2|S1+S2|NS|S1|S2|S1+S2|
|I_1|4.8|3.98|2.45|2.43|4.57|4.50|1.90|1.88|
| 单元格4 | 单元格5 | 单元格6 |
