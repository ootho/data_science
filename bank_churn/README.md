# Bank Customer Churn Prediction

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/bank_churn/bank_churn.ipynb)

Data Source: [kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

## Project Objective and Tasks

For the customer churn analysis project, we need to make predictions on whether a customer will churn in the near future or not. We have historical data on customer behavior and contract terminations with the bank.

**Tech Stack: Python, Pandas, Scikit-learn, CatBoost, NumPy**

## Conclusion

**The following steps were performed during the project:**
- The original dataset was prepared for analysis.
- The model was tested on imbalanced data.
- The model was trained on various balanced samples.
- A function for model and hyperparameter selection was utilized.
- The best model was evaluated on the test set.
- A threshold based on AUC-ROC was determined.

The best model for customer churn prediction is the `CatBoostClassifier` with the following parameters:
- `max_depth` = 4
- `l2_leaf_reg` = 2
- `learning_rate` = 0.05
- `iterations` = 200
- `threshold` = 0.19

The obtained model will successfully predict customer churn in 80% of cases before the customer discontinues services.