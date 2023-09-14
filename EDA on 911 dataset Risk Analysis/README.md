# Exploratory Data Analysis on 911 Dataset
Source : [Kaggle](https://www.kaggle.com/datasets/mchirico/montcoalert?select=911.csv)

# Code Summary

This Python script analyzes emergency call data from the '911.csv' dataset. It uses various data visualization techniques to explore and gain insights into the emergency call data, including the types of calls, reasons for calls, and call patterns over time.

## Data Loading and Exploration

The script starts by importing necessary libraries, including NumPy, Pandas, Matplotlib, Seaborn, and Plotly. It loads the '911.csv' dataset and explores its contents. Key steps in this section include:
- Checking the dataset information with `df.info()`.
- Creating a new column 'call_type' by extracting the call type from the 'title' column.
- Visualizing the distribution of call types using a bar plot.

## Call Types and Reasons

The script further analyzes the reasons for calls by:
- Extracting the actual reasons from the 'title' column and creating a new column 'Actual_reason'.
- Visualizing the most common reasons for calls using a bar plot.
- Converting the 'timeStamp' column to a datetime format.
- Extracting additional date and time-related columns, such as 'day,' 'month,' 'year,' and 'hour.'

## Temporal Analysis

The script performs temporal analysis of calls, including:
- Counting and visualizing call types by month using a count plot.
- Counting and visualizing call types by year using a count plot.
- Counting and visualizing call types by hour using a count plot.

## Location Analysis

The script explores the locations of calls by:
- Displaying the top 20 townships ('twp') with the highest call counts.
- Displaying the last 5 townships with the lowest call counts.
- Visualizing the top 100 townships with the highest call counts using a bar plot.
- Visualizing the last 10 townships with the lowest call counts using a bar plot.
- Exploring call locations by analyzing the 'addr' and 'twp' columns.

## Data Transformation

The script maps call types to numeric values by defining a function and applying it to the 'call_type' column. It then drops the unnecessary 'e' column.

## Correlation Analysis

The script calculates and visualizes the correlation between numeric columns in the dataset using a heatmap. This helps identify potential relationships between variables.
