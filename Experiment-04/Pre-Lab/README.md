# Experiment 04: Regression Modeling and Training Strategies

**Name:** Karthik

## Pre-Lab Tasks

### 1. What is regression in machine learning? Explain the working principle of Linear Regression and its applications in predicting continuous values.

Regression is a supervised machine learning technique used to predict continuous numerical values from one or more input features.

Linear Regression assumes a linear relationship between the input variables and the target variable. It represents this relationship using an equation such as:

y = β₀ + β₁x₁ + β₂x₂ + ... + βₙxₙ

where y is the predicted value, β₀ is the intercept, β₁...βₙ are model coefficients, and x₁...xₙ are input features.

The model determines the coefficients that minimize the difference between actual and predicted values, commonly using the Residual Sum of Squares.

Applications include house price prediction, sales forecasting, demand prediction, financial analysis, and temperature prediction.

---

### 2. What is the difference between Linear Regression, Support Vector Regression (SVR), and Decision Tree Regression?

**Linear Regression** assumes a linear relationship between input features and the target. It is simple, computationally efficient, and suitable when the relationship is approximately linear.

**Support Vector Regression (SVR)** is based on Support Vector Machine principles. It attempts to find a regression function within an epsilon-insensitive error margin. SVR can model nonlinear relationships using kernels such as the RBF kernel.

**Decision Tree Regression** uses a tree structure to divide the data into smaller regions based on feature values. Each leaf node produces a continuous prediction, usually based on the average target value of the samples in that leaf.

Therefore, Linear Regression is primarily linear, SVR can model complex relationships using kernels, and Decision Tree Regression uses recursive feature-based splitting.

---

### 3. What are the common evaluation metrics used for regression models?

Common regression evaluation metrics include:

**Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted values. Lower MAE indicates better performance.

**Mean Squared Error (MSE):** Measures the average squared difference between actual and predicted values. It gives greater importance to large errors.

**Root Mean Squared Error (RMSE):** The square root of MSE. It is expressed in the same units as the target variable.

**R² Score:** Measures how well the model explains the variation in the target variable. A value closer to 1 generally indicates better model performance.

These metrics help compare regression models and determine how accurately they predict continuous values.