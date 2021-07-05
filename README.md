### **Page available at: https://faisaljina.github.io/R-Time-Series-Met-Temperatures/**
#

# Time series analysis in Base R

There are many packages around to handle, estimate and predict on time series data, including popular packages `forecast` and `astsa`.

However, it is useful for a deeper understanding to be able to perform time series analysis without reliance on these pre-built packages. This project is an attempt to do exactly that!

## Highlights
### Features
- Time Series Modelling
- lapply
- Trend/Seasonality/ARMA modelling
- Forecasting

### Techniques
- Time Series
- Vectorisation
- First Principles Trend & Seasonality Estimation
- Visualisation
- Statistical Analysis

## Method

Temperature data is pulled from the Met Office website, and trends are estimated (linear to cubic), seasonality estimated (using both a seasonal means method and sine-cosine 'harmonics' method to order-6), and then ARMA models (to order 3,3) are estimated. These are all built on data from 1884 to 2019, and tested for accuracy (using an RMSE function) on actual temperatures in 2020, with surprising (but explainable!) results

## Summary
1. Met Office temperature data was loaded from gov.uk, creating 30 time series datasets.
2. EDA was performed including visualisation.
3. Trends were estimated using linear, quadratic and cubic models.
4. Seasonality was estimated using seasonal means and sine-cosine order-6 models, checking for statistical significance.
5. ARMA models were generated on the residuals up to (3,3).
6. Forecasting was compared to a test set and accuracy metrics analysed.
