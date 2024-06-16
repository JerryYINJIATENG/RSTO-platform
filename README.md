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

## Pseudocodes of BRC algorithm and ILS algorithm

![Algorithm 1. BRC algorithm to compute the optimal cost of big arcs](https://github.com/JerryYINJIATENG/RSTO-platform/blob/master/Materials/ILS.png)


![Algorithm 2. Improved label setting algorithm](https://github.com/JerryYINJIATENG/RSTO-platform/blob/master/Materials/LabelCorrecting.jpg)

## Parameters in the experiments

The basic operational parameters, involving running time between two stations, dwelling time at the platforms, minimum turnaround time, safety headway time  and slack time, etc.

## Results
We test the performance improvement of different acceleration schemes, i.e., our proposed big-arc strategy, the greedy-based column generation (termed as S1), and bi-directional search (termed as S2), in which the latter heuristics are widely used in the literature. This allows us to compare eight approaches for solving the instances: no-acceleration (NS), only S1, only S2, S1 plus S2 (S1+S2), both with and without big-arcs. The following table represents the details results for the constructed 30 instances.

|Instance|NS|S1|S2|S1+S2|NS|S1|S2|S1+S2|
|  ----  | ----  |----  |----  |----  |----  |----  |----  |----  |
| |Without big-arcs| |  | |With big-arcs| | | |
|I_1|4.8|3.98|2.45|2.43|4.57|4.50|1.90|1.88|
|I_2|5.51|5.02|4.22|2.98|5.28|4.45|2.88|2.13|
|I_3|1.03|1.04|1.03|1.03|1.03|1.05|1.04|1.08|
|I_4|2.98|2.88|2.65|2.48|2.78|2.55|2.09|1.98|
|I_5|2.96|2.92|2.92|2.87|2.54|2.42|2.33|2.21|
|I_6|14.3|12.2|13.2|10.2|10.5|9.2|10.4|8.6|
|I_7|76.8|55.6|68.7|52.3|54.3|36.4|52.1|34.5|
|I_8|70.3|58.3|63.2|48.4|50.9|39.2|48.8|37.3|
|I_9|99.8|85.4|	89.7|77.2|	80.4|	64.2|	78.5|	55.3|
|I_10|20.9|17.9|16.4|15.3|15.7|12.0|14.3|10.6|
|I_11|60.1|	52.3|	59.1|	51.2|	54.3|	47.8|	50.2|	45.0|
|I_12|50.0|42.4|48.7|39.1|45.2|37.5|35.5|32.8|
|I_13|288.2|250.4|277.5|242.3|229.9|188.9|220.4|186.0|
|I_14|180.7|166.9|178.4|164.2|134.7|130.3|133.5|115.3|
|I_15|190.8|179.4|185.5|174.3|179.4|160.9|168.6|154.2|
|I_16|2.21|2.01|2.20|1.95|2.02|2.01|2.20|1.90|
|I_17|3.53|2.98|2.99|2.21|2.45|2.23|2.44|2.21|
|I_18|2.32|2.40|1.22|1.08|1.90|1.90|1.23|1.10|
|I_19|3.01|3.00|1.90|1.89|2.20|2.11|2.10|1.98|
|I_20|3.87|3.74|2.98|2.25|3.01|2.98|2.42|2.24|
|I_21|49.8|42.2|40.3|32.3|33.7|30.5|29.8|28.5|
|I_22|42.5|40.9|40.0|38.0|41.4|40.8|33.5|30.3|
|I_23|80.4|80.1|80.0|78.1|74.4|74.3|60.8|60.2|
|I_24|95.4|90.9|90.3|82.5|69.2|69.1|52.5|50.4|
|I_25|94.1|87.6|89.2|83.9|76.9|70.4|74.2|68.3|
|I_26|264.9|235.0|252.3|223.4|210.9|202.5|209.0|198.7|
|I_27|288.9|275.5|287.4|272.2|270.3|265.4|268.8|254.4|
|I_28|75.5|69.5|70.0|59.8|60.4|55.2|56.6|48.3|
|I_29|122.2|120.2|117.9|101.2|98.8|90.3|91.2|87.6|
|I_30|80.1|71.3|70.9|68.6|65.6|52.4|55.4|49.9|
|Average|75.9|68.8|72.1|64.5|62.8|56.8|58.8|45.93|
