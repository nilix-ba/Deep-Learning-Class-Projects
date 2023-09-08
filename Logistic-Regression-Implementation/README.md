# logistic regression Implementation - Titanic Survival Prediction

## Introduction

This Python script, authored by Niloufar Baba Ahmadi, is part of MiniProject3, which focuses on predicting the survival of passengers aboard the Titanic. The dataset used for this project is provided in the 'train.csv' file. The objective is to develop a predictive model to determine whether a passenger survived or not based on various features such as age, gender, ticket class, and more.

The script employs data preprocessing techniques, normalization, logistic regression, and K-fold cross-validation to build and evaluate the predictive model. It aims to achieve a balance between model complexity and performance by tuning hyperparameters like learning rate and weight decay.

## Data Preprocessing

- Initial examination of the dataset reveals that some columns, such as 'Age' and 'Cabin,' contain significant null values. These missing values are addressed using statistical methods. 'Cabin' is dropped due to excessive missing data, while 'Age' is imputed with the mean value.
- Irrelevant attributes like 'PassengerId,' 'Name,' and 'Ticket' are removed from the dataset, as they do not contribute to the prediction task.
- Non-numeric columns ('Sex' and 'Embarked') are converted to numeric values to make them compatible with the logistic regression model.

## Logistic Regression

- Logistic regression is employed as the predictive model for this binary classification task.
- The logistic regression algorithm is implemented with gradient descent, and a sigmoid function is used to predict probabilities of survival.
- L2 regularization (weight decay) is incorporated into the loss function to control model complexity and mitigate overfitting.
- The script provides an accuracy metric to evaluate the model's performance.

## K-Fold Cross-Validation

- K-fold cross-validation is utilized to assess the model's robustness and generalization capability.
- The dataset is divided into five folds, with one fold used for validation while the remaining folds are used for training.
- The model is trained and evaluated iteratively for each fold to obtain accuracy, bias, and variance metrics.

## Hyperparameter Tuning

- The script explores different combinations of hyperparameters, including learning rate and weight decay, to fine-tune the logistic regression model.
- Ten iterations of cross-validation are performed for each hyperparameter combination, and evaluation metrics are recorded.

The code is structured to provide insights into the process of building a predictive model, from data preprocessing to hyperparameter tuning. It serves as a valuable resource for understanding and implementing logistic regression for binary classification tasks.

## Usage

1. Ensure you have the required Python libraries installed.
2. Run the script with the 'train.csv' dataset.
3. Examine the output accuracy and hyperparameter tuning results to choose the best model configuration for your Titanic survival prediction task.


