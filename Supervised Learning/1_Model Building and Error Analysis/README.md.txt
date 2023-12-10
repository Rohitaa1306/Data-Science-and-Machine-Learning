# Perceptron Classifier

## Overview

This project explores the fundamental concept of a perceptron, a simple neural network used for binary classification tasks. 

## Perceptron Structure

### Inputs and Weights

- The perceptron takes binary input signals, each associated with a weight.
- The weighted sum, combined with a bias term, determines the perceptron's decision boundary.

### Activation Function

- The weighted sum is passed through an activation function, producing the final output.

## Learning Process

### Training

- During training, the perceptron learns from labeled training data.
- Weights and bias are adjusted to minimize the error between predicted and true labels.

### Decision Boundary

- The perceptron's weights and bias define a hyperplane that acts as a decision boundary.
- This boundary separates instances of different classes.

## Dataset

### Breast Cancer Dataset

- The perceptron code in this repository uses the Breast Cancer dataset from scikit-learn.
- This dataset includes features computed from digitized images of breast masses and is labeled with two classes: malignant and benign tumors.

#### Dataset Information

The Breast Cancer dataset is available in the scikit-learn library. You can find more information about the dataset and how to load it in the [scikit-learn documentation](https://scikit-learn.org/stable/datasets/toy_dataset.html#breast-cancer-dataset).

## Code Implementation

- The `perceptron.ipynb` file contains the Python implementation of the perceptron classifier.
- The code demonstrates the training process and showcases how a perceptron can be used for binary classification tasks.

## Results

The perceptron model achieves the following performance metrics on the Breast Cancer dataset:

- Accuracy: 95.61%
- Precision: 98.53%
- Recall: 94.37%
- F1 Score: 96.40%

These results highlight the model's effectiveness in distinguishing between malignant and benign tumors.

## License

This project is licensed under the [MIT License](LICENSE).
