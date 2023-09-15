# ARIMA-for-Time-Series-Forecasting. 
Auto Regressive Integrated Moving Average (ARIMA) model is among one of the more popular and widely used statistical methods for time-series forecasting. It is a class of statistical algorithms that captures the standard temporal dependencies that is unique to a time series data. In this post, I will introduce you to the basic principles of ARIMA and present a hands-on tutorial to develop ARIMA for time-series forecasting in Python.
What is ARIMA?
Keywords: Stationarity and Autocorrelation
Before we dig right into ARIMA’s formal mathematical definition, let me introduce you to the concept of stationarity. Stationarity simply means observations that do not depend on time. For data that depends on time (eg. seasonal rainfall), the stationarity condition may not hold as different timing will yield different values for these observations.
Another important concept to understanding ARIMA is autocorrelation. How does it different from the typical correlation? First of all, correlation relates two different sets of observations (eg. between housing prices and the number of available public amenities) while autocorrelation relates the same set of observation but across different timing (eg. between rainfall in the summer versus that in the fall).

SARIMA (Seasonal ARIMA). This model is very similar to the ARIMA model, except that there is an additional set of autoregressive and moving average components. The additional lags are offset by the frequency of seasonality (ex. 12 — monthly, 24 — hourly).
SARIMA models allow for differencing data by seasonal frequency, yet also by non-seasonal differencing. Knowing which parameters are best can be made easier through automatic parameter search frameworks such as pmdarina.

SARIMA (Seasonal Auto-Regressive Integrated Moving Average) is an extension of the ARIMA (Autoregressive Integrated Moving Average) model that incorporates seasonality in addition to the non-seasonal components. ARIMA models are widely used for time series analysis and forecasting, while SARIMA models are specifically designed to handle data with seasonal patterns.
 
ARIMAX and SARIMAX

These models take into account exogenous variables, or in other words, use external data in our forecast. Some real-world examples of exogenous variables include gold price, oil price, outdoor temperature, exchange rate.
It is interesting to think that all exogenous factors are still technically indirectly modeled in the historical model forecast. That being said, if we include external data, the model will respond much quicker to its affect than if we rely on the influence of lagging terms.


 

