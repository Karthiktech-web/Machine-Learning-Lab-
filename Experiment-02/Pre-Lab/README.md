# Experiment 02 – Pre-Lab

## 1. What is supervised learning? How is classification different from regression?

**Supervised Learning** is a machine learning approach where a model learns from labeled data to predict outputs for new inputs.

**Classification** predicts discrete categories or class labels (e.g., Spam/Not Spam, Yes/No).

**Regression** predicts continuous numerical values (e.g., House Price, Temperature).

---

## 2. Explain the working principle of any two classification algorithms.

### Logistic Regression

- Used for binary classification.
- Calculates the probability of a sample belonging to a class using the sigmoid function.
- Classifies based on a threshold (usually 0.5).

### K-Nearest Neighbors (KNN)

- Stores all training samples.
- Finds the K nearest neighbors of a new sample.
- Predicts the majority class among those neighbors.

---

## 3. What is a confusion matrix? Why is it used?

A confusion matrix is a table used to evaluate classification models.

It contains:

- True Positive (TP)
- True Negative (TN)
- False Positive (FP)
- False Negative (FN)

It helps calculate accuracy, precision, recall, and F1-score.

---

## 4. What is cross-validation?

Cross-validation is a model evaluation technique that divides the dataset into multiple folds.

The model is trained on some folds and tested on the remaining fold.

This process repeats several times to obtain a reliable estimate of model performance and reduce overfitting.