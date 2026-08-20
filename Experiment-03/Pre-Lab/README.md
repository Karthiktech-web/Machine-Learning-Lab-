# Experiment 03: Supervised Classification and Performance Assessment

## Pre-Lab Tasks

### 1. What is supervised learning? How is classification different from regression?

Supervised learning is a machine learning technique in which a model learns from labeled data. The input data is provided along with the correct output, and the model learns the relationship between them to make predictions on new data.

Classification predicts categorical or discrete values. For example, predicting whether an email is spam or not spam.

Regression predicts continuous numerical values. For example, predicting the price of a house.

Therefore, classification produces class labels, while regression produces continuous numerical values.

---

### 2. Explain the working principle of any two classification algorithms.

#### Logistic Regression

Logistic Regression is a classification algorithm that predicts the probability of an input belonging to a particular class. It uses the sigmoid function to convert the model output into a probability between 0 and 1. A suitable threshold is then used to assign the input to a class.

#### k-Nearest Neighbors (k-NN)

k-Nearest Neighbors is a distance-based classification algorithm. For a new data point, it identifies the k nearest training data points using a distance measure such as Euclidean distance. The class that occurs most frequently among the nearest neighbors is assigned to the new data point.

---

### 3. What is a confusion matrix? Why is it used in evaluating classification models?

A confusion matrix is a table used to evaluate the performance of a classification model by comparing the actual class labels with the predicted class labels.

For binary classification, it consists of:

- True Positive (TP): Correctly predicted positive samples.
- True Negative (TN): Correctly predicted negative samples.
- False Positive (FP): Negative samples incorrectly predicted as positive.
- False Negative (FN): Positive samples incorrectly predicted as negative.

A confusion matrix helps identify the errors made by a classification model and is used to calculate metrics such as accuracy, precision, recall, and F1-score.

---

### 4. What is cross-validation, and how does it help improve the reliability of model evaluation?

Cross-validation is a model evaluation technique in which the dataset is divided into multiple subsets called folds. The model is trained using some folds and evaluated using the remaining fold. This process is repeated so that each fold is used for validation.

In k-fold cross-validation, the performance scores from all folds are averaged to obtain the final performance estimate.

Cross-validation improves the reliability of model evaluation because it evaluates the model using different training and validation subsets. It reduces dependence on a single train-test split and provides a more reliable estimate of how the model will perform on unseen data.