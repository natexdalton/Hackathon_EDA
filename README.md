Air Pollution and Vehicle Travel Analysis
Overview

This project explores the relationship between air pollution and vehicle miles traveled across selected IBX neighborhoods. Using publicly available air quality and transportation data, the analysis visualizes:

The composition of major air pollutants in the area

Trends in vehicle miles traveled over time by neighborhood

The goal is to better understand how driving behavior and pollution coexist spatially and temporally.

Data Description

The dataset includes yearly observations with the following key fields:

Geo Place Name – Neighborhood name

Name – Type of measurement (pollutant or vehicle miles)

Data Value – Observed value

Start_Date – Measurement date

A neighborhood mapping is used to standardize geographic names across the dataset.

Visualizations
1. Composition of Pollutants (Pie Chart)

A pie chart displays the average contribution of three major pollutants across all years and neighborhoods:

Ozone (O3)

Nitrogen dioxide (NO2)

Fine particles (PM 2.5)

The chart highlights how each pollutant contributes to overall air pollution in the area, with Ozone visually emphasized.

2. Vehicle Miles Traveled by Neighborhood (Line Chart)

A line chart shows annual trends in vehicle miles traveled, broken out by neighborhood. This visualization helps identify:

Long-term trends in driving behavior

Differences between neighborhoods over time

Methods

Filter data to selected IBX neighborhoods

Convert dates and extract year

Average pollutant values across neighborhoods and years

Aggregate vehicle miles traveled by year and neighborhood

Visualize results using Matplotlib

Technologies Used

Python

pandas

matplotlib

How to Run

Ensure required libraries are installed:

pip install pandas matplotlib

Load the dataset into a pandas DataFrame (df)

Define neighborhood_map

Run the analysis script to generate the charts

Interpretation

The pie chart provides a snapshot of pollutant composition, useful for understanding relative environmental burden.

The line chart captures how transportation activity has evolved, which may help contextualize pollution patterns.

These visualizations are intended for exploratory analysis, not causal conclusions.

Notes

Pollutant values are averaged without normalization; comparisons reflect relative composition, not health risk weighting.

Vehicle miles traveled are averaged per neighborhood per year.
