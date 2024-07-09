# Logistic Regression with Churn Prediction

This project aims to learn logistic regression and apply it to a churn prediction dataset. The dataset contains various features related to customer churn, and the goal is to build a model that can accurately predict whether a customer will churn or not.

## Table of Contents
- [Logistic Regression with Churn Prediction](#logistic-regression-with-churn-prediction)
  - [Table of Contents](#table-of-contents)
  - [Project Overview](#project-overview)
  - [Data Preprocessing and Selection](#data-preprocessing-and-selection)
  - [Model Training](#model-training)
  - [Evaluation](#evaluation)
  - [Different Solvers](#different-solvers)

## Project Overview

In this project, we will follow these steps:
1. Import necessary libraries and load the dataset.
2. Perform data preprocessing and select relevant features.
3. Split the dataset into training and testing sets.
4. Train a logistic regression model using different solvers.
5. Evaluate the model's performance using metrics like confusion matrix, classification report, and log loss.
6. Experiment with different solver parameters to optimize the model's performance.

## Data Preprocessing and Selection

The dataset used in this project is named `churnData.csv`. We will import the dataset and perform the following preprocessing steps:
1. **Select relevant features:** We will only keep the columns that are relevant to our analysis, such as 'tenure', 'age', 'address', 'income', 'ed', 'employ', 'equip', 'callcard', 'wireless', and 'churn'.
2. **Convert the 'churn' column to integer values.**
3. **Display the first few rows of the preprocessed dataset to verify the changes.**

## Model Training

We will use the preprocessed dataset to train a logistic regression model using different solvers. The solvers we will experiment with are 'liblinear', 'newton-cg', and 'sag'. We will follow these steps:
1. **Split the dataset into training and testing sets.**
2. **Train the logistic regression model using the training set and the specified solver.**
3. **Display the trained model.**

## Evaluation

We will evaluate the performance of the trained model using metrics like confusion matrix, classification report, and log loss. The steps to evaluate the model are as follows:
1. **Predict the outcomes using the test set.**
2. **Calculate the confusion matrix to analyze the model's performance in terms of true positives, true negatives, false positives, and false negatives.**
3. **Generate a classification report to provide precision, recall, and F1-score for each class.**
4. **Calculate the log loss to measure the discrepancy between the predicted probabilities and the actual outcomes.**
5. **Display the confusion matrix, classification report, and log loss.**

## Different Solvers

We will experiment with different solvers to optimize the model's performance. The solvers we will compare are 'liblinear', 'newton-cg', and 'sag'. The key differences between these solvers are as follows:
1. **'liblinear':** Suitable for small datasets and less computationally expensive. It uses a one-vs-rest approach for multiclass classification.
2. **'newton-cg':** A more complex and computationally expensive solver that uses the Newton-CG method for optimization. It is suitable for large datasets and can handle multiclass classification.
3. **'sag':** An improved version of the stochastic average gradient (SAG) method, suitable for large datasets and capable of handling multiclass classification. It is more efficient than the 'newton-cg' solver.

By comparing the log loss values obtained using different solvers, we can determine which solver provides the best performance for our specific dataset and problem.

Please note that this README.md file provides a high-level overview of the project. For more detailed information, you can refer to the code comments and documentation provided in the Python script.
