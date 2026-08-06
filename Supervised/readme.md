# Linear Regression from Scratch (OLS)

## 📌 Overview

This project implements **Simple Linear Regression from scratch** using the **Ordinary Least Squares (OLS)** method without using libraries like `scikit-learn`.

The purpose of this implementation is to understand the mathematical foundation behind Linear Regression and how the model calculates the best-fit line for prediction.

---

## 📖 Linear Regression

Linear Regression is a supervised machine learning algorithm used for predicting continuous values.

The relationship between input feature and target variable is represented as:

$$
y = mx + b
$$

Where:

- `m` = slope (coefficient)
- `b` = intercept
- `x` = input feature
- `y` = predicted output

---

## 📐 Ordinary Least Squares (OLS)

OLS finds the best-fitting line by minimizing the difference between actual values and predicted values.

The goal is to minimize:

$$
\sum (y_i - \hat{y_i})^2
$$

### Slope Formula

$$
m = \frac{\sum(x_i-\bar{x})(y_i-\bar{y})}
{\sum(x_i-\bar{x})^2}
$$

### Intercept Formula

$$
b = \bar{y} - m\bar{x}
$$

---

## 🚀 Features

- Implemented Linear Regression without `scikit-learn`
- Implemented OLS mathematical equations manually
- Calculates:
  - Mean of input values
  - Mean of target values
  - Slope
  - Intercept
- Predicts new values using the learned parameters
- Simple and beginner-friendly implementation

---

## 🛠 Technologies Used

- Python
- NumPy

---

## ⚙️ How It Works

1. Initialize the Linear Regression model

2. Fit the model using training data:

```
model.fit(X_train, y_train)
```

3. During training:
   - Calculate mean values
   - Calculate slope (`m`)
   - Calculate intercept (`b`)

4. Generate predictions:

```
model.predict(X_test)
```

5. The prediction equation becomes:

$$
\hat{y} = mx + b
$$

---

## 📊 Example

```python
from LinearRegression import LinearRegression

model = LinearRegression()

model.fit(X_train, y_train)

prediction = model.predict(X_test)
```

---

## 🧠 Concepts Learned

This project covers:

- Supervised Learning
- Regression Algorithms
- Ordinary Least Squares
- Mathematical Derivation of Linear Regression
- Slope and Intercept Calculation
- Model Training and Prediction

---

## 🔮 Future Improvements

- Multiple Linear Regression
- Gradient Descent implementation
- Add evaluation metrics:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score

---

## 🎯 Motivation

This project is part of my Machine Learning journey where I implement algorithms from scratch to understand their mathematical intuition before using high-level ML libraries.

---

## 👨‍💻 Author

**Najaf Ali**

BS Artificial Intelligence

Learning and implementing Machine Learning algorithms from scratch.
