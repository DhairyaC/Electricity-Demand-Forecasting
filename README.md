## Objective
In this project, we want to measure how daily temperatures affect electricity demand for a region. We will also investigate how accurately temperature can be used to forecast the demand in mid-term (8 weeks/2 months).

## Models
1. Linear Difference Equation
2. Auto Regressive Moving Average Model (ARMA/ARMAX)

## Observations
Since our goal was to see how well the model can be used for forecasting, we used the first 300 datapoints for estimating the model parameters and latter 65 datapoints, i.e., 8 weeks/2 months for forecasting. We learnt that the model does a pretty good job in predicting the future values of demand for the first few cycles. The performance degrades for future time points which is expected since ARIMA works for short/mid-term and not long-term predictions.

## Conclusion
We were able to infer that daily temperatures works well in estimating the electricity demand over time. Since our data was for one year, we were restricted by number of predictors which could be taken into consideration. If data is available for more time points, it would be interesting to see how the other factors like humidity and holidays affect the demand.

