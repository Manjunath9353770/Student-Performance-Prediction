# MODEL TRAINING AND EVALUATION

## 1. Introduction

This document explains the machine learning model used in the Student Performance Prediction project.

The project uses Linear Regression to predict students' final academic grades based on selected input features.

## 2. Machine Learning Algorithm

**Algorithm:** Linear Regression

**Learning Type:** Supervised Learning

**Problem Type:** Regression

Linear Regression is a supervised machine learning algorithm that estimates a continuous numerical output using a mathematical relationship between input variables and the target variable.

In this project, the target variable is G3 (final grade).

## 3. Input and Output Variables

**Input (X):**
- Student demographic information.
- Family and social information.
- Educational support information.
- Study time and other academic factors.

**Output (y):**
- G3 – Student's final grade.

The columns G1, G2 and G3 are excluded from the input features in this project. G3 is used as the prediction target.

## 4. Model Training Process

The model training process includes:

1. Import Linear Regression from Scikit-learn.
2. Create a Linear Regression model.
3. Fit the model using training data.
4. Generate predictions using test data.

The model is trained using 316 records and tested using 79 records.

## 5. Python Implementation

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

model.fit(X_train, y_train)

y_pred = model.predict(X_test)
```

## 6. Model Evaluation Metrics

The following regression metrics are used to evaluate the model:

**Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted grades. Lower values are better.

**Mean Squared Error (MSE):** Measures the average squared prediction error. Lower values are better.

**R-squared (R²):** Measures how much of the variation in the target variable is explained by the model. A value closer to 1 generally indicates a better fit.

Actual metric values must be copied from the notebook's evaluation output.

## 7. Model Saving

The trained model is saved using Python's Pickle library.

Model file:

`Source_Code/student_model.pkl`

The feature column information is saved separately:

`Source_Code/feature_columns.pkl`

These files allow the saved model and its expected input-column structure to be reused.

## 8. Conclusion

Linear Regression is used in this project to estimate students' final academic grades from available student information.

The model is trained, tested and evaluated using a supervised learning workflow.

This project demonstrates the practical application of Python and machine learning in educational data analysis.