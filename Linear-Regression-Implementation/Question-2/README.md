# Niloufar Baba Ahmadi 610398103 MiniProject2 Q2

## Table of Contents
- [Introduction](#introduction)
- [Imports](#imports)
- [Reading the Train Set](#reading-the-train-set)
- [Reading the Test Set](#reading-the-test-set)
- [Adding $x_{0}$](#adding-x_0)
- [Normalization](#normalization)
- [Normalization of the Train Data](#normalization-of-the-train-data)
- [Optimal Linear Weight Vector for Regression with Regularization](#optimal-linear-weight-vector-for-regression-with-regularization)
- [Calculating Cost](#calculating-cost)
- [Prediction](#prediction)
- [K-Fold Cross Validation](#k-fold-cross-validation)
- [Altering the Sets](#altering-the-sets)
- [Training Phase](#training-phase)
- [Prediction on the Test Set](#prediction-on-the-test-set)

## Introduction
This readme file provides an overview of the Python code presented by Niloufar Baba Ahmadi for MiniProject2 Question 2. The code focuses on implementing regression models with different degrees and regularization strengths, performing K-fold cross-validation, and making predictions on the test set.

## Imports
The code starts by importing the necessary libraries, including `pandas` for data manipulation, `numpy` for numerical operations, `math` for mathematical functions, `numpy.linalg.inv` for matrix inversion, `random.sample` for random sampling, `random` for random operations, and `matplotlib.pyplot` for data visualization.

## Reading the Train Set
The code reads the training dataset from a CSV file and displays the first 10 rows of the dataset using `df_train.head(10)`.

## Reading the Test Set
Similarly, the code reads the test dataset from a CSV file and displays the first 10 rows of the dataset using `df_test.head(10)`.

## Adding $x_{0}$
This section explains the addition of a column named 'x_0' to both the train and test datasets. The 'x_0' column is initialized with the value '1'. This column represents the bias term in the regression formula and allows for the calculation of the weight for the bias term.

## Normalization
The code defines three functions: `E(x)` to calculate the mean of a list, `var(x)` to calculate the variance of a list, and `norm(x)` to normalize a list of values.

## Normalization of the Train Data
The code normalizes the numerical columns of the train dataset using the `norm()` function, excluding the 'x_0' column.

## Optimal Linear Weight Vector for Regression with Regularization
A function `weight(mat_x, mat_y, l)` is defined to calculate the optimal linear weight vector for regression with regularization. The regularization strength 'l' is used to prevent overfitting.

## Calculating Cost
This section defines a function to calculate the Mean Squared Error (MSE) cost for the regression models. It computes the cost by comparing the model's predictions with the actual target values.

## Prediction
A function `predict(mat_x, w)` is defined to make predictions based on the regression formula.

## K-Fold Cross Validation
The code implements K-fold cross-validation, where the dataset is split into five folds, and the model is trained and validated iteratively. The training and cross-validation errors are calculated for each fold.

## Altering the Sets
The code adds extra features to the dataset as required for different polynomial degrees (3 and 5). It creates additional columns for each feature raised to the power of 2, 3, 4, and 5, increasing the complexity of the models.

## Training Phase
The code performs the training phase for regression models with degrees 1, 3, and 5, as well as different values of lambda (0, 1, and 10). It uses repeated 5-fold cross-validation with 10 repetitions to evaluate each model's performance. The training and cross-validation errors are stored in dictionaries for analysis.

## Prediction on the Test Set
Finally, the code selects the best model based on the cross-validation results and uses it to make predictions on the test set. The predictions are saved to a CSV file named 'prediction.csv'.

The provided code and explanations help you understand the implementation and evaluation of regression models with different degrees and regularization strengths. It also demonstrates the importance of cross-validation in model selection and helps you make predictions on new data using the selected model.
