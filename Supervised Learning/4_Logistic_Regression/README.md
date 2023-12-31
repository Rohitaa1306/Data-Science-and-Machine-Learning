# Logistic Regression Implementation and Analysis

## Designing a Single Neuron for Probability Prediction

We aim to create a single neuron model for predicting class probabilities instead of deterministic labels. 

### The Sigmoid Activation Function

The sigmoid function, a differentiable function with a range in [0, 1], is employed for its smooth "S"-shape, ideal for transitioning probability values based on input feature changes.

### Loss and Gradient Descent

The logistic regression model is trained using gradient descent to minimize the cross-entropy loss function. The cost function penalizes the model heavily for high-confidence incorrect predictions, and the goal is to find the values of the weights that minimize this cost function.

### Logistic Regression Implementation on Breast Cancer Dataset

#### Dataset

We utilize the breast cancer dataset from Scikit-learn, aiming to classify tumors as benign or malignant based on their characteristics.

#### Working/Implementation

The logistic regression implementation involves a single output neuron with a sigmoid activation function. Training the neuron includes minimizing the cross-entropy loss using gradient descent. Once parameters are learned, the neuron predicts the probability of the binary outcome for new input vectors.

## Summary

Logistic regression is implemented using a single output neuron with a sigmoid activation function. The neuron takes input features, applies a weighted sum, adds a bias term, and passes the result through the sigmoid function to obtain the predicted probability. Training involves minimizing the cross-entropy loss using gradient descent. Once parameters are learned, the neuron can predict the probability of the binary outcome for new input vectors.
