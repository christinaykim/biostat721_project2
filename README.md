# Project 2: Air Pollution and Sickle Cell Disease  
**Biostat 721: Introduction to Statistical Programming I — Duke University**

---

## Project Overview  
This project investigates air pollution trends in **Durham County, NC (Jan 2018 – Apr 2020)** to support research on the relationship between **environmental exposure and sickle cell disease (SCD)**.  
Using daily measurements of **CO**, **PM2.5**, and **O₃** concentrations from the **EPA monitor at RDU Airport**, the analysis focuses on cleaning, summarizing, and visualizing temporal air quality patterns.

---

## Data Processing Function  
An R function was written to process raw pollutant data for each year.  
The function performs the following steps:
- Renames pollutant columns with concise, descriptive variable names  
- Converts and formats the date variable  
- Averages multiple daily measurements per pollutant  
- Removes duplicate rows  
- Replaces negative pollutant values with zero  

The function was applied to three yearly datasets (`AQ_2018`, `AQ_2019`, `AQ_2020`), producing cleaned data suitable for analysis and visualization.

---

## Visualizations  
Two main plots were created to summarize and explore pollutant trends:

1. **Monthly Average CO and O₃ (2018–2020)**  
   Displays mean monthly concentrations with **95% confidence intervals**, using different colors for each pollutant.

2. **Monthly Average PM2.5 by Year**  
   Shows average monthly PM2.5 concentrations **colored and faceted by year**, highlighting seasonal and yearly variability.

All plots were created in **R** using `ggplot2` with thoughtful design choices (legends, labels, color palettes, and readability).

