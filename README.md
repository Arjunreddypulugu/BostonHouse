# Data Source
https://data.boston.gov/dataset/property-assessment

# Property Assessment Analysis

Welcome to the Property Assessment Analysis repository! This project aims to analyze property assessment data spanning fiscal years 2013 to 2017, providing insights and predictive models to assist stakeholders in the real estate industry. Below is a detailed guide to understanding and utilizing the contents of this repository.

## Overview

The primary objective of this project is to analyze property assessment data and derive actionable insights to assist various stakeholders, including real estate professionals, investors, and policymakers. By leveraging data preprocessing, exploratory data analysis (EDA), feature engineering, and predictive modeling techniques, we aim to extract valuable information from the dataset.

## Dataset

The dataset consists of property assessment records from fiscal years 2013 to 2017. Each record contains a variety of attributes such as property location, size, age, features, and assessed values. This rich dataset serves as the foundation for our analysis, enabling us to explore the factors influencing property values and ownership.

### Data Size

- Number of records: 302,101
- Number of attributes: 18

## Analysis Steps

1. **Data Preprocessing**: We start by loading the raw data into Pandas DataFrames and performing initial data cleaning tasks such as handling missing values and selecting relevant columns for analysis.

2. **Exploratory Data Analysis (EDA)**: Through visualizations such as histograms, boxplots, and scatter plots, we explore the distributions, relationships, and trends within the data. This step helps us gain insights into the characteristics of the dataset and identify potential patterns.

3. **Feature Engineering**: We engineer new features such as property age and time since last remodel to enrich the dataset and capture additional information relevant to property values. Polynomial features are also generated to capture non-linear relationships.

4. **Model Building**: Using machine learning models such as linear regression and Lasso regression, we build predictive models to estimate property values. We evaluate model performance using metrics like RMSE (Root Mean Squared Error) and R-squared to assess predictive accuracy.

5. **Logistic Regression for Ownership Prediction**: Employing logistic regression, we predict property ownership status based on other property attributes. We evaluate the logistic regression model using metrics such as accuracy, precision, recall, and F1 score.

6. **Receiver Operator Curve (ROC)**: We plot a ROC curve to visualize the logistic regression model's performance in predicting property ownership, providing insights into its classification capabilities.

## Model Metrics

### Linear Regression Model

- RMSE (Root Mean Squared Error) on training data: 104,876.17
- RMSE on test data: 105,103.12
- R-squared (R2) on test data: 0.42

### Lasso Regression Model

- R-squared (R2) on test data: 0.42

### Polynomial Regression Model (Degree=2)

- RMSE on training data: 78,206.51
- RMSE on test data: 77,984.99
- R-squared (R2) on test data: 0.68

### Polynomial Regression Model (Degree=3)

- RMSE on training data: 69,439.88
- RMSE on test data: 101,742.22
- R-squared (R2) on test data: 0.46

### Logistic Regression Model for Ownership Prediction

- Accuracy: 72.75%
- Precision: 75.20%
- Recall: 90.40%
- F1 Score: 82.17%

## Conclusion

This analysis provides valuable insights into property assessment data, including factors influencing property values and ownership status. By leveraging advanced analytics techniques, we empower stakeholders in the real estate industry to make data-driven decisions and optimize their strategies.

## Dependencies

To run the analysis code in notebook, you will need the following Python libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
