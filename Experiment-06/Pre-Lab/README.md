# Experiment 06: PCA and Clustering Models

**Name:** R. Karthik  
**Roll No:** 25EU02904

## Pre-Lab Tasks

### 1. What is Principal Component Analysis (PCA), and why is it used for dimensionality reduction?

Principal Component Analysis (PCA) is an unsupervised dimensionality reduction technique used to transform a dataset with many correlated features into a smaller number of new variables called principal components.

The principal components are linear combinations of the original features. The first principal component captures the maximum possible variance in the data, while subsequent components capture the remaining maximum variance while being orthogonal to the previous components.

PCA is used for dimensionality reduction because it can reduce the number of features while retaining most of the important information. It can also reduce computational complexity, remove redundant information, simplify visualization, and make high-dimensional datasets easier to interpret.

---

### 2. What is the difference between original features and principal components in PCA?

Original features are the variables directly measured or collected from the dataset. For example, the Iris dataset contains sepal length, sepal width, petal length, and petal width.

Principal components are new variables created by combining the original features using linear combinations. They are ordered according to the amount of variance they explain.

Therefore, original features have direct meaning in the dataset, while principal components represent transformed directions that capture important patterns and variation in the data.

---

### 3. What is K-Means clustering, and how does it assign data points to different clusters?

K-Means is an unsupervised clustering algorithm that divides data into a predefined number of clusters, represented by k.

The algorithm works by:

1. Selecting k initial cluster centroids.
2. Assigning each data point to the nearest centroid.
3. Recalculating the centroid of each cluster.
4. Reassigning data points based on the updated centroids.
5. Repeating the process until the cluster assignments stabilize or the centroids no longer change significantly.

The objective of K-Means is to minimize the within-cluster sum of squares (WCSS), so that data points within the same cluster are as similar as possible.

---

### 4. Why is feature scaling important before applying PCA and K-Means clustering?

Feature scaling is important because PCA and K-Means are affected by the scale of the input features.

In PCA, features with larger numerical ranges can contribute more strongly to the calculated variance and may dominate the principal components.

In K-Means, distances between data points and cluster centroids are used to assign clusters. A feature with a larger numerical scale can therefore dominate the distance calculation.

Standardization transforms features to have approximately zero mean and unit variance. This allows all features to contribute more fairly to PCA and K-Means clustering.