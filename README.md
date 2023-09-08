# Deep-Learning-Class-Projects
=======
# Pocket Algorithm Implementation

## Table of Contents
- [Introduction](#introduction)
- [Imports](#imports)
- [Reading the Train Set](#reading-the-train-set)
- [Plotting the Train Set](#plotting-the-train-set)
- [Classification Function](#classification-function)
- [Error Calculation Function](#error-calculation-function)
- [Pocket Algorithm Implementation](#pocket-algorithm-implementation)
- [Training the Model](#training-the-model)
- [Decision Boundary Plotting](#decision-boundary-plotting)
- [Reading the Test Set](#reading-the-test-set)
- [Plotting the Test Set](#plotting-the-test-set)
- [Evaluating the Model on the Test Set](#evaluating-the-model-on-the-test-set)
- [Decision Boundary Plotting on the Test Set](#decision-boundary-plotting-on-the-test-set)
- [Results Summary](#results-summary)

## Introduction
The code includes the implementation of the Pocket algorithm for binary classification on a given dataset, along with various functions and visualizations to understand the algorithm's behavior and evaluate its performance.

## Imports
The code begins with necessary imports, including `pandas` for data manipulation, `numpy` for numerical operations, and `matplotlib` for data visualization.

## Reading the Train Set
The code reads the training dataset from a CSV file named 'train.csv' using the `pd.read_csv` function and displays the first 10 rows of the dataset using `df_train.head(10)`.

## Plotting the Train Set
The code generates a scatter plot of the training dataset, where data points with target label '1' are shown in green, and data points with target label '0' are shown in firebrick color.

## Classification Function
The `classified` function calculates the predicted output based on given weights (`w_1` and `w_2`), input features (`x_train`), data index (`i`), and bias (`b`). It employs a simple sign activation function to make binary predictions.

## Error Calculation Function
The `Error` function calculates the classification error of the model by comparing the predicted values with the actual target values. The error is computed as the fraction of misclassified data points in the dataset.

## Pocket Algorithm Implementation
The `Pocket` function implements the Pocket algorithm, which is an iterative approach for updating weights and bias to minimize classification errors. It runs for a specified number of iterations (`T`) and includes learning rate (`a`) as a parameter. The algorithm tracks the best-performing weights and bias while iterating.

## Training the Model
In this section, the code trains the model using the Pocket algorithm. It initializes random weights (`w1`, `w2`) and bias (`bias`) and runs the algorithm for a total of 10 iterations with 4000 iterations each time. It records the weights, bias, classification error, and the number of iterations for each run.

## Decision Boundary Plotting
This section calculates the slopes and intercepts for the decision boundaries based on the obtained weights and bias. It then generates a series of plots, each showing the decision boundary and the scatter plot of the training data for different iterations.

## Reading the Test Set
The code reads the test dataset from a CSV file named 'test.csv' using the `pd.read_csv` function and displays the first 10 rows of the dataset using `df_test.head(10)`.

## Plotting the Test Set
Similar to the training set, this section generates a scatter plot of the test dataset, where data points with target label '1' are shown in green, and data points with target label '0' are shown in firebrick color.

## Evaluating the Model on the Test Set
The code evaluates the trained model's performance on the test set. It calculates the classification error for each set of weights and bias obtained during training and records these errors in `test_error_list`.

## Decision Boundary Plotting on the Test Set
This section is similar to the decision boundary plotting for the training set but focuses on the test set. It calculates and plots decision boundaries for the different sets of weights and bias obtained during training.

## Results Summary
Finally, the code compiles the results, including the weights (`w1`, `w2`), bias (`bias`), training error, and test error into a DataFrame and displays the results.

Please note that the code includes comments and explanatory text within the functions to help you understand its functionality.

