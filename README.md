# StockPrice-TimeSeries
Time series analysis is used to help model time based data and forecast future prices and trends.
This Project builds a machine learning model which uses historical stock data to predict future prices using various machine learning techniques.

## Dataset
__Source__: Historical stock price and volume of FACT Ltd.

## Methodology
- Data Preprocessing
- EDA
- Stationarity Checks
- ACF and PACF plots
- Differencing
- Model Training - ARIMA
- Model Training - SARIMAX
- Model evaluation  
Performance Evaluation is done using RMSE, AIC and BIC.
- Forecasting

### ARIMA
An ARIMA model is trained on the Closing price of the stock data and the best parameters for the model is selected. A rolling forecast is done against the test data and the model with the lowest RMSE is selected.

### SARIMAX
The SARIMAX model is trained on the Close price with the Volume data as the exogeneous variable.

### PROPHET
Prophet is a time-series forecasting tool by Meta which automatically handles trends, seasons, missing values and is robust to outliers. It is a powerful tool for time series forecasting especially when there is complex patterns involved.  

PROPHET is trained on the Close price and forecasting is done along the test data.

## Dependencies
- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `statsmodels`
- `scikit-learn`