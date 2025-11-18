# OLS Regression with Affinity propagation/PCA and momentum strategy
- Dimensionality Reduction: Used Affinity Propagation to identify the 27 clusters that explain the S&P, following which take the 27 centroids and feed this into PCA to create a filtered feature that drives the S&P 500 prices
- Following which, we run linear regression on lagged 5 day and 15 day returns against this PCA portfolio to develop an Orthogonal ML portfolio that explains components that are not currently explained by the S&P 500
## Simple momentum strategy: Implementing a simple momentum strategy using the predicted values from Linear Regression.
### Long Entry: 3-day simple moving average exceeds the 7-day simple moving average by arbitrary threshold 0.1% 
### Short Entry: 7-day simple moving average exceeds the 3-day simple moving average by arbitrary threshold 0.1%
