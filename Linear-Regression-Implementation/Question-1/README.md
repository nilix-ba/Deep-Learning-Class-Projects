# Niloufar Baba Ahmadi 610398103 MiniProject2 Q1

## Table of Contents
- [Introduction](#introduction)
- [Imports](#imports)
- [Reading the Train Set](#reading-the-train-set)
- [Reading the Test Set](#reading-the-test-set)
- [Adding $x_0$](#adding-x_0)
- [Plotting the Train Set](#plotting-the-train-set)
- [Plotting the Test Set](#plotting-the-test-set)
- [Optimal Linear Weight Vector](#optimal-linear-weight-vector)
- [Calculating Cost](#calculating-cost)
- [Poly Plot Function](#poly-plot-function)
- [Linear Regression](#linear-regression)
- [Linear Regression on Test Set](#linear-regression-on-test-set)
- [Polynomial Regression](#polynomial-regression)
- [Polynomial Regression on Test Set](#polynomial-regression-on-test-set)
- [Cost Comparison](#cost-comparison)

## Introduction
This readme file provides an overview of the Python code presented by Niloufar Baba Ahmadi for MiniProject2 Question 1. The code focuses on implementing and comparing linear and polynomial regression models for a given dataset.

## Imports
The code starts by importing the necessary libraries, including `pandas` for data manipulation, `numpy` for numerical operations, `numpy.linalg.inv` for matrix inversion, and `matplotlib.pyplot` for data visualization.

## Reading the Train Set
The code reads the training dataset from a CSV file named 'train_set.csv' and displays the first 10 rows of the dataset using `df_train.head(10)`.

## Reading the Test Set
Similarly, the code reads the test dataset from a CSV file named 'test_set.csv' and displays the first 10 rows of the dataset using `df_test.head(10)`.

## Adding $x_0$
This section explains the addition of a column named 'x_0' to both the train and test datasets. The 'x_0' column is initialized with the value '1'. This column represents the bias term in the regression formula and allows for the calculation of the weight for the bias term.

## Plotting the Train Set
The code generates a scatter plot of the training dataset, with 'x' as the independent variable and 'target' as the dependent variable.

## Plotting the Test Set
Similar to the training set, this section generates a scatter plot of the test dataset.

## Optimal Linear Weight Vector
The code explains the calculation of the optimal linear weight vector using the formula for linear regression. It calculates the weights 'w' based on the training data.

## Calculating Cost
This section defines a function to calculate the Mean Squared Error (MSE) cost for the linear regression model. It computes the cost by comparing the model's predictions with the actual target values.

## Poly Plot Function
A function named 'poly_plot' is introduced, which helps visualize the polynomial regression line with a degree of 5. This function also displays the data frame passed to it.

## Linear Regression
The code applies linear regression to the training data and calculates the weights, bias, and cost for the model. It also provides a visualization of how the linear regression line fits the training data.

## Linear Regression on Test Set
Similarly, this section demonstrates the performance of the linear regression model on the test set.

## Polynomial Regression
The code explores polynomial regression by extending the training data with additional features up to degree 5. It then trains polynomial regression models on subsets of the training data (10, 20, 50, 100, and 200 data points) and calculates the weights, bias, and cost for each model.

## Polynomial Regression on Test Set
This section evaluates the performance of the polynomial regression models on the test set.

## Cost Comparison
The code compares the cost of both linear and polynomial regression models on the training and test sets as the amount of training data increases (from 10 to 200 data points). It visualizes the cost trends for each model.

The provided code and explanations help you understand the implementation and behavior of linear and polynomial regression models on a given dataset. The cost comparisons provide insights into the models' performance as more training data is used, highlighting the trade-off between model capacity and overfitting.
