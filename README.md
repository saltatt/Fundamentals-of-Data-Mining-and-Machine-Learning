# Linear Regression Seminar & Homework

## Analytical Solution, Model Training, Validation, and Web Service Deployment

This repository contains materials from the seminar **“Linear Regression: Analytical Solution, Model Training, and Validation”** as well as **Homework #1**, which focuses on building and deploying a regression model.

---

## 📌 Seminar: Linear Regression — Training and Validation

### **1. Deriving the Analytical Formula for Weights**

In the seminar, we consider the problem of minimizing the loss function for linear regression:

$$
Q(w) = (Xw - y)^T (Xw - y)
$$

The task is to find the analytical solution for the optimal weights ( w ).
This is a classical least-squares optimization problem, where the solution is given by the **normal equation**:

$$
w = (X^T X)^{-1} X^T y
$$

The seminar explains each step of this derivation, properties of the solution, and when the analytical method is appropriate.

---

## 🧩 Homework #1

In this assignment, you will:

### **1. Train a Regression Model**

Build and train a model to predict **car prices** based on the provided dataset.
You may use scikit-learn, NumPy, Pandas, or implement your own model — depending on the task requirements.

### **2. Develop a Web Service**

You must implement a simple web API (e.g., using **FastAPI** or **Flask**) that applies the trained model to new incoming data.
The service should:

* accept input features,
* preprocess them,
* apply the trained regression model,
* return the predicted price.

### **Grading**

Your final score for the homework is calculated as:

$$
\text{Score} = \min(\text{your result},\ 10)
$$

---

## 📊 Confusion Matrix (Extra Topic)

Although confusion matrices are typically used for classification tasks (not regression), this repository may include materials explaining:

* What a **Confusion Matrix** is
* How it is constructed
* How to interpret TP, FP, TN, FN
* Connections to metrics such as accuracy, precision, recall, F1-score

This section can be helpful for future assignments involving classification problems.

---
📌 Logistic Regression Project (Ad Click Prediction)

Logistic Regression is widely used to estimate the probability that an object belongs to a specific class.
If the predicted probability is greater than 50%, the model classifies the object as 1; otherwise — as 0.
Thus, logistic regression is a binary classifier.

In this notebook, we discuss the theory behind Logistic Regression and apply it to a practical task:
predicting whether a user will click on an online advertisement.

The goal of the project is to build a model that can determine whether a user will click on an ad based on several user-related features.

Dataset Features

The dataset includes the following variables (features):

user demographics

browsing behavior

activity history

device and platform information

advertisement context

and other factors that may influence the probability of clicking

These features are used to train a logistic regression model, evaluate its performance, and analyze which variables most strongly affect user behavior.
