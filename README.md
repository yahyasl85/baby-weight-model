# baby-weight-model
model used to predict baby weight
## BigQuery Project: Predicting Baby Weight

**Purpose:**

This project uses BigQuery to build and evaluate a linear regression model for predicting baby weight. The model is trained on the `natality` dataset from the `bigquery-public-data.samples` project. The goal is to identify factors that influence baby weight and to use this information to make predictions about the weight of newborns.

**Methodology:**

1. **Data Preparation:** The `natality` dataset is used for training and prediction. Relevant features such as mother's age, father's age, gestation weeks, plurality, and the baby's sex are selected.
2. **Model Creation:** A linear regression model is created using BigQuery's `CREATE MODEL` statement. The model is trained using the selected features and the baby's weight as the target variable.
3. **Prediction:** The trained model is used to predict the weight of newborns using the `ML.PREDICT` function in BigQuery. Predictions are made on a subset of the `natality` dataset.
4. **Evaluation:** The model's performance is evaluated using metrics such as mean squared error (MSE) and R-squared. This helps to assess the accuracy and reliability of the predictions.

**Results Summary:**

* The linear regression model was successfully trained on the `natality` dataset.
* The model was able to predict baby weight with reasonable accuracy.
* The most influential factors in predicting baby weight were found to be gestation weeks and plurality.
* The model can be used to make predictions about the weight of newborns, which can be valuable information for healthcare professionals and parents.

**Further Development:**

* Explore other machine learning models, such as decision trees or neural networks, to potentially improve prediction accuracy.
* Incorporate additional features from the `natality` dataset, such as birth weight and mother's health indicators, to enhance the model's predictive power.
* Deploy the model as a web service or API to make it accessible to a wider audience.
