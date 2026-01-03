# Battery Data Analysis

## Overview
This project analyzes battery performance data, focusing on voltage, current, and temperature. It includes fault detection for low voltage and over-temperature conditions and visualizes key parameters over time.

## Dataset
The analysis uses CSV files containing time-series measurements with the following columns:  

- `Time` – Time in seconds  
- `Voltage_measured` – Measured battery voltage (V)  
- `Voltage_load` – Load voltage (V)  
- `Current_measured` – Measured current (A)  
- `Current_load` – Load current (A)  
- `Temperature_measured` – Measured battery temperature (°C)  

## Features
1. **Voltage Analysis**  
   - Plots measured vs. load voltage over time.  
   - Marks low voltage events (voltage < 2.7 V).  

2. **Current Analysis**  
   - Plots measured vs. load current over time.  

3. **Temperature Analysis**  
   - Plots battery temperature over time.  
   - Detects over-temperature events (temperature > 55 °C).  

4. **Fault Detection**  
   - Flags low voltage and over-temperature conditions.  
   - Provides counts of fault occurrences.  

## Requirements
- Python 3.8+  
- pandas  
- numpy  
- matplotlib  

## Usage
1. Place your CSV data in the `data/cleaned_dataset/` folder.  
2. Update the file path in the script if necessary:  
   ```python
   df = pd.read_csv("../data/cleaned_dataset/data/00005.csv")
