* Advertising Campaign - Simple/Multi/Non-Linear Regression

This project builds 3 linear regression models to analyze and predict sales performance based on advertising spending across various channels. The dataset includes expenses on TV, radio, and newspaper advertisements, with the goal of identifying how total ad spend affects sales.

---

* Problem Statement

The business objective is to:

- Understand the relationship between total advertising spend and unit sales.
- Predict unit sales for an upcoming advertising campaign with a planned total spend of $200,000.

* Dataset Overview

The dataset contains:

- Independent Variables:
  - TV: Advertising cost on TV.
  - Radio: Advertising cost on Radio.
  - Newspaper: Advertising cost on Newspapers.

- Dependent Variable:
  - Sales: Number of units sold.



* Steps Followed
  
1. Business Understanding
- Formulated the sales prediction problem based on advertising budget.

2. Data Understanding
- Loaded and explored the dataset.
- Verified data integrity and structure.

3. Data Preprocessing
- Calculated total ad spend per campaign.
- Split the dataset into training and testing sets.

4. Modeling
- Used Simple Linear Regression

- Trained the model using `sklearn.linear_model.LinearRegression`.

5. Evaluation
- Used metrics:
  - R² Score (Train & Test)
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Cross-validation score (5-fold)

- Visualized:
  - Linearity of errors
  - Distribution of residuals

6. Final Model Summary
- Model generalizes well with Train R², Test R², and CV Score all within ±5% tolerance.
- Saved using `joblib` for reuse and deployment.

---

* Prediction

For a total ad spend of $200,000, the projected sales are predicted by: (may vary as per the model)

model.predict(pd.DataFrame({"Total Expenses": [200000]}))
