# :chart_with_upwards_trend: Salary Prediction using Linear Regression

This repository contains a simple machine learning project focused on predicting employee salaries based on their years of professional experience using **Simple Linear Regression**.

---

## :dart: Project Overview & Purpose

The purpose of this project is to practice and demonstrate the core concepts of supervised regression learning:
- Analyzing the linear relationship between a single independent feature (Years of Experience) and a continuous dependent target variable (Salary).
- training a linear model using `scikit-learn`'s `LinearRegression` algorithm.
- Evaluating model fit and validating the linear equation mathematical model manually.

---

## :bar_chart: Dataset Information

- **Dataset Name**: `Salary_dataset.csv`
- **Source**: [Download from Google Drive](https://drive.google.com/file/d/1NiiFyW8Cr1g49mbK-qjv2_QIs5QSbApt/view?usp=sharing)
- **Features**:
  - `YearsExperience` (Numeric): The number of years of professional experience. (Independent variable / Input feature $X$).
  - `Salary` (Numeric): The annual salary of the employee in USD. (Dependent variable / Target label $Y$).

---

## :gear: Model Training Pipeline

The training process is completed in the following steps within the Jupyter Notebook:

1. **Exploratory Data Analysis (EDA)**:
   - Visualizing the data points on a 2D scatter plot using `matplotlib` to verify if they exhibit a linear pattern.

2. **Model Selection & Fitting**:
   - Using the `LinearRegression` class from `sklearn.linear_model`.
   - Fitting the model on the full feature space: $X$ = `YearsExperience` and $y$ = `Salary`.

3. **Mathematical Formulation**:
   The model maps inputs to outputs using the standard slope-intercept linear equation:
   $$y = w \cdot x + b$$
   
   From our training session, we extracted:
   - **Slope/Weight ($w$)**: `9449.96232146` (Representing salary increase per year of experience)
   - **Intercept ($b$)**: `24848.203966523208` (Base salary for 0 years of experience)
   
   Thus, the prediction formula is:
   $$\text{Salary} = 9449.96 \times (\text{Years of Experience}) + 24848.20$$

4. **Model Evaluation**:
   - **R-squared ($R^2$) Score**: **0.957 (95.7%)**, indicating that 95.7% of the variance in salary is explained by years of experience.
   - **Sample Prediction**: For **10.5 years of experience**, the model predicts a salary of **$124,072.81** (validated both via `.predict()` and the manual formula).

5. **Visualization of the Best-Fit Line**:
   - Plotting the regression line over the data points to visually evaluate model fit.

---

## :rocket: How to Run the Notebook

You can open and run this notebook directly in Google Colab without any local setup. Click the badge below:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/umertabraiz/machine-learning-practice/blob/main/notebooks/Linear_Regression.ipynb)

---
