# Shampoo Sales Forecasting using ARIMA Model

## Overview
This project analyzes the monthly shampoo sales data over a three-year period and builds an ARIMA time series forecasting model. The goal is to predict future sales accurately by using historical data, and to evaluate the forecasting performance.

## Dataset
- The dataset contains monthly shampoo sales figures for 36 months.
- The "Month" column represents the date in YYYY-MM format.
- The "Sales" column contains shampoo sales values.

## Project Steps
1. **Data Loading & Preprocessing**
   - Load dataset from CSV.
   - Convert "Month" to datetime.
   - Set "Month" as the index and sort it.
   - Ensure the datetime index has a monthly frequency.

2. **Train-Test Split**
   - Use all data except the last 12 months as training data.
   - Use the last 12 months as testing data.

3. **Modeling**
   - Build an ARIMA(1,1,1) model using the training data.

4. **Forecasting & Evaluation**
   - Forecast sales for the test period.
   - Evaluate predictions using Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).

5. **Visualization**
   - Plot actual vs predicted sales for comparison.

## Usage Instructions
- Ensure Python 3.x is installed.
- Required libraries: `pandas`, `numpy`, `matplotlib`, `statsmodels`, `sklearn`.
- Run the provided Python script to see the model performance and plot.

## Notes
- The datetime index must be continuous monthly data without missing dates.
- Warnings related to date frequency and monotonicity are suppressed for cleaner output.
- Modify the ARIMA order `(p,d,q)` if needed based on model diagnostics.

## Contact
For any queries or suggestions, please reach out.

---

**Author:** Kangkan Kalita  
**Course:** B.Tech Computer Science Engineering  
**Semester:** 6th

