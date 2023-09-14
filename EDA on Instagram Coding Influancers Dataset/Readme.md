# Instagram Profiles Data Analysis

## Introduction
This Python script focuses on preprocessing and visualizing data from an Instagram profiles dataset. It includes data loading, inspection, visualization, and some data preprocessing steps.

## Data Loading and Basic Inspection
- The script loads a dataset from a CSV file named 'Instagram Profiles - Github Hashtag - instagram_profile.csv' into a Pandas DataFrame named `df`.
- It displays the first few rows and provides information about the dataset using `df.head()` and `df.info()`.

## Data Visualization Class
- The script defines a Python class named `visual_preprocess` to encapsulate data visualization and preprocessing functions.

## Data Exploration and Preprocessing
- The class contains various methods for exploring and preprocessing the data:
  - `_row_col`: Helper function to calculate the number of rows and columns in the DataFrame.
  - `disp_tot_row_col`: Displays the total row and column count.
  - `missingv`: Visualizes missing values using a heatmap.
  - `_null_calculator`: Helper function to calculate the percentage of null values in columns.
  - `null_percentage`: Calculates and displays columns with a specified percentage of null values.
  - `get_col_empty`: Returns columns with null values above a specified threshold.

## Data Cleaning
- Columns with a high percentage of null values (above 50%) are dropped from the DataFrame.

## Data Visualization
- Various data visualizations are created using Seaborn and Matplotlib, including:
  - Distribution of 'posts_count' using a histogram.
  - Filtering and exploration of records with 'posts_count' greater than 2000.
  - Scatterplots of various features ('followers', 'following', 'highlights_count', etc.) with respect to different account types and privacy settings.
  - Bar plots showing relationships between 'is_business_account' and 'is_professional_account' with 'followers' and 'following'.
  - Additional scatterplots exploring features related to 'following' and 'followers'.

## Hashtag Analysis
- The script defines a function (`hashtag_freq`) to extract and analyze hashtags from the 'post_hashtags' column.
- The function counts the frequency of hashtags and displays the top 10 most frequently used hashtags in the dataset.
