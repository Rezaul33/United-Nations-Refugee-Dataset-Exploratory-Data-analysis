# United Nations Refugee Data Analysis 🌍

[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)

## Project Overview
This project performs exploratory data analysis and machine learning modeling on **United Nations** refugee data from 1951-2023 as apart of my partial fullfilment of my Data Analyst Internship  at **Save the Children International**. The analysis includes data cleaning, feature engineering, and implementation of various regression models to predict refugee numbers using open-source data from Kaggle.

## Features
- Data cleaning and preprocessing
- Feature engineering with one-hot encoding
- Correlation analysis and feature selection
- Implementation of multiple regression models
- Model performance comparison and evaluation

## Regression Models Implemented
The following regression algorithms were used to analyze and predict refugee patterns:

1. **Linear Regression**
   - Simple and interpretable
   - Assumes linear relationship between features and target variable

2. **Ridge Regression**
   - Extension of linear regression with regularization
   - Prevents overfitting by penalizing large coefficients

3. **Lasso Regression**
   - Includes regularization for feature selection
   - Forces some coefficients to zero

4. **ElasticNet Regression**
   - Combines Ridge and Lasso regularization
   - Balances feature selection and regularization

5. **Decision Tree Regression**
   - Non-linear regression algorithm
   - Captures complex feature relationships

6. **Random Forest Regression**
   - Ensemble learning method using multiple decision trees
   - More robust and less prone to overfitting

7. **Gradient Boosting Regression**
   - Sequential ensemble learning method
   - Each tree corrects previous errors


8. **K-Nearest Neighbors (KNN)**
   - Non-parametric method
   - Predicts based on nearest neighbor averages


## Data Processing Steps
1. Data Cleaning
   - Removed ISO country codes
   - Handled missing values
   - Standardized numeric columns
2. Feature Engineering
   - One-hot encoding for country variables
   - Feature correlation analysis
   - Removal of highly correlated features
3. Data Preprocessing
   - Train-test split (80-20)
   - Feature scaling
   - Missing value imputation


## Implemented Models and Performance

| Model Type | MSE | RMSE | R² Score |
|------------|-----|------|----------|
| Linear Regression | 2.31e+11 | 480,934.21 | 0.256 |
| Ridge Regression | 2.31e+11 | 480,934.21 | 0.256 |
| Lasso Regression | 2.32e+11 | 481,791.44 | 0.253 |
| ElasticNet | 2.32e+11 | 481,791.44 | 0.253 |
| Decision Tree | 2.42e+11 | 491,456.32 | 0.258 |
| Random Forest | 1.98e+11 | 445,237.89 | 0.389 |
| Gradient Boosting | 1.33e+11 | 364,142.65 | 0.587 |
| KNN | 2.44e+11 | 493,561.78 | 0.201 |


### Best Performing Models:
1. **Gradient Boosting**: Best overall performance with R² = 0.587
2. **Random Forest**: Second best with R² = 0.389
3. **Decision Tree**: Third best with R² = 0.258


## Project Structure
```
├── Dashboard Images/
├── data/
│   ├── United Nations Refugee Data.csv
│   ├── United Nations Refugee Data cleaned.csv
│   ├── United Nations Refugee Data cleaned_Augmented.csv
│   └── United Nations Refugee Data filtered.csv
├── Notebook.ipynb
├── requirements.txt
└── README.md
```

## Setup and Installation
1. Clone the repository
2. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage
1. Open the Jupyter notebook:
```bash
jupyter notebook "EDA on United Nations Refugee Data.ipynb"
```
2. Run the cells in sequence to reproduce the analysis

## Requirements
- Python 3.10+
- See requirements.txt for package dependencies