# Boston Housing Price Prediction using Machine Learning

## Overview

This project aims to predict housing prices in Boston using various Machine Learning regression algorithms. The dataset contains information about different towns and suburbs in Boston, with 13 features describing housing and neighborhood characteristics and a target variable representing the median house price.

The objective is to build predictive models and compare their performance using standard regression evaluation metrics.

---

## Problem Statement

Accurate house price prediction is an important task in the real estate industry. The goal of this project is to develop a machine learning model that can estimate the price of a house based on various socio-economic and geographical factors.

Given a set of housing features, the model predicts the median value of owner-occupied homes in Boston.

---

## Dataset Information

**Dataset:** Boston Housing Dataset

* Total Records: 506
* Features: 13
* Target Variable: PRICE

### Features Description

| Feature | Description                                                         |
| ------- | ------------------------------------------------------------------- |
| CRIM    | Per capita crime rate by town                                       |
| ZN      | Proportion of residential land zoned for large lots                 |
| INDUS   | Proportion of non-retail business acres per town                    |
| CHAS    | Charles River dummy variable (1 if tract bounds river, 0 otherwise) |
| NOX     | Nitric oxide concentration                                          |
| RM      | Average number of rooms per dwelling                                |
| AGE     | Proportion of owner-occupied units built before 1940                |
| DIS     | Weighted distance to employment centers                             |
| RAD     | Accessibility to radial highways                                    |
| TAX     | Property tax rate                                                   |
| PTRATIO | Pupil-teacher ratio                                                 |
| B       | Proportion of Black population                                      |
| LSTAT   | Percentage of lower-status population                               |
| PRICE   | Median value of owner-occupied homes (Target)                       |

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost

---

## Project Workflow

### 1. Data Collection

Loaded the Boston Housing dataset and converted it into a Pandas DataFrame.

### 2. Data Exploration

Performed exploratory data analysis (EDA) to understand:

* Dataset shape
* Data types
* Missing values
* Statistical summaries
* Correlations among features

### 3. Data Visualization

Generated:

* Correlation Heatmap
* Feature Distribution Plots
* Scatter Plots
* Actual vs Predicted Price Graphs

### 4. Data Preprocessing

* Checked for missing values
* Verified data consistency
* Prepared feature matrix (X) and target variable (y)

### 5. Model Building

The following regression models were trained:

1. Linear Regression
2. Random Forest Regressor
3. XGBoost Regressor
4. Support Vector Regressor (SVR)

### 6. Model Evaluation

Models were evaluated using:

* R² Score
* Adjusted R² Score
* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)

---

## Results

### Linear Regression

| Metric      | Value  |
| ----------- | ------ |
| R² Score    | 71.22% |
| Adjusted R² | 68.51% |
| MAE         | 3.86   |
| MSE         | 30.05  |
| RMSE        | 5.48   |

### Random Forest Regressor

| Metric      | Value  |
| ----------- | ------ |
| R² Score    | 86.41% |
| Adjusted R² | 85.13% |
| MAE         | 2.57   |
| MSE         | 14.19  |
| RMSE        | 3.77   |

### XGBoost Regressor

| Metric      | Value  |
| ----------- | ------ |
| R² Score    | 84.95% |
| Adjusted R² | 83.53% |
| MAE         | 2.45   |
| MSE         | 15.72  |
| RMSE        | 3.96   |

### Support Vector Regressor (SVR)

| Metric      | Value  |
| ----------- | ------ |
| R² Score    | 59.00% |
| Adjusted R² | 55.14% |
| MAE         | 3.76   |
| MSE         | 42.81  |
| RMSE        | 6.54   |

---

## Model Comparison

| Model                    | R² Score (%) |
| ------------------------ | ------------ |
| Random Forest            | 86.41        |
| XGBoost                  | 84.95        |
| Linear Regression        | 71.22        |
| Support Vector Regressor | 59.00        |

---

## Best Performing Model

Based on the evaluation metrics, **Random Forest Regressor** achieved the highest R² Score of **86.41%** and the lowest prediction error among all tested models.

Therefore, Random Forest was selected as the best-performing model for Boston house price prediction.

---

## Conclusion

This project successfully implemented and compared multiple machine learning regression algorithms for predicting Boston housing prices.

The results demonstrate that ensemble-based models such as Random Forest and XGBoost outperform traditional Linear Regression and Support Vector Regression for this dataset.

Random Forest Regressor provided the most accurate predictions and can be effectively used for housing price estimation tasks.

---

## Future Improvements

* Hyperparameter tuning using GridSearchCV
* Feature selection and dimensionality reduction
* Cross-validation for more robust evaluation
* Deployment using Flask or Streamlit
* Testing on larger and more recent housing datasets

---

