# Detection of Toxic Comments

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/yp_toxic_comments/toxic_comments.ipynb)

## Project Objective and Tasks

The online store `WikiShop` is launching a new service where users can edit and supplement product descriptions, similar to wiki communities. This means that customers can suggest their edits and comment on changes made by others. The store needs a tool that can identify toxic comments and send them for moderation.

We have a dataset with labels indicating the toxicity of the edits. The goal is to train a model that can classify comments as positive or negative.

During the project, we will use traditional machine learning models and also explore `toxic-BERT` model.

**Tech Stack: Python, Pandas, Scikit-learn, CatBoost, NLTK, PyTorch**

## Conclusion

`Toxic-BERT` out of the box, without fine-tuning, achieved an F1 score of 0.84, while the best result among the classical models was obtained by `LogisticRegression` with an F1 score of 0.80 on the test set. If there are no strict time requirements, we can use `Toxic-BERT`, otherwise, `LogisticRegression` would be a suitable choice.