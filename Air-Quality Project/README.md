# Air-Quality Project
#  Air Quality Time Series Analysis

## Overview
This notebook presents a complete workflow for analyzing and forecasting air quality data using time series techniques. The process includes data loading from ARFF files, preprocessing, exploratory analysis, stationarity testing, and forecasting using SARIMA (Seasonal ARIMA) models.

The objective is to transform raw atmospheric measurements into a clean time-indexed dataset and evaluate forecasting performance using statistical models.

---

## Project Workflow

1. **Import Libraries**  
   Uses `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, and `scikit-learn`.

2. **Load Dataset**  
   Reads air quality data from an `.arff` file and converts it into a pandas DataFrame.

3. **Datetime Construction**  
   Combines `year`, `month`, `day`, and `hour` columns into a single `datetime` column.

4. **Data Cleaning & Preprocessing**  
   - Drops unnecessary columns  
   - Handles missing values  
   - Applies time-based interpolation  
   - Groups data by monitoring station (if applicable)

5. **Exploratory Data Analysis (EDA)**  
   - Time series plots  
   - Missing value checks  
   - ACF and PACF plots  
   - Stationarity testing using the Augmented Dickey–Fuller (ADF) test

6. **SARIMA Modeling**  
   - Defines target air quality variable  
   - Splits data into training and testing sets  
   - Fits SARIMAX models  
   - Generates forecasts

7. **Model Evaluation**  
   - Mean Absolute Error (MAE)  
   - Root Mean Squared Error (RMSE)  
   - Visualization of predicted vs actual values

---

##  Requirements

Install the required dependencies:

```bash
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn liac-arff



