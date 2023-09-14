# Code Summary

This code is a Python script that demonstrates a machine learning workflow using the pandas library for data manipulation, seaborn and matplotlib for data visualization, and scikit-learn for building and evaluating machine learning models. The code appears to be working with a dataset named 'loan_data.csv' and aims to predict whether a loan applicant will not fully pay their loan (binary classification).

## Data Exploration and Visualization

The code begins by importing necessary libraries and loading the dataset using pandas. It then performs the following data exploration and visualization tasks:
- Displays the first few rows of the dataset using `df.head()`.
- Provides dataset information using `df.info()`.
- Creates various plots, including count plots and histograms, to explore relationships and distributions within the data.

## Data Preprocessing

The code conducts some data preprocessing steps:
- One-hot encodes the 'purpose' column using `pd.get_dummies()` to convert categorical data into a numerical format.
- Multiplies the 'int.rate' column by 100 to convert interest rates to percentages.
- Drops the 'purpose' column, as it has been one-hot encoded.

## Model Building

The code proceeds to build and evaluate two classification models:
1. **Decision Tree Classifier**:
   - Imports the DecisionTreeClassifier from scikit-learn.
   - Splits the data into training and testing sets using `train_test_split()`.
   - Fits the DecisionTreeClassifier to the training data.
   - Makes predictions on the testing data and evaluates the model using confusion matrix and classification report.

2. **Random Forest Classifier**:
   - Imports the RandomForestClassifier from scikit-learn.
   - Initializes the classifier with 300 decision trees.
   - Fits the RandomForestClassifier to the training data.
   - Makes predictions on the testing data and evaluates the model using confusion matrix and classification report.

## Model Evaluation

Both models are evaluated using metrics such as confusion matrix, precision, recall, and F1-score. The code also calculates and prints the accuracy of the models on the testing data.

Overall, this code demonstrates a typical machine learning workflow for classification tasks, including data exploration, preprocessing, model building, and evaluation.

