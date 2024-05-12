## Overview
Time Series data are collected based on certain periods which have constant values (e.g., daily, weekly, or monthly). Prediction is one of the objectives of the time series analysis by identifying the model from previous data and assuming the current information will also occur in the future.

## Goal
In this project, our goal is to measure how daily temperatures affect electricity demand for a region. We will also predict how accurately temperature can be used to forecast the demand in mid-term (8 weeks/2 months).

## Objective
1. Describe the data set, the variables, and the basic hypotheses you wish to test.
2. Plot the time series data.
3. Report and summarize the auto-correlations and the cross-correlations.
4. Report and summaries the spectral analysis of each series.
5. Fit a linear dynamic model to the data and compare several competing models.
6. Analyze the findings using predictive modeling and relate these to the initial hypothesis.

## Techniques/Models
1. Techniques:
   - Periodogram of residuals
   - Auto-correlation and Spectral Density
   - Cross-correlation and Coherence
   - F-Test/Analysis of Variance (ANOVA) Test
   - A/B Testing
   - AIC/BIC metric
2. Models:
   - Linear Difference Equations with different orders (lags) and cyclic components
   - Auto Regressive Moving Average (ARMA/ARMAX) with different orders (lags) and cyclic components

## Observations
Since our goal was to see how well the model can be used for forecasting, we used the first 300 datapoints for estimating the model parameters and latter 65 datapoints, i.e., 8 weeks/2 months for forecasting. We learnt that the model does a pretty good job in predicting the future values of demand for the first few cycles. The performance degrades for future time points which is expected since ARIMA works for short/mid-term and not long-term predictions.

## Conclusion
We were able to infer that daily temperatures works well in estimating the electricity demand over time. Since our data was for one year, we were restricted by number of predictors which could be taken into consideration. If data is available for more time points, it would be interesting to see how the other factors like humidity and holidays affect the demand.

