# Weather project.

Purpose: This project compares precipitation levels across two U.S. cities (Seattle and Portland) between 2018 and 2022 to analyze rainfall patterns.

---
## Project Overview

This project explores the question: Does it rain more in Seattle or in Portland?

In this analysis, we will use daily precipitation data from the National Centers for Environmental Information (NOAA) for the years 2018–2022 to compare rainfall patterns between these two cities. (link is provided below)

We will:

- Explore and clean the datasets.
- Handle missing values.
- Generate visualizations and draw observations.
- Compare rainfall frequency and total rainfall intensity between the two cities.
  
By the end of this project, we will determine which city is wetter overall, "Seattle" or "Portland", based on total amount of precipitation.

---
## Repository Structure

Weather-project/

    ├── weather/                # Core project folder

    ├── code/                   # Jupyter notebooks and Python scripts
    
    ├── data/                   # Raw and processed data
    
    ├── License                 # Project license
    
    ├── Weather Report.pdf      # Generated report and visualizations
    
    ├── requirements.txt        # Dependencies
    
    └── README.md               # Project documentation 

---
## Data

The precipitation data sets were downloaded from the [**National Centers for Environmental Information NOAA Climate Online Data tool**](https://www.ncei.noaa.gov/cdo-web/search?datasetid=GHCND).


Seattle data source:  
[https://raw.githubusercontent.com/brian-fischer/DATA-5100/refs/heads/main/weather/seattle_rain.csv](https://raw.githubusercontent.com/brian-fischer/DATA-5100/refs/heads/main/weather/seattle_rain.csv)

Portland data source:  
[https://raw.githubusercontent.com/anushkanaidu/Weather-Data-Project/refs/heads/main/weather/portland_rainfall.csv](https://raw.githubusercontent.com/anushkanaidu/Weather-Data-Project/refs/heads/main/weather/portland_rainfall.csv)

---
## Requirements
To run the code, install pandas, numpy, seaborn and matplotlib.

---
## Analysis

The analysis for this project is done in one notebook: **`weather/code/weather.ipynb`**.  
Follow the steps below to reproduce the results.

1. **Import Libraries**  
   Load all the required Python libraries (`pandas`, `numpy`, `seaborn`, `matplotlib`).

2. **Load Data**  
   Read the Seattle and Portland CSV files from the `data/` folder and check the first few rows.

3. **Clean Data**  
   Convert the `DATE` column to datetime, keep only the needed columns (`STATION`, `DATE`, `PRCP`), and fill missing precipitation values with the average rainfall for each city.

4. **Combine Data**  
   Merge both datasets using the `DATE` column with an *outer join* so all dates from both cities are included.

5. **Reshape Data**  
   Change the data to a long format so it’s easier to compare and plot.

6. **Visualize Results**  
   Create graphs to compare daily, monthly, and seasonal rainfall between Seattle and Portland.

7. **Findings**  
   Summarize which city rains more often and which has heavier rainfall overall.
---

**Note:**  
Run the cells from top to bottom in the notebook. Each step depends on the previous one.

---
## Results

Based on the analysis of precipitation data for Seattle and Portland from 2018 to 2022, we can draw the following conclusions:

Total Rainfall:
Portland received more total rainfall than Seattle during this period.

Frequency vs. Intensity:
Seattle experienced rain on more days overall, but the rainfall was usually lighter.
In contrast, Portland had fewer rainy days, but when it rained, the precipitation was heavier on average.

Seasonal Patterns:
Both cities showed clear seasonal trends where it rained more during the winter months and less during the summer.
However, Portland had higher rainfall peaks during the wet season compared to Seattle.

In summary:
Seattle tends to have rain more often but in smaller amounts, while Portland has fewer rainy days with heavier rainfall, leading to a higher total precipitation overall.

---
## Authors
**Anushka Naidu Maddisetty** – (https://github.com/anushkanaidu)

---

## License
This project is licensed under the **MIT License** – see the ([LICENSE](https://github.com/anushkanaidu/Weather-project/blob/main/weather/License)) file for details.

---

## Acknowledgements
**Tools and Libraries Used:**  
- [Pandas](https://pandas.pydata.org/)  
- [NumPy](https://numpy.org/)  
- [Seaborn](https://seaborn.pydata.org/)  
- [Matplotlib](https://matplotlib.org/)

**Data Source:**  
- [NOAA Climate Data Online](https://www.ncei.noaa.gov/cdo-web/)

**Inspiration and Guidance:**  
- Seattle University **DATA-5100 (Foundations of Data Science)** project template.  
- Course instructor and peers for feedback and support.
