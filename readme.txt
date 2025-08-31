# Dynamic Electricity Pricing with UK Smart Meter Data

This repository supports my MSc dissertation investigating how smart meter data can be used to design dynamic, fair, and sustainable electricity tariffs. It contains all scripts, notebooks, data, and results used in the project.

---

## Data
The project uses available smart meter datasets from **UK Power Networks**:

- [Smart meter consumption – substation](https://ukpowernetworks.opendatasoft.com/explore/dataset/ukpn-smart-meter-consumption-substation/information/)  
- [Smart meter consumption – LV feeder](https://ukpowernetworks.opendatasoft.com/explore/dataset/ukpn-smart-meter-consumption-lv-feeder/information/)

---

## Repository Contents  
- **Data** (already included)  
- **Code**: Preprocessing, clustering, elasticity estimation, and dynamic tariff simulations  
- **Results**: KPI tables and scenario outputs (CSV and figures)  

---

## Requirements  
- Python 3.8+  
- Key packages:  
  - pandas, numpy  
  - scikit-learn  
  - statsmodels  
  - matplotlib, seaborn  

Project Workflow 

- Two open datasets have been utilised with the LV dataset for validation onyl
1) The initial EDA explored the Substation dataset ensuring it is reflective of real-world
  expected electrcity consumption data

2) Clustering was performed on the data using K-means; results produced were not ideal
  however have been included to show the method

3) The simulation was completed using a S-Learner and simple elasticity method to compare
  different reformed tariff scenarios and show their effect on electricity consumption
  - KPIS included total reduction perctange, peak reduction and load factor change

Key Results

Average elasticity of demand was estimated to be close to zero, highlighting limited responsiveness to pricing signals.

S-learner models provided more granular insights but also suggested only modest demand shifting under dynamic tariffs.

Aggressive reforms created higher peak reductions, but often at the expense of customer cost neutrality.

The exploratory k-means clustering did not yield useful consumer groupings, but demonstrated attempts to uncover heterogeneity.