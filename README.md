 📈 Predictive Analytics Using Historical Data
Forecasting Air Passenger Trends with Machine Learning & Time Series Models

📌 Project : 

This project builds a complete end-to-end Predictive Analytics pipeline using real-world historical airline passenger data. The goal is to analyze historical trends and use multiple machine learning and time-series models to forecast future passenger numbers.

The dataset used is the classic Air Passengers Dataset (`AirPassengers.csv`), which contains monthly international airline passenger counts from January 1949 to December 1960 — a total of 144 months of data.

🔄 Workflow
```text
START
  │
  ├── STEP 1 ──► Setup
  │               Install Prophet and Statsmodels
  │               Import all libraries
  │
  ├── STEP 2 ──► Data Loading
  │               Upload AirPassengers.csv
  │               Rename #Passengers → Passengers
  │               Convert Month to datetime format
  │               Set the month as the index
  │
  ├── STEP 3 ──► Exploratory Data Analysis
  │               Check shape, data types, and missing values
  │               Statistical summary (min, max, mean, median)
  │               Identify the busiest year and busiest month
  │
  ├── STEP 4 ──► Data Visualization
  │               Raw time series line chart
  │               Rolling 12-month mean overlay
  │               Yearly growth bar chart
  │               Monthly seasonality chart
  │
  ├── STEP 5 ──► Preprocessing and Feature Engineering
  │               Extract Year, MonthNum, TimeIndex
  │               Create Lag_1  → previous month passengers
  │               Create Lag_12 → same month last year
  │               Create Rolling_3 → 3-month rolling average
  │               Split → 80% Training | 20% Testing
  │
  ├── STEP 6 ──► Train Models
  │               │
  │               ├── ML Models
  │               │     Model 1 → Linear Regression
  │               │     Model 2 → Random Forest (200 trees)
  │               │
  │               └── Time Series Models
  │                     Model 3 → ARIMA (5, 1, 0)
  │                     Model 4 → Facebook Prophet
  │
  ├── STEP 7 ──► Model Evaluation
  │               Calculate MAE, RMSE, and R² for each model
  │               Print comparison table
  │               Bar chart comparing MAE scores
  │
  ├── STEP 8 ──► Visualize Predictions
  │               Actual vs Predicted for all models
  │               Prophet 3-year future forecast chart
  │               Confidence interval shading
  │               Seasonal component chart
  │
  └── STEP 9 ──► Export Results
                  Save forecast to CSV
                  Auto-download to the local computer

END
```
 📂 Project Structure

```text
📦 Predictive-Analytics-Air-Passengers/
│
├── 📄 README.md
├── 📊 AirPassengers.csv
├── 📓 Predictive_Analytics_Notebook.ipynb
│
├── 📁 images/
│   ├── 01_raw_time_series.png
│   ├── 02_yearly_growth_bar_chart.png
│   ├── 03_monthly_seasonality_chart.png
│   ├── 04_seasonal_decomposition.png
│   ├── 05_linear_regression_actual_vs_predicted.png
│   ├── 06_random_forest_actual_vs_predicted.png
│   ├── 07_arima_actual_vs_forecasted.png
│   ├── 08_prophet_future_forecast.png
│   ├── 09_prophet_seasonal_component.png
│   └── 10_model_mae_comparison.png
│
└── 📁 outputs/
    └── 📄 AirPassengers_Forecast_Results.csv
```
 🎯 Conclusion

This project successfully demonstrates a complete predictive analytics workflow on real-world historical data.





