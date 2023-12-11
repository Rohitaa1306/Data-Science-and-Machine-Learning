# Linear Regression Implementation

## Overview
This repository contains a simple implementation of linear regression to predict salaries based on years of experience. Linear regression is a supervised machine learning algorithm that models the relationship between a dependent variable (target) and one or more independent variables (features) by fitting a linear equation to the observed data.

## Inner Working of Linear Regression

### 1. Model Representation
The linear regression model is represented by the equation:
Y = β₀ + β₁X₁ + β₂X₂ + ... + βₙXₙ
where:
- Y is the dependent variable (target),
- β₀ is the intercept (bias term),
- β₁, β₂, ..., βₙ are the coefficients (weights),
- X₁, X₂, ..., Xₙ are the independent variables (features).

### 2. Training Process
The model is trained using the gradient descent algorithm to find the optimal values for the coefficients that minimize the mean squared error (MSE) between predicted and actual values. The training involves iteratively updating the weights to minimize the cost function.

### 3. Dataset
The dataset used in this implementation contains information on salaries and years of experience. The goal is to predict salaries based on the number of years of experience.

### 4. Implementation Steps
- Data loading: The dataset is loaded into a Pandas DataFrame.
- Data preprocessing: Features are standardized, and a bias term is added.
- Model training: The linear regression model is trained on the training set.
- Model evaluation: The model's performance is evaluated on the test set using regression metrics.
- Visualization: Scatter plots are used to visualize the relationship between actual and predicted values.

## Dependencies
- NumPy
- Matplotlib
- Seaborn
- Pandas
- scikit-learn

