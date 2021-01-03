# Cryptocurrency_Prices

### Data
The dataset is obtained from Kaggle which has historical cryptocurrency Prices for all tokens between 28 Apr 13 and 30 Nov 18. All historic open, high, low, close values for all cryptocurrencies are included in this data. 

The total obser- vation of data set is 942,297 with 11 features as follow:
• Slug: name of crypto currency symbol
• Symbol: A symbol given to cryptocurrency
• Name: name of crypto currency
• Ranknow : current rank of crypto currency in the world • Open : opening price of crytocurrency for the day
• High : peak price of cryptocurrency for the day
• Low : least price of cryptocurrency for the day
• Close : closing price of cryptocurrency for the day
• Market : volume currently in circulation in market


### Task 

• Examine auto-correlation with cryptomarket prices (BTC)
• Models using Linear regression and multiple regression, SES, SES holt, ARIMA,Naive forecasts.
• Residual analysis
• Framing hypothesis & p-value
• Try to analyse trend and seasonality in BTC Prices
• Fromtheaboveinsights,useamodelsuchasARIMAand compare it with naive forecasts.


### Model

- Linear Regression
- Simple Exponential forecasting model(SES) 
- ARIMA

### Result
This is all model of results measured by three criteria: 

- Mean Error (ME)
- Root Mean Square Error (RMSE)
-  Mean Average Error (MAE)

Surprisingly, Naive always have better performance, having lowest ME, RMSE, and MAE. 
The reason for this is possibly because BTC’s daily prices resemble a white noise series. Given a short forecasting window like 1 day, the naive forecast yields the best results, as it simply uses the previous day’s price as forecast. On the other hand, 
In the particular domain of crypto currency, it is possible that ARIMA and SES forecast method has higher forecast errors than the naive model because those two models have used more than 1-day previous data to forecast.


### References

- Data Source Kaggle : Every Cryptocurrency Daily Market Price 
( https://www.kaggle.com/jessevent/all-crypto-currencies ) 
- Cryptocurrency Predictions with ARIMA 
( https://www.kaggle.com/taniaj/cryptocurrency-predictions-with-arima )
- Autocorrelation ( https://en.wikipedia.org/wiki/Autocorrelation )
- A Gentle Introduction to Exponential Smoothing for Time Series Forecasting in Python 
( https://en.wikipedia.org/wiki/Autocorrelation )
- ARIMA models ( https://otexts.com/fpp2/arima.html ) 
