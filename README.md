# Credit Risk Classification
## Module 20 Challenge
### By Eduardo Almonte

## Overview of the Analysis

The purpose of this analysis is to create a machine learning model that can predict the creditworthiness of borrowers based on historical lending data from a peer-to-peer lending company. By identifying whether a loan is likely to be "healthy" or "high-risk," the model will assist lenders in making more informed decisions, potentially reducing defaults and financial loss.

The dataset contains financial information about the borrowers, including factors such as loan size, income, and debt-to-income ratio. The target variable we aim to predict is loan_status, which takes the following values:

0: Indicates a "healthy" loan, meaning it has a low risk of default.
1: Indicates a "high-risk" loan, meaning it has a higher likelihood of default.

The analysis followed a structured machine learning process, which included the following stages:

## Data Preparation:

The dataset was loaded into a Pandas DataFrame.
The target variable (loan_status) was separated into the labels (y), and the remaining columns were used as features (X).
We split the dataset into training and testing sets using the train_test_split function to ensure that we train the model on one portion of the data and test it on unseen data.


## Model Training:

A Logistic Regression model was chosen as the initial classification algorithm. Logistic regression is a popular algorithm for binary classification tasks due to its simplicity, ease of implementation, and interpretability.
The model was trained using the training data (X_train and y_train).

## Prediction and Evaluation:

The trained logistic regression model was used to make predictions on the testing data (X_test).
The performance of the model was evaluated using a confusion matrix and a classification report. The classification report provided key metrics such as accuracy, precision, recall, and F1 score, which were used to measure the model’s ability to classify both healthy and high-risk loans effectively.

## Results Interpretation:

After generating predictions and evaluating the model, the focus was on interpreting how well the logistic regression model performed in distinguishing between healthy and high-risk loans. This involved examining metrics such as accuracy (the overall correctness of the model), precision (how many predicted positive cases were actually positive), and recall (how well the model identified all positive cases).

By following these steps, we aimed to create a reliable and interpretable model that can help the lending company make better decisions regarding loan approvals.

## Summary

I recommend using this model for predicting loan outcomes, as it has demonstrated strong performance in accurately classifying loan risks.



![matrix](https://github.com/almonte951/Credit_Risk_Classification/blob/main/Images/condusion%20matrix%20df.png)

![report](https://github.com/almonte951/Credit_Risk_Classification/blob/main/Images/Classification%20Report.png)

The logistic regression model performs exceptionally well in predicting both healthy and high-risk loans. It correctly identified 18,655 healthy loans, with only 36 incorrectly classified as healthy. The model achieved a 100% precision in predicting healthy loans, while the precision for high-risk loans was 84%. Overall, the logistic regression model proves to be highly effective in classifying loan types.
