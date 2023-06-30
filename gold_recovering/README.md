# Gold Recovery from Ore

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/yp_gold_recovering/gold_recovering.ipynb)

## Project Objective and Tasks

The goal of this project is to predict the gold recovery coefficient from gold-bearing ore. The model will also help optimize production by avoiding operating with unprofitable characteristics.

**Technological Process**
When the extracted ore undergoes primary processing, it becomes a crushed mixture. It is then sent for flotation (enrichment) and two-stage cleaning:
1. Flotation
The flotation plant receives a mixture of gold-bearing ore. After enrichment, a rough concentrate and "tailings" are obtained, which are residues of the product with a low concentration of valuable metals. The stability of this process is influenced by the inconsistent and suboptimal physicochemical state of the flotation pulp (a mixture of solid particles and liquid).
2. Cleaning
The rough concentrate undergoes two cleaning stages. The final concentrate and new tailings are obtained as outputs.

**Tech Stack: Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn**

## Conclusion

In the first stage, the project data was prepared by:
1. Removing features that are not present in the test set from the training set.
2. Adding corresponding target variables to the test set.
3. Constructing a correlation matrix and removing features with multicollinearity.
4. Preprocessing the data for model training.

In the second stage, data analysis was conducted based on predefined criteria, revealing the following:
1. The concentration of silver decreases at each production stage, while the concentration of gold increases. The concentration of lead increases after the first stage and remains unchanged after the second stage.
2. The size distribution of raw material particles in the training and test sets is slightly different. This difference will not affect the model's quality.
3. The total concentration of all substances increases throughout the cycle.

In the third stage:
1. Formulas for calculating sMAPE (symmetric mean absolute percentage error) and the final sMAPE were derived.
2. Several models, including Linear Regression, Decision Tree Regressor, Random Forest Regressor, and ElasticNet, were trained. Hyperparameters for these models were tuned using gridSearchCV.
3. The best model underwent testing on the test set, achieving a final sMAPE result of 8.58%.
4. The best model is RandomForestRegressor with parameters max_depth=4 and n_estimators=13.