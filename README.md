# 📉 Ridge and Lasso Regression

**Ridge** and **Lasso Regression** are advanced linear modeling techniques that apply **regularization** to prevent overfitting. These methods modify the loss function to penalize large coefficients, thus helping the model generalize better to unseen data.

---

## ⚙️ What is Regularization?

Regularization is a technique used in machine learning to:
- Prevent overfitting by controlling model complexity
- Encourage simpler models that generalize well
- Handle multicollinearity (correlated input features)
- Reduce variance in high-dimensional datasets

It works by adding a penalty term to the cost (loss) function of the model. This penalty increases with the magnitude of the model coefficients.

---

## 🧮 Ridge Regression (L2 Regularization)

Ridge regression adds an **L2 penalty** (the square of the magnitude of coefficients) to the ordinary least squares cost function:

```math
\text{Loss} = \sum (y_i - \hat{y}_i)^2 + \lambda \sum w_j^2
