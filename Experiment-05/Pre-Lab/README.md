# Experiment 05: Decision Tree and Ensemble Learning Models

**Name:** R. Karthik  
**Roll No:** 25EU02904

## Pre-Lab Tasks

### 1. What is a Decision Tree? Explain its structure, working principle, and applications in classification and regression.

A Decision Tree is a supervised machine learning algorithm that uses a tree-like structure to make predictions. It can be used for both classification and regression problems.

The main components of a Decision Tree are the root node, internal decision nodes, branches, and leaf nodes. The root node represents the first decision, internal nodes represent feature-based conditions, branches represent the outcomes of those conditions, and leaf nodes contain the final prediction.

The algorithm recursively divides the dataset based on feature values. For classification, measures such as Gini impurity or entropy can be used to select suitable splits. For regression, the algorithm generally selects splits that reduce prediction error or variance.

Decision Trees are used in applications such as medical diagnosis, customer classification, fraud detection, house price prediction, and risk assessment.

---

### 2. What is Ensemble Learning? Explain the working principles of Bagging, Random Forest, and Voting techniques.

Ensemble Learning is a machine learning approach that combines multiple models to produce a stronger and more reliable prediction than a single model.

**Bagging:**  
Bagging, or Bootstrap Aggregating, trains multiple models on different bootstrap samples of the training dataset. Their predictions are then combined. For classification, majority voting is generally used. Bagging helps reduce variance and overfitting.

**Random Forest:**  
Random Forest is an ensemble of Decision Trees. It uses bootstrap samples and randomly selected subsets of features when constructing trees. The predictions of the individual trees are combined to obtain the final prediction. This reduces correlation between trees and improves generalization.

**Voting:**  
Voting combines predictions from different machine learning algorithms. In hard voting, the final class is selected based on the majority of predicted classes. In soft voting, predicted probabilities are combined and the class with the highest combined probability is selected.

---

### 3. What is Boosting? Explain the working principles of AdaBoost and Gradient Boosting, and differentiate Boosting from Bagging.

Boosting is an ensemble learning technique that builds models sequentially. Each new model attempts to improve the errors or weaknesses of the previous models.

**AdaBoost:**  
AdaBoost trains weak learners sequentially and gives greater importance to samples that were incorrectly classified by previous learners. The learners are then combined using weighted voting.

**Gradient Boosting:**  
Gradient Boosting also builds models sequentially. Each new model attempts to reduce the errors of the previous ensemble by fitting a new model to the residual errors or negative gradient of the loss function.

**Difference between Boosting and Bagging:**

- Bagging trains models independently and in parallel.
- Boosting trains models sequentially.
- Bagging mainly focuses on reducing variance.
- Boosting focuses on reducing bias and improving predictive accuracy.
- Random Forest is an example of a bagging-based ensemble.
- AdaBoost and Gradient Boosting are examples of boosting techniques.

---

### 4. Compare Decision Trees, Ensemble Learning, and Boosting techniques based on their working principles.

| Technique | Working Principle | Main Advantage |
|---|---|---|
| Decision Tree | Uses recursive feature-based splitting to form a tree structure | Simple and interpretable |
| Ensemble Learning | Combines multiple models to produce a stronger prediction | Improves stability and generalization |
| Bagging | Trains models independently on bootstrap samples | Reduces variance |
| Random Forest | Combines multiple randomized Decision Trees | Good generalization and robustness |
| Voting | Combines predictions from different models | Uses strengths of multiple algorithms |
| Boosting | Builds weak learners sequentially to correct previous errors | Can achieve high predictive accuracy |
| AdaBoost | Gives more weight to incorrectly classified samples | Improves weak learners |
| Gradient Boosting | Sequentially minimizes loss using gradient-based optimization | Effective for complex prediction problems |

In summary, Decision Trees are individual predictive models, Ensemble Learning combines multiple models, and Boosting builds models sequentially to progressively improve performance.