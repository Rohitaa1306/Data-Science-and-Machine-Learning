# K-Means Clustering on Iris Dataset

This repository contains code for applying the k-means clustering algorithm to the Iris dataset. The goal is to partition the dataset into distinct clusters based on sepal length and sepal width.

## Dataset

The Iris dataset is a well-known dataset in machine learning and statistics. The dataset consists of measurements for 150 iris flowers, representing three different species: setosa, versicolor, and virginica. Each species is represented by 50 samples.

### Features

1. **Sepal Length:** Length of the iris flower's sepal (in centimeters).
2. **Sepal Width:** Width of the iris flower's sepal (in centimeters).
3. **Petal Length:** Length of the iris flower's petal (in centimeters).
4. **Petal Width:** Width of the iris flower's petal (in centimeters).

### Target Labels

The target variable is the species of iris, categorized into three classes:

1. **Setosa (0)**
2. **Versicolor (1)**
3. **Virginica (2)**

## Code Overview

## Code Overview

### 1. Data Loading and Visualization

The code starts by loading the Iris dataset and creating a scatter plot to visualize the distribution of iris flowers based on sepal length and sepal width.

### 2. K-Means Clustering Algorithm Implementation

A custom implementation of the k-means clustering algorithm is provided in the `k_means_clustering` class. The algorithm is initialized with parameters such as the number of clusters (k), maximum iterations, and convergence threshold.

### 3. Exploration of Optimal k Value

The code explores the behavior of the k-means algorithm for different values of k. Mean Squared Error (MSE) is used to evaluate clustering performance.

### 4. Clustering Visualization

The results of the k-means clustering algorithm are visualized by plotting clustered data points and final centroids. Different colors represent different clusters.

### 5. MSE Over Iterations

The code generates a plot illustrating how the Mean Squared Error (MSE) changes over the iterations of the k-means algorithm, providing insights into convergence.

## Algorithm Steps
1. Initialize centroids.
2. Assign data points to clusters based on the nearest centroid.
3. Update centroids based on the mean of assigned data points.
4. Repeat steps 2 and 3 until convergence or a maximum number of iterations is reached.
5. Output final cluster centroids and data point assignments.
   
# Mathematical Formulas

## Initialization of Centroids
C_old = initialize_centroids()

## Calculation of New Centroids
C_new = new_centroids(C_old)

## Euclidean Distance
distance(a, b) = square_root(sum((a_i - b_i)^2 for i in range(n)))

## Clustering
clustering(x, centroids) = argmin(distance(x, centroid) for centroid in centroids)

## Mean Squared Error (MSE) for Each Cluster
mse_classes(centroids) = sum(sum(0.5 * ||centroid - a||^2 for a in A_i) for i in range(k))
