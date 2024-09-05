# Time Series Forecasting for Jakarta's Charitable Ambulance Service

## Project Overview
This project focuses on developing a forecasting model for Jakarta's 118 ambulance service to optimize crew scheduling and resource allocation. Using nearly six years of historical call data (01/01/17 to 23/10/22), we forecast the upcoming eight weeks' demand (24/10/22 to 18/12/22), uncover seasonality patterns, and identify prevailing trends.

## Key Features
- Comprehensive data exploration and visualization
- Time series decomposition analysis
- Implementation and comparison of multiple forecasting models:
  - Naive
  - Single Exponential Smoothing (SES)
  - Holt Linear
  - Simple Linear Regression
  - ARIMA
  - TBATS

## Data
The dataset comprises 3,742 observations of ambulance call data from January 1, 2017, to October 21, 2022. Each entry includes the date and time of the incoming call.

## Methodology
1. Data Preprocessing:
   - Handling missing values
   - Aggregating data into weekly call volumes

2. Exploratory Data Analysis:
   - Time series plots
   - Seasonal decomposition
   - ACF and PACF plots

3. Model Implementation:
   - Baseline models (Naive, SES)
   - Trend models (Holt Linear, Simple Linear Regression)
   - Complex models (ARIMA, TBATS)

4. Model Evaluation:
   - Mean Absolute Percentage Error (MAPE)
   - Root Mean Square Error (RMSE)
   - Ljung-Box test for residual autocorrelation

## Results
The TBATS model demonstrated the best performance, capturing complex patterns and seasonality in the data. Key findings include:
- Weekday call peaks on Mondays, Wednesdays, and Thursdays
- Lower call volumes on weekends
- Busiest hours: 5:00 AM - 6:00 AM and 10:00 AM - 11:00 AM
- Overall downward trend in call volumes from 2017 to 2022

## Repository Structure
- `data/`: Contains the dataset
- `scripts/`: R scripts for data preprocessing, analysis, and modeling
- `results/`: Output files, including forecasts and performance metrics
- `figures/`: Visualizations and plots
- `poster/`: Final A2 poster presentation

## Usage
1. Clone the repository
2. Install required R packages: `install.packages(c("forecast", "ggplot2", "dplyr", "plotly"))`
3. Run the R scripts in the `scripts/` directory

## Future Work
- Incorporate external factors (e.g., weather, events) into the forecasting model
- Develop a more granular forecast (e.g., daily or hourly predictions)
- Implement machine learning models for comparison

## Contributors
- Eshaq Rahmani

## Acknowledgments
- Jakarta's 118 ambulance service for providing the dataset
- Cardiff University School of Mathematics for project supervision
