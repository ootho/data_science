# Age Estimation from Photos (Keras)

[View Notebook](https://nbviewer.org/github/ootho/data_science/blob/main/yp_face_age_recognition_keras/face_age_recognition_keras.ipynb)

## Project Objective and Tasks

The network supermarket "Hleb-Sol" is implementing a computer vision system for processing customer photos. Capturing photos at the checkout area will help determine the age of customers in order to:
- Analyze purchases and suggest products that may interest customers in that age group.
- Control cashiers' compliance when selling alcohol.

**Tech Stack: Python, Pandas, NumPy, Keras**

## Conclusion

The `ResNet50` network pretrained on the `imagenet` dataset was used as the basis. Since the network is initially trained for classification tasks, we replaced the last two layers with `GlobalAveragePooling` and a `Dense` layer with a single output for regression. The Mean Squared Error (MSE) was used as the loss function, and the model was evaluated based on Mean Absolute Error (MAE). The learning rate was set to 0.0001, and no data augmentation was performed.

The achieved MAE on the test set is 6.71, obtained within 3 epochs. This result is sufficient for product recommendations, but not accurate enough to determine the threshold for selling tobacco and alcohol at the age of 18, as the error of 6.7 years is too high.