# Bike Rental Analysis

## Overview
This project analyzes factors influencing bike rental demand using data from Seoul. It involves data cleaning, exploratory data analysis (EDA), feature engineering, and machine learning to predict bike rental counts, which is the main interest of the project. Although some other parameters can be predicted, like the demand for renting bikes.

## Dataset
- **Source**: Seoul Bike Sharing Data: https://archive.ics.uci.edu/dataset/560/seoul+bike+sharing+demand
- **Features**:
  - Weather conditions (e.g., Temperature, Humidity)
  - Temporal data (e.g., Hour, Seasons, Holidays)
  - Target: `Rented Bike Count`

## Some Key Insights
- Strong correlation between `Temperature` and `Rented Bike Count`.
- Bike rentals peak during morning and evening hours, especially in summer.
- Weather conditions like rainfall negatively impact bike rentals.

## Pipeline
1. **Data Cleaning**:
   - Handled missing values and removed duplicates.
   - Addressed outliers in weather data.
2. **EDA**:
   - Visualized relationships between features and rental demand.
   - Identified seasonal trends and time-based patterns.
3. **Feature Engineering**:
   - Extracted temporal features (e.g., `Hour`, `Weekday`).
4. **Model Building**:
   - Built and tuned regression models (Random Forest, Gradient Boosting).
   - Evaluated models using metrics like MAE, RMSE, and R².

## Results
- Best-performing model: **Gradient Boosting Regressor**:
  - MAE: ~100
  - RMSE: ~163
  - R²: 0.925
- **Linear Regressor** had accuracy of ~0.56

## Requirements
- Python 3.8+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`

Install dependencies:
```bash
pip install -r requirements.txt