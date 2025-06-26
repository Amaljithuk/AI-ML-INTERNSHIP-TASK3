Titanic Linear Regression
Task Overview
This repository contains the solution for Task 3 of the Elevate AI & ML Internship. The objective is to implement simple and multiple linear regression on the Titanic dataset to predict Fare, using a Jupyter Notebook.
Steps Performed

Data Preprocessing:
Handled missing values: Age (median), Embarked (mode), dropped Cabin.
Encoded categorical features: Sex (label encoding), Embarked (one-hot encoding).
Standardized numerical features (Age, Fare, SibSp, Parch).
Removed outliers using the IQR method.


Exploratory Data Analysis:
Generated summary statistics and a correlation matrix to understand feature relationships.


Linear Regression:
Simple linear regression: Predicted Fare using Pclass.
Multiple linear regression: Predicted Fare using all features.
Evaluated models using MAE, MSE, and R².
Plotted the regression line for simple linear regression and interpreted coefficients.



Files

titanic_linear_regression.ipynb: Jupyter Notebook with preprocessing, EDA, and linear regression code.
Titanic-Dataset.csv: Original Titanic dataset.
Titanic-Cleaned-Dataset.csv: Preprocessed dataset.
correlation_matrix.png: Correlation matrix heatmap.
simple_regression_line.png: Regression line for simple linear regression.
README.md: This documentation file.

Tools Used

Python 3
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn
scikit-learn

How to Run

Clone this repository:git clone https://github.com/Amaljithuk/AI-ML-INTERNSHIP-TASK3.git


Install required dependencies:pip install pandas numpy matplotlib seaborn scikit-learn jupyter


Launch Jupyter Notebook:jupyter notebook


Open titanic_linear_regression.ipynb and run all cells to:
Generate the cleaned dataset (Titanic-Cleaned-Dataset.csv).
Save visualizations (correlation_matrix.png, simple_regression_line.png).
Display model metrics and interpretations.



Observations

EDA: Strong negative correlation between Pclass and Fare (~-0.7), indicating higher-class passengers paid more.
Simple Linear Regression: Low R² suggests Pclass alone is insufficient to predict Fare. Negative coefficient confirms higher classes paid more.
Multiple Linear Regression: Higher R² and lower MAE/MSE indicate better fit with all features. Pclass is the strongest predictor.
Inferences: Fare’s skewness may violate linearity assumptions, suggesting potential log-transformation for improved modeling.

Notes

The notebook uses explicit assignments to avoid Pandas FutureWarning for fillna.
The cleaned dataset is suitable for regression tasks.
Visualizations and metrics provide insights into model performance and feature importance.

Submission
This repository is submitted for Task 3 of the Elevate AI & ML Internship, completed on June 26, 2025, within the 10:00 AM to 10:00 PM submission window.
