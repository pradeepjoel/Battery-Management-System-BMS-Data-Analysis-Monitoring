Battery Data Analysis
Overview

This project analyzes battery performance data, focusing on voltage, current, and temperature. It includes fault detection for low voltage and over-temperature conditions and visualizes key parameters over time.

Dataset

The analysis uses CSV files containing time-series measurements with the following columns:

Time – Time in seconds

Voltage_measured – Measured battery voltage (V)

Voltage_load – Load voltage (V)

Current_measured – Measured current (A)

Current_load – Load current (A)

Temperature_measured – Measured battery temperature (°C)

Features

Voltage Analysis

Plots measured vs. load voltage over time.

Marks low voltage events (voltage < 2.7 V).

Current Analysis

Plots measured vs. load current over time.

Temperature Analysis

Plots battery temperature over time.

Detects over-temperature events (temperature > 55 °C).

Fault Detection

Flags low voltage and over-temperature conditions.

Provides counts of fault occurrences.

Requirements

Python 3.8+

Pandas

NumPy

Matplotlib

Usage

Place your CSV data in the data/cleaned_dataset/ folder.

Update the file path in the script if necessary:

df = pd.read_csv("../data/cleaned_dataset/data/00005.csv")


Run the script to generate plots and fault analysis.

Example Output

Low voltage events: 7

Over temperature events: 0
