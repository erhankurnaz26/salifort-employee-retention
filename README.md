# Salifort Motors — Employee Retention Prediction
A machine learning project that predicts employee turnover and provides data-driven recommendations to improve retention at Salifort Motors.

#### Project Overview
Salifort Motors' HR department collected survey data from employees but lacked the analytical capability to extract actionable insights. This project addresses the core business question:
"What factors are most likely to make an employee leave the company?"
By building predictive models on top of exploratory data analysis, this project helps HR proactively identify at-risk employees and understand the structural causes of attrition — before it becomes a costly problem.

#### Exploratory Data Analysis
Key patterns uncovered during EDA:

Employees who left clustered into two distinct groups: those with very low satisfaction and high hours, and those with high evaluation scores but still resigned — suggesting burnout among top performers.
Employees managing 6–7 projects had significantly higher attrition rates.
Staff who had been at the company 3–4 years were the most likely to leave, particularly those with no promotion.
Monthly hours averaged 201 across all employees — well above a healthy full-time baseline — pointing to a systemic overwork problem.
Only 2.1% of employees received a promotion in the last 5 years.

### Models Built
Three classification approaches were implemented and evaluated:
1. Logistic Regression (baseline)
2. Decision Tree (tuned with GridSearchCV)
3. Random Forest (tuned with GridSearchCV)

Hyperparameters tuned: max_depth, max_features, max_samples, min_samples_leaf, n_estimators
Modestly outperformed the Decision Tree across all metrics
Feature importances extracted via Gini impurity
