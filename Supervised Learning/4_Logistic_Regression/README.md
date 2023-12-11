# Logistic Regression Implementation and Analysis

## Designing a Single Neuron for Probability Prediction
We aim to create a single neuron model for predicting class probabilities instead of deterministic labels. The chosen activation function is the sigmoid function due to its differentiable nature and its suitability for transforming pre-activation values into probability representations.

### The Sigmoid Activation Function
The sigmoid function, defined as σ(z) = 1 / (1 + e^(-z)), is employed for its smooth "S"-shape, ideal for transitioning probability values based on input feature changes.

### Loss and Gradient Descent
The logistic regression model is trained using gradient descent to minimize the cross-entropy loss function. The cost function is given by:
$$
\[ J(\theta) = -\frac{1}{m}\sum_{i=1}^{m}[y^{(i)}\log(h_\theta(x^{(i)})) + (1 - y^{(i)})\log(1 - h_\theta(x^{(i)}))] \]
$$
where \(m\) is the number of samples, \(y^{(i)}\) is the true label for sample \(i\), \(h_\theta(x^{(i)})\) is the predicted label for sample \(i\), and \(\theta\) is the vector of weights.

## Logistic Regression Model
Building a logistic regression model from scratch involves using a sigmoid function to map input features to the probability of the positive class. The logistic regression equation is:

\[ h_\theta(x) = \frac{1}{1 + e^{-(\theta^Tx)}} \]

Here, \(h_\theta(x)\) is the predicted class probability, σ is the sigmoid function, \(\theta_0\) is the bias term, and \(\theta_1\) to \(\theta_n\) are the weights for features \(x_1\) to \(x_n\).

### Logistic Regression Algorithm
The logistic regression algorithm is employed for binary classification, predicting the probability of a binary outcome given input features. It is widely used in various machine learning applications.

![Logistic Regression](images/logistic_regression.png)

## Logistic Regression Implementation on Breast Cancer Dataset
### Dataset
We utilize the breast cancer dataset from Scikit-learn, aiming to classify tumors as benign or malignant based on their characteristics.

### Working/Implementation
The logistic regression implementation involves a single output neuron with a sigmoid activation function. The mathematical equation for the neuron is expressed as:

\[ z = \theta^Tx + \theta_0 \]

The output is obtained through the sigmoid function:

\[ h_\theta(x) = \frac{1}{1 + e^{-z}} \]

Training involves minimizing the cross-entropy loss using gradient descent. The neuron predicts the probability of the binary outcome for new input vectors after parameter learning.

## Summary
Logistic regression is implemented using a single output neuron with a sigmoid activation function. The neuron takes input features, applies a weighted sum, adds a bias term, and passes the result through the sigmoid function to obtain the predicted probability. Training involves minimizing the cross-entropy loss using gradient descent. Once parameters are learned, the neuron predicts the probability of the binary outcome for new input vectors.

