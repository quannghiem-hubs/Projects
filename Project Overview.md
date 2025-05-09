# Waze – User Churn Prediction Model Proposal

## Overview

This project focuses on predicting **user churn for the Waze navigation app**. By identifying users at high risk of churning, we aim to support **targeted retention strategies**, improve user experience, and drive business growth. The project follows the **PACE (Plan, Analyze, Construct, Execute)** workflow and includes structured tasks and milestones.

---

## Milestones & Deliverables

| Milestone | Tasks                         | Deliverables/Reports                                 |
|----------:|-------------------------------|------------------------------------------------------|
| 1         | Establish project workflow    | Global project document outlining goals, milestones  |
| 1a        | Write a project proposal      | Defined project structure and workflow               |
| 2         | Compile data summary          | Data files ready for EDA                             |
| 2a        | Begin data exploration        | Cleaned and structured dataset for analysis          |
| 3         | Perform data cleaning and EDA | EDA report                                           |
| 3a        | Create visualizations         | Tableau dashboard/visuals                            |
| 4         | Compute descriptive statistics| Test analysis between two variables                  |
| 4a        | Conduct hypothesis testing    | Regression model predicting churn                    |
| 5         | Build regression model        | Statistical test results, hypothesis report          |
| 5a        | Evaluate model performance    | Model evaluation summary                             |
| 6         | Build machine learning model  | Final predictive model                               |
| 6a        | Communicate final insights    | Final project report with actionable insights        |

---

## Tools & Technologies

- Python (Pandas, Scikit-learn, Statsmodels)
- Tableau (Data visualization)
- Jupyter Notebook
- GitHub for version control and collaboration

---

## Expected Outcomes

- Identified key predictors of user churn
- Trained ML model with actionable churn probabilities
- Dashboards and reports for business stakeholders
- Strategic insights to improve Waze user retention

---

## 📂 Project File Breakdown

Below is a summary of the key Jupyter notebooks used in this project, aligned with major tasks:

- **DataExploration.ipynb**: Data exploration and basic cleaning using pandas.
- **Initial EDA.ipynb**: Initial EDA and summary statistics.
- **Hypothesis testing and regression modeling.ipynb**: Hypothesis testing and regression modeling.
- **Machine Learning.ipynb**: Machine learning model development and evaluation.
  
---

## Project Results & Conclusion

### Key Findings

- **Churn Indicators Identified**:
  - **Low satisfaction levels** and **low engagement (fewer active days/month)** were the strongest predictors of churn.
  - **Users with fewer completed navigations**, **infrequent usage**, and **high report-to-trip ratios** also showed a higher churn tendency.
  - **No meaningful impact** was observed from age or city-specific features, suggesting churn is behavior-driven, not demographically driven.

- **Statistical Testing**:
  - Hypothesis tests confirmed a **statistically significant difference in satisfaction** and **average usage patterns** between churned and retained users.
  - Regression analysis demonstrated that satisfaction, average days active, and user engagement significantly influenced the churn probability.

- **Model Performance**:
  - The **logistic regression model** achieved moderate precision but struggled with recall due to class imbalance.
  - The **Random Forest model**, tuned with GridSearchCV, outperformed others, achieving:
    - **Accuracy**: ~82%
    - **F1 Score (Churn class)**: ~0.66
    - **ROC AUC**: ~0.84
  - Feature importance analysis confirmed the central role of **user activity frequency** and **satisfaction-related behaviors**.

### Final Deliverables

- A **machine learning model** capable of predicting high-risk churn users with strong ROC-AUC.
- A clear **set of behavioral churn drivers** that Waze can act on for retention marketing.

---

## Conclusion

The analysis confirms that **user behavior and satisfaction are primary churn drivers** for Waze. By leveraging the final predictive model, the business can:
- **Flag high-risk users early**, enabling timely re-engagement campaigns.
- **Tailor the user experience** to reduce churn probability.
- **Inform product and UX enhancements** based on behavioral insights.

These insights equip Waze with data-driven strategies to **optimize retention** and sustain **long-term user engagement**.



