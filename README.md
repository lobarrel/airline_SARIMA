# Time-Series Analytics - Forecasting Airline Passengers using SARIMA

SARIMA (Seasonal Auto-Regressive Integrated Moving Average) is an extension of the ARIMA (Autoregressive Integrated Moving Average) model that incorporates seasonality in addition to the non-seasonal components. ARIMA models are widely used for time series analysis and forecasting, while SARIMA models are specifically designed to handle data with seasonal patterns.

It adds three new hyperparameters to specify the autoregression (AR), differencing (I) and moving average (MA) for the seasonal component of the series, as well as an additional parameter for the period of the seasonality.

**Trend Elements:**

There are three trend elements that require configuration. They are the same as the ARIMA model, specifically:

p: Trend autoregression order.
d: Trend difference order.
q: Trend moving average order.

**Seasonal Elements:**

There are four seasonal elements that are not part of ARIMA that must be configured; they are:

P: Seasonal autoregressive order.
D: Seasonal difference order.
Q: Seasonal moving average order.
m: The number of time steps for a single seasonal period. For example, an S of 12 for monthly data suggests a yearly seasonal cycle.

**SARIMA notation: SARIMA(p,d,q)(P,D,Q,m)**