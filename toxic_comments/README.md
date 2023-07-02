# Detection of Toxic Comments

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/toxic_comments/toxic_comments.ipynb)

## Project Objective and Tasks

The goal is to train a model that can classify comments as positive or negative.  
During the project, we will use classic machine learning models and also explore `toxic-BERT` model.  

**Tech Stack: Python, Pandas, Scikit-learn, CatBoost, NLTK, PyTorch**

## Conclusion

`Toxic-BERT` out of the box, without fine-tuning, achieved an F1 score of 0.84, while the best result among the classical models was obtained by `LogisticRegression` with an F1 score of 0.80 on the test set. If there are no strict time requirements, we can use `Toxic-BERT`, otherwise, `LogisticRegression` would be a suitable choice.