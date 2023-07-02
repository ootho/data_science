# Recommender System for Mobile Operator Tariffs

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/mobile_recomender/mobile_recomender.ipynb)

## Project Objective and Tasks

The goal is to conduct a preliminary analysis of two tariffs on a small sample of customers and determine which tariff is more promising for the operator.  

**Tech Stack: Python, Pandas, Seaborn, Scikit-learn, SciPy**

## Conclusion

During the project, the optimal model for the given task was selected. Three different models were trained on the training set, and the model that performed the best was identified through testing on the validation set. Specifically, the `RandomForestClassifier` achieved an accuracy of 0.89.

The best model was then tested on the test set, showing a good result of 0.88. The model also passed a sanity check to ensure its adequacy.