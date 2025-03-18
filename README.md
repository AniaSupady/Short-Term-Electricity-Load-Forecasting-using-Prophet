# Short-Term-Electricity-Load-Forecasting-using-Prophet
Prophet-based electricity load forecasting: Prepares data, fits model with yearly/weekly seasonality, predicts next 48 hours, and visualizes results.
https://github.com/AniaSupady/Short-Term-Electricity-Load-Forecasting-using-Prophet/blob/main/Energy_Load_Forecasting_(Short_term)_using_CAISO.ipynb

# Load Forecasting Model Approach

The foundation of this model is to predict energy demand (load) accurately over various time horizons. Here’s the approach:

## Data Input for Load Forecasting

### 1. Historical Load Data
- Daily or hourly historical load data from the CAISO database.

### 2. LMP Data
- Day-ahead and real-time locational marginal prices (LMP) to gauge pricing trends and their impact on load demand.

### 3. Renewable Generation Data
- Solar and wind generation data, as renewables can influence load patterns (e.g., high solar generation may reduce grid reliance).

### 4. Weather Data
- Historical weather patterns affecting energy demand, such as temperature, humidity, and solar radiation levels.

---

## Methods for Forecasting

### Short-Term Forecasting (Next 24-72 hours)
1. **Time Series Forecasting**:
   - Use models like ARIMA, Exponential Smoothing (ETS), or Prophet for forecasting hourly or daily load based on historical data.
2. **Machine Learning**:
   - Apply models like Random Forest or XGBoost to predict load considering multiple features like weather, LMP, and renewable generation.

### Long-Term Forecasting (Monthly/Annual)
1. **Regression Models**:
   - Use time series regression models or multivariate regression with features like population growth, economic activity, and historical demand.
2. **Scenario-based Forecasting**:
   - Forecast based on different scenarios (e.g., high renewable growth, shifts in customer behavior).
