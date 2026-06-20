# House Price Prediction Using Machine Learning

## Project Overview

This project focuses on predicting residential property prices using Machine Learning techniques. The objective is to analyze housing features, identify the factors that influence house prices, and build predictive models capable of estimating property values accurately.

## Problem Statement

Real estate buyers and sellers often rely on guesswork or outdated comparisons to estimate a property's fair value. This project aims to develop a regression model that predicts house prices based on features such as area, number of bedrooms, bathrooms, stories, parking facilities, and additional amenities.

---

## Dataset

**Source:** Kaggle Housing Prices Dataset

Dataset Link:
https://www.kaggle.com/datasets/yasserh/housing-prices-dataset

The dataset contains information about residential properties including:

- Area
- Bedrooms
- Bathrooms
- Stories
- Parking
- Main Road Access
- Air Conditioning
- Basement
- Furnishing Status
- Preferred Area
- House Price (Target Variable)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

## Project Workflow

### 1. Data Loading & Exploration

- Loaded dataset using Pandas
- Examined dataset structure
- Identified target and feature variables
- Checked for missing values

### 2. Data Cleaning

- Removed duplicate records
- Verified missing values
- Applied One-Hot Encoding to categorical variables
- Prepared data for machine learning

### 3. Model Building

Two regression models were trained and evaluated:

#### Linear Regression

Performance:
- MAE: 970,043
- RMSE: 1,324,507
- R² Score: 0.653

#### Random Forest Regressor

Performance:
- MAE: 1,021,546
- RMSE: 1,400,566
- R² Score: 0.612

---

## Model Comparison

| Model | MAE | RMSE | R² Score |
|---------|---------|---------|---------|
| Linear Regression | 970,043 | 1,324,507 | 0.653 |
| Random Forest Regressor | 1,021,546 | 1,400,566 | 0.612 |

Linear Regression achieved the best performance on this dataset.

---

## Visualizations

The project includes:

1. House Price Distribution
2. Correlation Heatmap
3. Actual vs Predicted Prices
4. Price vs Area Analysis
5. Feature Importance Analysis
6. Furnishing Status vs Price

---

## Key Findings

- Area was the most influential factor affecting house prices.
- Bathrooms had the second highest impact on property value.
- Air conditioning, parking, and stories significantly influenced pricing.
- Linear Regression outperformed Random Forest on this dataset.
- The model explained approximately 65% of the variation in house prices.

---

## Project Structure

```text
House-Price-Prediction/

├── analysis.ipynb
├── Housing.csv
├── summary.pdf
├── README.md

├── charts/
│   ├── price_distribution.png
│   ├── correlation_heatmap.png
│   ├── actual_vs_predicted.png
│   ├── price_vs_area.png
│   ├── feature_importance.png
│   └── furnishing_status_price.png
```

## Requirements

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

---

## Conclusion

This project successfully developed machine learning models to predict house prices using housing characteristics. Through data preprocessing, exploratory data analysis, visualization, and model evaluation, meaningful insights were obtained regarding the factors influencing house prices. The Linear Regression model achieved the best performance with an R² score of 0.653 and demonstrated the practical application of machine learning in real estate price prediction.
