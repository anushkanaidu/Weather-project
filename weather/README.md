# Weather project

***Purpose:*** This project compares precipitation levels across two U.S. cities (Seattle and Portland) between 2018 and 2022 to analyze rainfall patterns.
---
## Project Overview

This project compares rainfall patterns between **Seattle, WA** and **Portland, OR** using daily precipitation data from **2018 to 2022**.  
It explores which city experiences heavier rainfall overall and which one rains more frequently.  
By cleaning, merging, and analyzing real NOAA climate data, the project provides visual insights into rainfall trends and seasonal variations across both cities.

**Objective:**  
To determine which city is wetter overall by comparing total precipitation, rainfall frequency, and seasonal patterns.

**Domain:**  
Environmental Data Analysis / Climate Studies

**Key Techniques:**  
Data Cleaning, Missing Value Imputation, Data Transformation (Reshape & Merge), Data Visualization using **Pandas**, **NumPy**, **Seaborn**, and **Matplotlib**.
---
## Repository Structure

Weather-project/
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
---
## Data 

seattle data:[ https://raw.githubusercontent.com/brian-fischer/DATA-5100/refs/heads/main/weather/seattle_rain.csv ]

portland data:[ https://raw.githubusercontent.com/anushkanaidu/Weather-Data-Project/refs/heads/main/weather/portland_rainfall.csv ]
---
## Requirements
To run the code, install pandas numpy seaborn matplotlib
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

The analysis shows clear differences between rainfall patterns in Seattle and Portland from 2018 to 2022.

- **Seattle** experiences rain more often, meaning it has a higher number of rainy days throughout the year.  
- **Portland** receives more total rainfall overall — when it rains, it tends to rain harder.  
- Both cities follow similar seasonal patterns, with the most rain falling between **November and February** and the least rain during the **summer months**.
---
## Authors
**Anushka Naidu Maddisetty** – [@anushkanaidu](https://github.com/anushkanaidu)

---

## License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

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
