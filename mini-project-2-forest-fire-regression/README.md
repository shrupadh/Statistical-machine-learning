Forest Fire Regression Analysis using Multiple Linear Regression
# Mini Project 2: Forest Fire Regression Analysis

## Overview

This project applies exploratory data analysis (EDA) and multiple linear regression to the UCI Forest Fires dataset. The objective was to identify factors associated with forest fire burned area, evaluate regression assumptions, improve the regression model, and predict burned area using the final model.

---

## Dataset

- **Dataset:** UCI Forest Fires Dataset
- **Observations:** 515
- **Response Variable:** `log_area` (log-transformed burned area)

---

## Objectives

- Explore the dataset using summary statistics and visualizations.
- Build simple and multiple linear regression models.
- Identify statistically significant predictors.
- Evaluate linear regression assumptions.
- Detect influential observations using Cook's Distance.
- Improve the regression model by removing influential observations.
- Predict burned area using the final regression model.

---

## Methods

- Exploratory Data Analysis (EDA)
- Data Visualization
- Log Transformation of Burned Area
- Simple Linear Regression
- Multiple Linear Regression
- Model Selection
- Regression Diagnostics
- Cook's Distance
- Residual Analysis
- Q-Q Plot
- Prediction

---

## Project Summary

### (a) Simple Linear Regression
- Built separate simple linear regression models for each quantitative predictor.
- Evaluated regression coefficients, p-values, and R² values.
- No individual predictor showed a strong linear relationship with the response variable.

### (b) Multiple Linear Regression
- Built a multiple linear regression model using quantitative and categorical predictors.
- Evaluated regression coefficients, t-tests, and overall model significance.
- Selected significant predictors through model refinement.

### (c) Exploratory Data Analysis
- Examined variable distributions.
- Visualized relationships between predictors and burned area.
- Generated summary statistics to understand the dataset.

### (d) Response Transformation
- Applied a log transformation:

  `log(area + 1)`

- Reduced skewness in the response variable and improved model assumptions.

### (e) Model Diagnostics
Evaluated regression assumptions using:
- Residual vs Fitted Plot
- Histogram of Residuals
- Normal Q-Q Plot
- Cook's Distance

These diagnostics were used to assess:
- Linearity
- Normality of residuals
- Homoscedasticity
- Influential observations

### (f) Final Regression Model
- Constructed the final multiple linear regression model using quantitative predictors and categorical variables (month and day).
- Represented categorical variables using dummy encoding.

### (g) Prediction
- Predicted burned area using:
  - Sample mean values for quantitative predictors.
  - Most frequent categories (Month = August, Day = Sunday).

**Predicted log(area + 1):** **0.9883**

**Predicted Burned Area:** **1.69 hectares**

### (h) Outlier Analysis
- Identified influential observations using Cook's Distance.
- Removed 27 influential observations.
- Refit the regression model and compared performance.
- The updated model showed:
  - Higher R² and Adjusted R²
  - Lower AIC and BIC
  - Improved overall model significance

The refined model was selected as the final model.

---

## Python Libraries

- pandas
- NumPy
- matplotlib
- seaborn
- scipy
- statsmodels

---

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data Cleaning and Transformation
- Simple & Multiple Linear Regression
- Feature Selection
- Statistical Hypothesis Testing
- Regression Diagnostics
- Outlier Detection (Cook's Distance)
- Model Evaluation
- Predictive Modeling
- Python for Data Science

---

## Files

- **Forest_Fires_EDA_and_Regression.ipynb** – Jupyter Notebook containing the complete analysis, modeling, diagnostics, and prediction.
- **Forest_Fires_EDA_and_Regression.html** *(or PDF, if applicable)* – Exported notebook for easy viewing.
- **forestfires.csv** – UCI Forest Fires dataset used for the analysis.

---

## Future Improvements

- Compare regression models with tree-based methods such as Random Forest and Gradient Boosting.
- Perform cross-validation for model evaluation.
- Evaluate regression performance using RMSE, MAE, and MSE.
