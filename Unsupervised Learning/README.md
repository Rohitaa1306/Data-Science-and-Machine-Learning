# Unsupervised Learning

This folder contains implementations and explanations of various unsupervised learning techniques. Unsupervised learning is a type of machine learning where the algorithm is not provided with labeled training data, and it must find patterns and relationships within the data on its own.

### 1. k-Means Clustering

**Overview:**
k-Means Clustering is an unsupervised learning algorithm designed for partitioning a dataset into K distinct, non-overlapping subsets or clusters. The objective is to group similar data points together, forming clusters based on their proximity to each other.

**How it Works:**
1. **Initialization:** Randomly select K initial centroids, serving as the center points for clusters.
2. **Assignment:** Assign each data point to the cluster whose centroid is closest to it.
3. **Update Centroids:** Recalculate the centroids based on the mean of the data points in each cluster.
4. **Repeat:** Iteratively perform steps 2 and 3 until convergence, achieving stable cluster assignments.

### 2. Principal Component Analysis (PCA)

**Overview:**
Principal Component Analysis (PCA) is a dimensionality reduction technique employed in unsupervised learning. It transforms the dataset into a new coordinate system, emphasizing the dimensions with the highest variance and providing a compressed representation of the original data.

**How it Works:**
1. **Covariance Matrix:** Compute the covariance matrix of the original data.
2. **Eigenvalue Decomposition:** Obtain the eigenvectors and eigenvalues of the covariance matrix.
3. **Principal Components:** Select the top-k eigenvectors (principal components) corresponding to the highest eigenvalues to form the new coordinate system.
4. **Data Transformation:** Project the original data onto the selected principal components.
