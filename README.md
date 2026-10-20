# Advertising Data Analysis

## Project Overview
This project explores user behavior and advertising engagement using Python. It combines Exploratory Data Analysis (EDA) with a Logistic Regression classification model to predict whether a user clicks on an advertisement.

## Objectives
- Explore user demographics, income, internet usage, and time spent on a website.
- Analyze patterns and relationships in the advertising dataset.
- Visualize distributions, user activity, and correlations.
- Build and evaluate a Logistic Regression model to predict ad clicks.

## Dataset
The dataset contains **1,000 records and 10 columns**, including:

- `Daily Time Spent on Site`
- `Age`
- `Area Income`
- `Daily Internet Usage`
- `Ad Topic Line`
- `City`
- `Male`
- `Country`
- `Timestamp`
- `Clicked on Ad` — target variable

The dataset had no missing values according to the initial missing-value check.

## Tools & Technologies
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Inspection and Preparation
- Loaded the dataset using Pandas.
- Examined data types and descriptive statistics.
- Checked for missing values.
- Converted the `Timestamp` column to datetime format.
- Extracted month, year, day, and hour features from the timestamp.

### 2. Exploratory Data Analysis
Created visualizations to explore:
- Age distribution using a histogram.
- Relationship between age and area income using a joint plot.
- Relationship between age and time spent on the website using a KDE joint plot.
- User activity by hour using a count plot.
- Correlations among numerical variables using a heatmap.

### 3. Model Development
- Selected numerical user-behavior and demographic features for prediction.
- Standardized the selected features using `StandardScaler`.
- Split the data into training and testing sets, with 70% for training and 30% for testing.
- Trained a Logistic Regression classification model.

### 4. Model Evaluation
Evaluated the model using accuracy, a confusion matrix, and a classification report.

**Test accuracy: 97%**

| Metric | Class 0 | Class 1 |
|---|---:|---:|
| Precision | 0.96 | 0.98 |
| Recall | 0.98 | 0.96 |
| F1-score | 0.97 | 0.97 |

The model correctly classified 291 out of 300 test records.

## Key Takeaway
This project demonstrates an end-to-end introductory machine learning workflow, from data inspection and visualization to feature standardization, classification, and model evaluation.

## Repository Contents
- `Advertising Data Project.ipynb` — notebook containing the analysis, visualizations, and Logistic Regression model.
- `advertising.csv` — dataset used in the analysis.
