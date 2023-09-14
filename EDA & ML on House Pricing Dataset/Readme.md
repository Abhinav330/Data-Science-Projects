# Code Summary

This Python script is a simple housing price prediction model using linear regression. It imports necessary libraries, loads the 'USA_Housing.csv' dataset, preprocesses the data, visualizes it, builds a linear regression model, and allows for predicting house prices based on user input.

## Data Loading and Preprocessing

The script starts by importing essential libraries, loading the 'USA_Housing.csv' dataset using pandas, and performing data preprocessing:
- Drops the 'Address' column, which is not required for analysis.
- Rounds the numeric columns to integers.
- Renames some columns for readability.

## Data Visualization

Data visualization is performed with various plots:
- A heatmap is used to check for missing values.
- Histograms and bar plots show the distribution of house prices and relationships between variables like 'House Age' and 'Price'.
- A heatmap of the correlation matrix visualizes feature correlations.
- A joint plot shows a hexbin plot and a kernel density estimate plot of 'Area Population' vs. 'Price'.

## Model Building

The code then proceeds to build a linear regression model:
- Splits the data into feature variables ('x') and the target variable ('y') using `train_test_split`.
- Imports `LinearRegression` from scikit-learn and initializes the model.
- Fits the model to the training data.
- Makes predictions on the testing data.

## Model Evaluation

The script evaluates the linear regression model's accuracy using the R-squared (R2) score:
- Imports `r2_score` from scikit-learn and calculates the R2 score.
- Prints the model's accuracy as a percentage.
- Plots the actual vs. predicted house prices for visual comparison.

## User Interaction

The script allows users to input values for 'Area Income,' 'House Age,' 'No. of rooms,' and 'Area Population' to predict the house price:
- Prompts users for input and creates a DataFrame with the input values.
- Uses the trained model to predict the house price based on user input.
- Displays the predicted price in both thousands of dollars and crores of rupees.
- Asks if the user wants to continue predicting house prices.

## Note

- The script is a basic linear regression model and does not include advanced features or extensive data preprocessing.
- Users can continue predicting house prices as long as they answer 'y' to the prompt.

Ensure that the 'USA_Housing.csv' dataset is correctly loaded, and all necessary imports are available before running the code. Also, consider enhancing the model and preprocessing steps for more accurate predictions.
