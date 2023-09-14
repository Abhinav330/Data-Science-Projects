# Code Summary

This Python script demonstrates the classification of Iris flowers into different species (Setosa, Versicolor, Virginica) using a Support Vector Machine (SVM) classifier. It imports necessary libraries, loads the Iris dataset, explores the data, and trains an SVM model. The code also performs model tuning using GridSearchCV and evaluates the model's performance.

## Iris Flower Species

The code begins by displaying images of the three Iris flower species:
- Iris Setosa
- Iris Versicolor
- Iris Virginica

## Data Preparation

The script imports essential libraries, loads the 'Iris.csv' dataset using pandas, and performs data preprocessing:
- Drops the 'Id' column, which is not required for analysis.

## Data Exploration and Visualization

The code explores and visualizes the data:
- Creates pair plots to visualize pairwise relationships between features, color-coded by species.
- Displays the column names.

## Data Splitting

The dataset is split into training and testing sets using `train_test_split`. The feature variables are stored in 'x_train' and 'x_test', while the target variable ('Species') is stored in 'y_train' and 'y_test'.

## Support Vector Machine (SVM) Modeling

The script uses an SVM classifier to train and predict Iris flower species:
- Imports `SVC` (Support Vector Classifier) from scikit-learn.
- Initializes and fits an SVM model to the training data.
- Makes predictions on the testing data.

## Model Evaluation

The code evaluates the SVM model's performance by:
- Importing `classification_report`, `confusion_matrix`, and `accuracy_score` from scikit-learn.
- Printing the confusion matrix to assess true positive, true negative, false positive, and false negative predictions.
- Printing the classification report, which includes metrics such as precision, recall, and F1-score.

## Hyperparameter Tuning with GridSearchCV

The code performs hyperparameter tuning using GridSearchCV to optimize the SVM model:
- Defines a parameter grid with different values of 'C' and 'gamma'.
- Initializes GridSearchCV with an SVM classifier, the parameter grid, and other parameters.
- Fits the model to the training data and finds the best parameters using cross-validation.

## GridSearchCV Model Evaluation

The tuned model is evaluated using the same metrics as before:
- Confusion matrix and classification report are printed for the tuned model.

