# 🏠 House Price Prediction using Machine Learning

## Overview

This is an end-to-end **Data Science** project that predicts house prices using the **Bengaluru House Price Dataset**. The project covers the complete machine learning workflow, including data cleaning, feature engineering, exploratory data analysis, outlier removal, model training, and evaluation.

## Dataset

* **Dataset:** Bengaluru House Price Dataset
* **Source:** Kaggle
* **Original Records:** 13,320
* **Records After Preprocessing:** 12,513

## Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab

## Project Workflow

1. Loaded and explored the dataset.
2. Handled missing values.
3. Converted `size` into a numerical `bhk` feature.
4. Cleaned the `total_sqft` column by converting ranges into numeric values.
5. Created `price_per_sqft` and `sqft_per_bhk` for analysis.
6. Removed unrealistic and location-wise outliers.
7. Applied One-Hot Encoding to categorical features.
8. Trained and compared multiple regression models.
9. Selected the best-performing model based on evaluation metrics.

## Models Compared

| Model             |       MAE |      RMSE |  R² Score |
| ----------------- | --------: | --------: | --------: |
| Linear Regression |     42.59 |    100.67 |     0.511 |
| Decision Tree     |     36.32 |    101.44 |     0.504 |
| **Random Forest** | **31.13** | **90.98** | **0.601** |

### Best Model

The **Random Forest Regressor** achieved the best performance with:

* **R² Score:** 0.601
* **MAE:** 31.13 Lakhs
* **RMSE:** 90.98 Lakhs

## Project Structure

House-Price-Prediction/
├── BengaluruHousePrice.ipynb
├── Bengaluru_House_Data.csv
├── actual_vs_predicted.png
├── requirements.txt
└── README.md

## Sample Visualization

The project includes an **Actual vs Predicted Price** scatter plot to evaluate model performance.

## Key Learning Outcomes

* Data Cleaning and Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Outlier Detection and Removal
* One-Hot Encoding
* Regression Modeling
* Model Evaluation using MAE, RMSE, and R² Score

## Future Improvements

* Hyperparameter tuning using GridSearchCV.
* Cross-validation for better model evaluation.
* Streamlit web application for interactive price prediction.
