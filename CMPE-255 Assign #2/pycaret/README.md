# Data Science Tasks Repository

This repository contains code and data for various data science tasks as part of an assignment. Here's an overview of what was done for each task:

## Tasks

### Classification 
**Binary Classification - Level:**
- Used the PyCaret library to predict binary outcomes on a dataset.
- Cleaned the data, handled missing values, and prepared it for modeling.
- Split the data into training and testing sets.
- Trained multiple models to predict binary targets.

**Multiclass Classification - Level:**
- Expanded the binary classification task to work with multiple classes.
- Employed PyCaret for data prep and model training.
- Predicted a target variable with several classes.
- Evaluated model performance using different metrics.

### Regression
- Used PyCaret for regression analysis on a dataset.
- Handled data preprocessing tasks such as dealing with missing data and encoding categorical features.
- Split the data into training and testing sets.
- Trained and evaluated regression models to predict continuous target values.

### Clustering
- Explored clustering techniques using PyCaret.
- Grouped data into clusters using clustering algorithms.
- Visualized clusters and analyzed their properties.

### Anomaly Detection
- Explored anomaly detection using PyCaret.
- Focused on identifying unusual data points (anomalies) within the dataset based on various features.

## Corresponding Targets or Objectives

### Classification
**Binary Classification - Level:**
- Predicted 'GDP_Class' - Binary classification based on GDP classification.

**Multiclass Classification - Level:**
- Predicted 'GDP_Category' - Multiclass classification based on GDP category with multiple classes.

### Regression
- Predicted 'GDP (current US$)' - Regression based on the continuous GDP values.

### Clustering
- The clustering task was feature-based, and no specific target variable was used.

### Anomaly Detection
- The goal was to identify anomalies or outliers in the dataset based on various features.

## Association Rule Mining with Python

Discover patterns in your transactional data using Python and mlxtend.

- **Generate Data:** Create a dataset with transaction records.
- **Data Preprocessing:** Load data into a Pandas DataFrame.
- **Association Rule Mining:** Utilize the Apriori algorithm.
- **Rule Filtering:** Apply filters (support, confidence, lift).
- **Results:** Extract valuable insights from the rules.

Find detailed code in the associated notebook or script. Feel free to adapt for your own projects!

## Time Series Forecasting with pycaret on Temperature Dataset

### Dataset:
- The dataset contains yearly temperature anomalies sourced from 'GCAG'. Each record is represented by a year and its corresponding mean temperature anomaly.

### Objective:
- Forecast future temperature anomalies using historical data.

### Steps:
1. **Data Preparation:**
    - Load the dataset.
    - Convert the 'Year' column to a datetime format.
    - Set the 'Year' as the DataFrame index.
    - Filter the dataset to only include records from the 'GCAG' source.
2. **Initialize Time Series Environment in pycaret:** 
    - Initialize the time series environment using the setup function in pycaret.time_series.
    - Provide the dataset and specify the target column as 'Mean'. 
    - Choose a fold strategy like 'rolling' and set a session ID.
3. **Train and Compare Models:** 
    - Use the compare_models function to automatically train and evaluate multiple models. 
    - The best model will be selected based on performance metrics like MAE.
4. **Forecast:** 
    - Once the best model is selected, use it to forecast future temperature anomalies.

## Colab Notebooks

- [Anomaly detection](https://colab.research.google.com/drive/1k0rWaXlISyMuimhnsQOUksAT4aodf0Wn?usp=sharing)
- [Classification: Binary classification, Multiclass, Regression](https://colab.research.google.com/drive/1k0rWaXlISyMuimhnsQOUksAT4aodf0Wn?usp=sharing)
- [Clustering](https://colab.research.google.com/drive/1h5wunFhz_MyOtq7gibwJUfY_1vcaJ5hc?usp=sharing)
