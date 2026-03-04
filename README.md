Problem statement: To design a simple reflex agent that takes environmental parameters from sensors (provided as a dataset file) and calculates the Air Quality Inex(AQI)
***The dataset used in this project is based on air quality data from 2015
Therefore:
All AQI calculations are performed using 2015 data
Any selected date must belong to 2015
The project is not using real-time data

The agent works as a Simple Reflex Agent, meaning:
It does not store past states
It only reacts to current environmental input
It follows predefined AQI threshold rules

The agent processes the following environmental parameters:
NO
NO₂
NOx
CO
SO₂
O₃
Benzene
Toluene
Xylene

Step-by-Step Working:
Read pollutant concentrations from dataset (for a selected date in 2015).
Identify the maximum pollutant concentration.
Map that value to the AQI scale using predefined threshold ranges.
Classify the AQI into categories:
Good
Satisfactory
Moderate
Poor
Very Poor
Severe

Extension: Traffic regulation logic
Based on AQI level, the system can estimate:
Whether vehicle restrictions are required
Approximate number of vehicles allowed on road
Pollution control recommendations

For example:
AQI Range	Action
0–50	No restriction
51–100	Monitor levels
101–200	Reduce vehicles by 20%
201–300	Odd-even system
301+	Emergency restrictions
