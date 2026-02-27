[README.md](https://github.com/user-attachments/files/25612691/README.md)

# Air Pollution and Vehicle Travel Analysis

## Overview
This project explores the relationship between **air pollution** and **vehicle miles traveled** across selected IBX neighborhoods. Using publicly available air quality and transportation data, the analysis visualizes:

- The **composition of major air pollutants** in the area  
- **Trends in vehicle miles traveled over time** by neighborhood  

The goal is to better understand how driving behavior and pollution coexist spatially and temporally.

---

## Data Description
The dataset includes yearly observations with the following key fields:

- **Geo Place Name** – Neighborhood name  
- **Name** – Type of measurement (pollutant or vehicle miles)  
- **Data Value** – Observed value  
- **Start_Date** – Measurement date  

A neighborhood mapping is used to standardize geographic names across the dataset.

---

## Visualizations

### Composition of Pollutants (Pie Chart)
A pie chart displays the **average contribution** of three major pollutants across all years and neighborhoods:

- Ozone (O3)  
- Nitrogen dioxide (NO2)  
- Fine particles (PM 2.5)  

This visualization highlights how each pollutant contributes to overall air pollution in the area.

### Vehicle Miles Traveled by Neighborhood (Line Chart)
A line chart shows **annual trends in vehicle miles traveled**, broken out by neighborhood. This visualization helps identify:

- Long-term trends in driving behavior  
- Differences between neighborhoods over time  

---

## Methods
1. Filter data to selected IBX neighborhoods  
2. Convert dates and extract year  
3. Average pollutant values across neighborhoods and years  
4. Aggregate vehicle miles traveled by year and neighborhood  
5. Visualize results using Matplotlib  

---

## Technologies Used
- Python  
- pandas  
- matplotlib  

---

## How to Run
1. Install required libraries:
   ```bash
   pip install pandas matplotlib
   ```
2. Load the dataset into a pandas DataFrame (`df`)
3. Define `neighborhood_map`
4. Run the analysis script to generate the charts

---

## Interpretation
- The **pie chart** provides a snapshot of pollutant composition, useful for understanding relative environmental burden.  
- The **line chart** captures how transportation activity has evolved, which may help contextualize pollution patterns.

These visualizations are intended for **exploratory analysis**, not causal conclusions.

---

## Notes
- Pollutant values are averaged without normalization; comparisons reflect relative composition, not health risk weighting.
- Vehicle miles traveled are averaged per neighborhood per year.
