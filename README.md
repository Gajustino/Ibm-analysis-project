# Churn Analysis and Prediction - IBM HR Dataset

## Project Objective

This project aims to identify the key factors driving voluntary employee attrition at IBM. With a current churn rate of 16%, our goal is to understand the underlying patterns through data analysis and propose strategic actions to improve talent retention.

---

## Problem Statement

High employee turnover results in significant costs related to offboarding, recruitment, and training. This project seeks to analyze employee behavior based on historical data and answer the following questions:

- Which groups are most at risk of leaving?
- Which variables are most strongly correlated with churn?
- Can we predict which employees are most likely to leave?

---

## Project Stages

- Data import, cleaning and preprocessing  
- Conversion of ordinal variables to readable categories  
- Exploratory Data Analysis (EDA) focused on risk variables  
- Strategic visualizations and heatmaps  
- Data transformation for modeling (One-hot encoding)  
- Predictive modeling using a Decision Tree  
- Generation of insights and strategic recommendations  

---

## Tools and Libraries Used

- Pandas, NumPy  
- Matplotlib, Seaborn  
- scikit-learn  

---

## Key Analyses Performed

- Churn by salary range, age, tenure, and job involvement  
- Churn by categorical variables like job role, overtime, and satisfaction level  
- Heatmaps combining "Years at Company × Promotions" and "Age Range × Overtime"  
- Correlation between features and the target variable (Attrition)  
- Comparative visualizations by department and job role  

---

## Predictive Modeling

**Decision Tree** (`DecisionTreeClassifier`) with limited depth (`max_depth=3`) was used to understand the main churn-driving factors.

### Top variables in the model:

- **OverTime**: most influential risk factor  
- **MonthlyIncome**: lower salaries associated with higher churn  
- **TotalWorkingYears**: less experience increases attrition likelihood

---

## Key Findings

- Employees working overtime are **3x more likely** to leave  
- Young employees (18–24 years) and those with **less than 2 years at the company** show the highest churn rates  
- **Sales Representatives** and **HR** roles have the highest turnover  
- **Entry-level employees** are more likely to leave, possibly due to onboarding or expectation gaps  
- Salaries **below U$ 2,700** are strongly correlated with churn above 30%

---

## Strategic Recommendations

| Identified Issue                   | Suggested Strategic Action                                                 |
|------------------------------------|----------------------------------------------------------------------------|
| High overtime workload             | Monitor and compensate overtime with time off or bonuses                   |
| High turnover in entry-level roles | Strengthen onboarding and create accelerated development programs          |
| Lack of recent promotions          | Reinforce career development plans and structured feedback                 |
| Low initial salary                 | Reassess salary bands and offer non-financial incentives                   |
| Turnover among young/new employees | Implement structured onboarding for the first 6 months                     |
| High churn in HR and Sales         | Review goals, support systems, and work environment in these departments   |
