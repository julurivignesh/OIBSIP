 Task 2 - Unemployment Analysis with Python

Objective
Performed exploratory data analysis (EDA) on unemployment data in India, focusing on regional and temporal trends, with special emphasis on the impact of the COVID-19 pandemic on unemployment rates across Indian states.

Tech Stack
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

Dataset
"Unemployment in India" dataset, sourced from Kaggle. Contains monthly estimated unemployment rate, estimated employed population, and estimated labour participation rate for 28 Indian states/regions from 2019 to 2020.

Steps Performed
1. Data loading and cleaning (removed null rows, stripped whitespace from column names, converted date column to proper datetime format)
2. Exploratory Data Analysis - shape, data types, null value check
3. Region-wise average unemployment rate analysis
4. Month-wise unemployment trend analysis
5. Time-series visualization for 3 major states (Delhi, Maharashtra, Tamil Nadu)
6. Bar chart of top 10 states with highest average unemployment
7. Correlation heatmap between unemployment rate, employment, and labour participation rate
8. Pre-COVID vs Post-COVID comparison analysis
9. Written observations added after each visualization

Key Findings
- The average unemployment rate nearly doubled after the COVID-19 outbreak, rising from 9.51% (pre-COVID) to 17.77% (post-COVID)
- Tripura (28.35%) and Haryana (26.28%) recorded the highest average unemployment rates among all states
- April 2020 saw a dramatic spike to 23.64%, directly following India's nationwide COVID-19 lockdown announced on March 25, 2020
- Tamil Nadu and Delhi experienced the sharpest individual spikes (nearing 50%) during April-May 2020
- Unemployment rate showed only a weak correlation with employment numbers (-0.22) and labour participation rate (~0.00), suggesting the relationship is more complex than simple supply-demand dynamics

Files in this Folder
- `task2_unemployment_analysis.ipynb` - Complete Jupyter Notebook with code, visualizations, and analysis
- `README.md` - This file

Author
Juluri Vignesh | Data Science Intern | Oasis Infobyte
