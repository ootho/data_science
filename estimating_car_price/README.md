# Estimating Car Price

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/estimating_car_price/car_price.ipynb)

## Project Objective and Tasks

We have historical data available of a car marketplace, including technical specifications, configurations, and prices of cars. Our goal is to build a model for predicting car prices.

The client values the following aspects:
- Prediction quality
- Prediction speed
- Training time

**Tech Stack: Python, Pandas, Scikit-learn, Optuna, LightGBM, CatBoost**

## Conclusion

During the project, we performed analysis and preprocessing of the raw data. 
We trained four different models on the processed data. 
For each model, we selected hyperparameters that showed the best performance based on the `RMSE` metric. 
We conducted an analysis of the training quality and time for the best models and selected the following two:
- LightGBM - if prioritizing `RMSE`
- DecisionTree - if prioritizing training and prediction speed.