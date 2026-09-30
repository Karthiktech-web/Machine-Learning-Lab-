# Experiment 07: Model Validation, Hyperparameter Optimization and Pipelines

**Name:** R. Karthik  
**Roll No:** 25EU02904

## Pre-Lab Tasks

### 1. Difference between training data and testing data

Training data is used to train a machine learning model and learn patterns and relationships between input features and the target.

Testing data is used after training to evaluate how well the model performs on previously unseen data.

The test data should remain unseen during training because using it during model development can cause data leakage and produce an overly optimistic estimate of model performance.

---

### 2. K-Fold Cross-Validation

K-Fold Cross-Validation divides the dataset into K approximately equal parts called folds.

The procedure is:

1. Divide the dataset into K folds.
2. Use K-1 folds for training.
3. Use the remaining fold for validation.
4. Calculate the validation score.
5. Repeat the process until every fold has been used as the validation set.
6. Calculate the mean of all validation scores.

Changing K affects the amount of training and validation data used in each iteration. A larger K generally provides more training data in each iteration but requires more computational time.

---

### 3. Grid Search vs Manual Hyperparameter Selection

Manual hyperparameter selection requires the user to choose parameter values based on experience or experimentation.

Grid Search systematically evaluates all combinations of hyperparameters specified in a parameter grid using cross-validation.

### Advantages of Grid Search

- Systematic parameter evaluation.
- Reduces manual experimentation.
- Can identify useful parameter combinations.
- Works together with cross-validation.

### Limitations of Grid Search

- Can be computationally expensive.
- The number of combinations increases rapidly when more parameters and values are added.
- It only searches values specified by the user.
- It may require considerable processing time for large datasets.