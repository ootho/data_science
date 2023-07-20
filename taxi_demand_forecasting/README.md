# Taxi Orders Prediction

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/taxi_demand_forecasting/taxi_demand_forecating.ipynb)

## Project Objective and Tasks

We have historical data on taxi orders at airports. To attract a sufficient number of drivers during peak load periods, we need to forecast the number of taxi orders for the next hour.  

**Tech Stack: Python, Pandas, Matplotlib, Scikit-learn, CatBoost**

## Conclusion

Four models were trained: linear regression, decision tree, random forest, and gradient boosting. The best result on cross-validation, with an RMSE of 23.76, was achieved by the `CatBoostRegressor` model. On the test set, the RMSE was 46.

The residuals passed the Dickey-Fuller test for stationarity.