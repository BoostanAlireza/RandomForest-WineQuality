# Wine Quality Classification using Random Forest

This project demonstrates a binary classification task using the red wine quality dataset. The original wine quality scores are transformed into a binary label: wines with a quality score of 5 or lower are labeled as 0 (low quality), and those with a score above 5 are labeled as 1 (high quality). A machine learning pipeline is built using a Random Forest classifier to predict wine quality.

## Dataset

- **Source**: [UCI Machine Learning Repository - Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/Wine+Quality)
- **File used**: `winequality-red.csv`
- **Target variable**: `quality_binary` (0: low quality, 1: high quality)

## Features

The dataset contains 11 physicochemical features:

- fixed acidity
- volatile acidity
- citric acid
- residual sugar
- chlorides
- free sulfur dioxide
- total sulfur dioxide
- density
- pH
- sulphates
- alcohol

## Workflow

1. **Data Preprocessing**

   - Load the dataset with pandas
   - Transform the multiclass `quality` column to binary `quality_binary`
   - Split the dataset into training and testing sets

2. **Model Pipeline**

   - Use `StandardScaler` to normalize the features
   - Use `RandomForestClassifier` as the estimator

3. **Hyperparameter Tuning**

   - Define a hyperparameter distribution
   - Use `RandomizedSearchCV` with 5-fold stratified cross-validation to find the best parameters

4. **Evaluation**

   - Print the best parameters and cross-validation score
   - Evaluate the model on the test set using:
     - Accuracy
     - Precision, Recall, F1-score
     - Confusion matrix

5. **Visualization**

   - Display the confusion matrix for test predictions