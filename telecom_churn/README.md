# Customer Churn Prediction for Telecom Operator

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/yp_telecom/yp_telecom.ipynb)

## Project Objective and Tasks

The goal of this project is to create a machine learning model that can predict customer churn with high accuracy, enabling the company to proactively offer promotions and special conditions to retain customers. The target is to achieve a ROC-AUC value of at least 0.85, and accuracy is also an important metric for us.

**Tech Stack: Python, Pandas, Scikit-learn, CatBoost**

## Conclusion

During the training phase, three different models were trained. The `CatBoostClassifier` model performed the best, achieving an accuracy of 0.9 on the test set. This means that the model is capable of predicting 90% of customers who are likely to churn. The predictions will allow the company to take necessary measures to retain customer loyalty.