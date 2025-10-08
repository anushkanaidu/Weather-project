# Weather project

**Purpose:** This project compares precipitation levels across two U.S. cities (Seattle and Portland) between 2018 and 2022 to analyze rainfall patterns.

## Repository Structure

Weather-project/
│
├── weather/
│ ├── code/
│ │ └── weather.ipynb # Main Jupyter Notebook containing the analysis
│ ├── data/
│ │ ├── seattle_rain.csv # Seattle daily precipitation data (NOAA)
│ │ └── portland_rainfall.csv# Portland daily precipitation data (NOAA)
│ ├── reports/
│ │ └── report.pdf # Final summary report (PDF export)
│ ├── README.md # Project overview
│ └── requirements.txt # List of required Python libraries

## Data 

seattle data:[ https://raw.githubusercontent.com/brian-fischer/DATA-5100/refs/heads/main/weather/seattle_rain.csv ]

portland data:[ https://raw.githubusercontent.com/anushkanaidu/Weather-Data-Project/refs/heads/main/weather/portland_rainfall.csv ]

## Requirements
To run the notebook, install pandas numpy seaborn matplotlib

## Analysis Overview
1. **Data Cleaning:**  
   - Converted date formats for consistency.  
   - Selected relevant columns (`STATION`, `DATE`, `PRCP`).  
   - Checked and handled missing values (imputed using each city’s mean precipitation).  

2. **Data Transformation:**  
   - Merged the two datasets on `DATE` using an **outer join**.  
   - Reshaped data from wide to long format for visualization.  

3. **Visualization & Insights:**  
   - Created line plots and bar charts using Seaborn and Matplotlib.  
   - Compared **mean daily precipitation**, **monthly precipitation trends**, and **proportion of rainy days**.  

4. **Conclusion:**  
   - Seattle experiences rain **more frequently**, but in **smaller amounts**.  
   - Portland has **fewer rainy days**, but with **heavier rainfall overall**.

Author: Anushka Naidu Maddisetty
Course: DATA 5100 – Foundations of Data Science
Institution: Seattle University
