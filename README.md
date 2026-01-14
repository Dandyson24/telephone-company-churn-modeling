
📉 Telco Customer Churn Analysis with Logistic Regression

####                                    Project Summary

Customer churn is one of the most expensive problems in subscription-based businesses. In this project, I explored a real-world telecommunications customer dataset to understand why customers leave and to build a predictive churn model using logistic regression.

Rather than focusing only on model accuracy, this project emphasizes:

- Interpretability

- Business relevance

- Actionable insights

The goal is to demonstrate how data science can support real business decisions, not just generate predictions.

####                                       Business Objective

To identify customers who are at risk of churning and uncover the key factors influencing churn, so the business can take proactive retention actions instead of reacting after customers leave.

####                                        Dataset Overview

The dataset contains customer-level information including:

Demographics (gender, senior citizen status, dependents)

Account details (tenure, contract type, payment method)

Service usage (internet service, streaming, tech support)

Billing information (monthly and total charges)

Target Variable:

Churn (Yes / No)

####                                      Approach & Methodology

Data cleaning and preprocessing

Exploratory Data Analysis (EDA)

Encoding categorical variables

Feature scaling

Logistic regression model training

Model evaluation using classification metrics

Interpretation of model coefficients

Business-focused recommendations


###                                              Exploratory Data Analysis (EDA)

#### Churn Distribution

This visualization shows the proportion of customers who churned versus those who stayed.

What it shows:
The dataset is moderately imbalanced, with more customers staying than leaving. This reinforces the need to look beyond accuracy when evaluating the model.

![Churn Pie Chart](https://github.com/Dandyson24/telephone-company-churn-modeling/blob/main/churn_pie_chart.png?raw=true)

### Tenure and Churn

This chart compares customer tenure for churned and non-churned customers.

Insight:
Customers with shorter tenure are significantly more likely to churn, highlighting the importance of early customer engagement and onboarding.

![Tenure vs Churn](https://github.com/Dandyson24/telephone-company-churn-modeling/blob/main/mean_tenure_by_churn.png?raw=true)

### Monthly Charges and Churn

This visualization explores the relationship between monthly charges and churn.

Insight:
Customers paying higher monthly charges show a higher churn tendency, suggesting price sensitivity and perceived value concerns.

![Monthly Charges vs Churn](https://github.com/Dandyson24/telephone-company-churn-modeling/blob/main/av_monthly_charges_by_churn.png)

### Model Performance

The churn prediction model was built using logistic regression, and was chosen for its balance between performance and interpretability.

📈 Key Metrics

Accuracy: ~79%

Precision (Churn): ~63%

Recall (Churn): ~52%

F1-score (Churn): ~57%

####                                  Interpretation:

- The model performs strongly in identifying customers who will not churn.

- Recall for churn is moderate, which is common in churn problems.

- The model is suitable for risk scoring and targeted retention, especially when combined with business rules.

![Classification Report](https://github.com/Dandyson24/telephone-company-churn-modeling/blob/main/classification_report.png?raw=true)

####              Confusion Matrix

The confusion matrix helps visualize correct and incorrect predictions.

While some churn cases are missed, the model provided valuable early signals that can guide retention strategies before customers leave.

![Confusion Matrix](https://github.com/Dandyson24/telephone-company-churn-modeling/blob/main/confusion_matrix.png?raw=true)

####  ROC Evaluation
![ROC_AUC CURVE](https://github.com/Dandyson24/telephone-company-churn-modeling/blob/main/roc_curve.png?raw=true)

####                    Feature Interpretation (Why Customers Churn)

One advantage of logistic regression is transparency. By analyzing model coefficients, we can see which features influence churn.

  **Factors Increasing Churn Risk**

Month-to-month contracts

Short customer tenure

Higher monthly charges

Lack of add-on services

**Factors Reducing Churn Risk**

Long-term contracts

Tech support and online security

Longer tenure

This makes the model easy to explain to non-technical stakeholders.

![Feature Coefficients](https://github.com/Dandyson24/telephone-company-churn-modeling/blob/main/Features.png?raw=true)

####                  Business Recommendations

Strengthen engagement during the first few months of customer tenure

Incentivize customers to move from month-to-month to long-term contracts

Introduce loyalty pricing or bundled offers for high-risk customers

Promote value-added services such as tech support

####                  Tools & Technologies

Python

Pandas & NumPy

Scikit-learn

Matplotlib / Seaborn

Jupyter Notebook


####                Next Steps

- Test tree-based models for improved churn recall

- Continue tuning classification thresholds to improve accuracy

- Deploy churn scoring for real-time retention use

- Build an interactive Power BI dashboard

**Author**: Andrew Nwachimere-eze Okebugwu
LinkedIn: https://www.linkedin.com/in/andrew-nwachimereze-okebugwu-mbbs-mph-phd-6b429617/
