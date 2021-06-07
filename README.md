# R-Time-Series-Met-Temperatures

## Time series analysis in Base R

There are many packages around to handle, estimate and predict on time series data, including popular packages `forecast` and `astsa`.

However, it is useful for a deeper understanding to be able to perform time series analysis without reliance on pre-built packages. This project is an attempt to do exactly that!

## Method
Temperature data is pulled from the Met Office website, and trends are estimated (linear to cubic), seasonality estimated (using both a seasonal means method and sine-cosine 'harmonics' method to order-6), and then ARMA models (to order 3,3) are estimated. These are all built on data from 1884 to 2019, and tested for accuracy (using an RMSE function) on actual temperatures in 2020, with surprising results!
