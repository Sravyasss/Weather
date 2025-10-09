# Project Title (This is a template README.md file that you can adapt to your project)

> The purpose of this project is to compare the rainfall in seattle and tampa for 2018-2022. Through this analysis between seattle and tampa dataframes, we explore how often and how much it rains in both seattle and tampa city and identify the significant differences.

---
## Project Overview

Rainfall patterns are rally crucial for us to know as they play an important role various aspects of our day to day life.
This project uses previous precipitation data to from 2018-2022 to identify the rainfall patterns in both seattle and tampa cities.

-> Understanding the precipition and the amount of rainfall in each month in both cities.
-> Compare average precipitation between two contrasting climates of two different cities Seattle and Tampa.
-> Apply statistical tests like t-test and z-test to determine if differences are significant.
-> Visualize the seasonal trends using various plot like histograms, line plots, boxplots, and bar charts.


Objective: To determine whether Seattle receives more rain than Tampa and how the pattern of precipitation differs between the two cities.
Domain: Climate Data analysis 
Key Techniques: Exploratory data analysis, converting datatypes, Imputing missing values, T-tests, Z-test, Visualizing data with matplolib and seaborn.

---
## Project Structure

```
├── data/                 # Raw and processed data
    ├──seattle_rain.csv     
    ├──stl_rain.csv          
    ├──Tampa.csv            
├── code/                 # Jupyter notebooks and Python scripts
    ├──Weather_data.ipynb 
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:**
https://github.com/brian-fischer/DATA-5100/blob/main/weather/seattle_rain.csv #The seattlerain is downloaded from the github.
https://www.ncei.noaa.gov/cdo-web/orders?email=smurala@seattleu.edu&id=4131968 #The source for the city tampa data is taken from this page.

- **Description:**
Size of seattle dataset:129.7+ KB
Size of tampa dataset: 3.6+ MB
key features: Date, precipitation, city
Format: datetime format

- **License:** Public data (NOAA & educational sources)

---

## Analysis

1. It began with Data collection and preparation, where Seattle and Tampa precipitation datasets were brought into pandas, their structure explored using the head(), info(), and describe() functions, and the date column converted to datetime format to extract month and day_of_year to facilitate analysis.
2. In the process of Data cleaning, values for missing precipitation were imputed using monthly averages, and a new binary column any_precipitation was created to verify if it had rained on a given day, month. 
3. The exploratory data analysis (EDA) was focused on viewing rainfall patterns by plotting daily trend plots, monthly histograms, boxplots, and barplots of average precipitation between seattle and tampa cities. 
4.To statistically compare the differences, two-sample t-tests were used to compare mean precipitation and two-proportion z-tests for testing differences in rainy days' numbers, determining months with statistically significant results. Finally, a range of visualizations like line plots, histograms, boxplots, and barplots were implemented to efficiently represent rainfall distributions and highlight major differences between the two cities. These were all performed on the notebook Seattle&tampa_weather_project.ipynb, a jupyter notebook by using the cleaned data clean_seattle_tampa_weather.csv.

Jupyter notebook (.ipynb) file- Seattle&tampa_weather_project.ipynb
Clean file- clean_seattle_tampa_weather.csv

---

## Results

For the seattle dataset, it had more rainy days throughout the year, the number of rainy days were more for seattle compared to tampa.
The Tampa has fewer rainy days overall but significantly heavier rainfall during certain months.
-> Mean daily precipitation and monthly precipitation shows tampa has higher mean precipitation than seattle.
-> Visualizations clearly show the seasonal rainfall patterns for both cities through exploratory data analysis.
-> Several months showed statistically significant differences in precipitation between the two cities.
-> The contingency table states that there are 114 days of precipitation in seattle which is only 33 for tampa.

---

## Author - https://github.com/Sravyasss

---

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---
## Acknowledgements

Tools/Libraries: pandas, numpy, matplotlib, seaborn, scipy, statsmodels
Data Sources: NOAA & GitHub(https://github.com/brian-fischer/DATA-5100) 
Inspiration: Brian Fischer

---