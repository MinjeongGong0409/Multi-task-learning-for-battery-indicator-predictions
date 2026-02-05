# Multi-task-learning-for-battery-indicator-predictions
## Introduction
This repository contains diagnostic protocol data collected from 18650 cylindrical batteries, corresponding battery indicators, and the source code for three key battery indicator predictions. Three key battery indicators include state of health (SoH), DCIR (direct current internal resistance) increase rate, and Max. temp. (maximum temperature measured during 0.5 C-rate charging and discharging).

## MTL_data overview
The raw data of diagnostic protocol data are in our previous study (https://github.com/MinjeongGong0409/Direct_SoH_prediction). It consists of all protocol data measured at a specific cycle, and each protocol data includes the voltages at each current pulse and rest time (1.65, 2.0 C-rate charge and discharge current pulse for 5 seconds and rest times between every current pulse)
The calculated features every state of charge (SoC) are stored in 'MTL_data.xlsx. There are initial/final voltage at each current pulse and rest time, resistance, IR drop, skewness, and kurtosis. In addition, the ratio of resistance, or hysteresis also calculated.

## Code overview
All of the codes used in model optimization, training and analysis can be found in ‘Multi-task learning for battery indicator prediction.ipynb'.
