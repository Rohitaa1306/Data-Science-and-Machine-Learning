# Gradient Descent Implementation

## Task
Implement batch gradient descent from scratch to perform classification between benign or malignant tumors using the Breast Cancer dataset from Scikit-learn datasets.

## Dataset
The breast cancer dataset is part of the datasets provided by Scikit-learn. The dataset classifies tumors as benign or malignant based on their characteristics. The goal is to build a model that accurately classifies tumors as cancerous or not based on these features.

## Working of Gradient Descent
Gradient Descent optimizes a machine learning model's cost function by iteratively adjusting model weights based on the negative gradient of the Mean Squared Error (MSE) loss function. This process continues until a local minimum of the cost function is found.

**Algorithm Steps:**
1. Initialize model weights randomly.
2. Compute the gradient of the MSE loss function.
3. Update weights using the gradient descent update rule.
4. Repeat steps 2-3 until convergence or reaching a maximum number of iterations.

## Summarization
Gradient Descent is a vital optimization algorithm in machine learning, finding the local minimum of the cost function by iteratively adjusting model parameters. The learning rate, a crucial hyperparameter, requires careful tuning to avoid divergence or slow convergence.
