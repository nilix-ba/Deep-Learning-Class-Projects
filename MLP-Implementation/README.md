# MLP Implementation for Classification

## Introduction

This Python script implements a Multi-Layer Perceptron (MLP) for image classification using TensorFlow and NumPy. The goal of this implementation is to classify images into different categories based on the provided datasets (Fashion Mnist).

The code comprises several key components:
- Loading and preprocessing image data.
- Defining the architecture of the neural network with configurable hyperparameters.
- Training the MLP model using mini-batch gradient descent with weight decay.
- Fine-tuning hyperparameters to achieve the best performance.
- Evaluating the model on test data and calculating accuracy, bias, and variance.

## Dependencies

- The script utilizes TensorFlow and NumPy for neural network operations and data manipulation. Make sure to install these libraries before running the code.

## Data Preprocessing

- The script normalizes pixel values to a range between 0 and 1, enhancing training efficiency.
- Images are flattened from their original 2D shape to 1D vectors.
- Labels are converted to one-hot encoding for categorical representation.

## Architecture

- The neural network architecture consists of an input layer, a hidden layer, and an output layer.
- Activation functions include ELU (Exponential Linear Unit) for the hidden layer and softmax for the output layer.
- Weight decay (L2 regularization) is employed to control overfitting.

## Training

- The training function utilizes mini-batch gradient descent for optimization.
- Weight updates are performed based on gradients and hyperparameters.
- Training progress is tracked with loss and accuracy metrics for each epoch.

## Hyperparameter Tuning

- The script fine-tunes hyperparameters like learning rate, weight decay, and hidden layer size to optimize model performance.
- The relationships between bias, variance, and these parameters are explored.

## Predicting Test Data

- After training, the model predicts test data and calculates accuracy, bias, and variance on the test set.

## Results

- The script outputs the accuracy of the model on the test data, bias, and variance.
- Use these metrics to assess the quality of your MLP model for image classification.
