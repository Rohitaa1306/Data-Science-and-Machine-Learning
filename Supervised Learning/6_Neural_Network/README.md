# Deep Neural Network

## Tasks
1. Build a multilayer feedforward network from scratch and implement it for the Fashion MNIST classification problem.

2. Build a multilayer feedforward network using TensorFlow and Keras for the Fashion MNIST classification problem.

## Dataset Overview
- The Fashion MNIST dataset is a benchmark dataset in machine learning and computer vision research.
- It consists of 70,000 grayscale images of fashion products, categorized into 10 classes.
- Each image is 28x28 pixels.

### Fashion MNIST Classes
1. T-shirt/top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle boot

The dataset is designed as a replacement for the original MNIST dataset, offering more complexity and variability within each category.

## Implementation of a Multilayer Perceptron (MLP)
- A multilayer feedforward network, or MLP, is an artificial neural network with multiple layers.
- It consists of interconnected nodes, each layer fully connected to the next, excluding connections within the same layer.
- MLP architecture examples: 1 Hidden MLP, MultiLayer Perceptron with two hidden layers.

### Mathematical Formulation
- Let `x` be the input, and `y` be the desired output.
- The network has `L` layers, with the first as the input layer, the last as the output, and the rest as hidden layers.
- Output of the `j-th` node in the `i-th` layer is denoted by `a_ij`.
- Weights connecting node `i` in layer `l` to node `j` in layer `(l+1)` are denoted by `w_ij^(l)`.
- Biases of node `j` in layer `(l+1)` are denoted by `b_j^(l)`.

### Output Computation
`a_ij^(l) = activation(w_ij^(l) * a_i^(l-1) + b_j^(l))`

### Loss Function
- Common choice: Mean Squared Error (MSE).
- `MSE = (1/N) * Σ(Σ(y_ij - ŷ_ij)^2)`, where `N` is the number of samples.

### Parameters Update (Stochastic Gradient Descent - SGD)
`w_ij^(l) = w_ij^(l) - α * ∂L/∂w_ij^(l)`
`b_j^(l) = b_j^(l) - α * ∂L/∂b_j^(l)`

### Backpropagation Algorithm
1. Compute gradient of the loss function with respect to the output layer.
2. Compute gradients for subsequent layers in reverse order.
3. Update weights and biases using SGD.

### Hyperparameters Adjustment
- Number of layers, nodes in each layer, activation functions.
