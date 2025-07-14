# Reservoir Characterization Toolkit using Python
Python toolkit for estimating reservoir fluid properties, log-based porosity & saturation, and volumetric OOIP

It integrates key petroleum engineering calculations including:

-  Bubble Point Pressure (Pb), Solution GOR (Rs), and Oil Formation Volume Factor (Bo)
-  Porosity, Water Saturation (Sw), and Bulk Volume Water (BVW) from well log data
-  Original Oil in Place (OOIP) using volumetric method

  
##  Features

###  Module 1: PVT Estimation (Standing's Correlation)
- Calculates bubble point pressure (Pb)
- Estimates solution gas-oil ratio (Rs)
- Computes oil formation volume factor (Bo)

###  Module 2: Formation Evaluation from Well Logs
- Upload `.csv` log data with Depth, Density, and Resistivity
- Calculates:
  - Porosity using density log
  - Water saturation using Archie’s equation
  - BVW (bulk volume water)

###  Module 3: OOIP Calculation
- Estimates Original Oil In Place using the volumetric formula:
  \[
  \text{OOIP} = \frac{7758 \times A \times h \times \phi \times (1 - S_w)}{B_o}
  \]
- Uses average porosity and saturation from the log data
