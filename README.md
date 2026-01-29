# Bank_Marketing_Campaigns
This project compares the performance of multiple classification models—Logistic Regression, K-Nearest Neighbors, Decision Trees, and Support Vector Machines—using a dataset related to the telephone marketing of bank products. 

A link to the completed Jupyter Notebook is provided below:
https://github.com/ninakaushik/Bank_Marketing_Campaigns/blob/main/prompt_III.ipynb

Business Understanding
The business problem addressed in this project is the inefficient use of resources in telephone marketing campaigns. Contacting clients who are unlikely to subscribe to a term deposit increases operational costs and can negatively impact customer experience. The objective of this analysis is to predict whether a client will subscribe to a term deposit, enabling the bank to prioritize outreach efforts, reduce unnecessary calls, and improve overall campaign efficiency.
This task is framed as a binary classification problem, where the target variable indicates whether a client subscribed to a term deposit (“yes” or “no”).

Data Understanding and Preparation
The dataset was examined for missing values, data types, and implicit missing categories (e.g., “unknown”). Descriptive statistics and visualizations were used to understand both categorical and continuous variables. The target variable was found to be highly imbalanced, reinforcing the need for appropriate baselines and evaluation metrics.
Feature engineering focused on bank client demographic information. Categorical variables were encoded using one-hot encoding, numeric variables were standardized where appropriate, and the data was split into training and test sets using stratification to preserve class proportions.

Modeling and Evaluation
Multiple machine learning models were trained and evaluated, including Logistic Regression, K-Nearest Neighbors, Decision Trees, and Support Vector Machines. A baseline model was established to provide a minimum performance benchmark. Models were compared using training accuracy, test accuracy, and training time.
Cross-validation was incorporated through GridSearchCV, and hyperparameter tuning was performed to improve model performance. Evaluation metrics were clearly identified and justified, with alternative metrics explored to better account for class imbalance. Logistic Regression coefficients were interpreted to explain the direction and relative importance of features in predicting term deposit subscription.

Findings and Actionable Insights
The analysis demonstrates that not all clients should be contacted equally. Client demographics and prior campaign behavior show meaningful relationships with subscription outcomes. Logistic Regression provided a strong and interpretable model with consistent generalization performance, while more complex models introduced trade-offs between computational cost and interpretability.
These findings indicate that predictive modeling can be used as a decision-support tool to guide marketing strategy rather than relying on uniform outreach.

Next Steps and Recommendations
Based on the results of this analysis, the bank should move toward a more targeted approach to telephone marketing by prioritizing clients with a higher likelihood of subscribing to a term deposit. Ranking clients by predicted likelihood allows marketing teams to allocate call center resources more efficiently and reduce unnecessary outreach.
The bank should also establish clear guidelines around follow-up contact frequency to avoid diminishing returns and customer fatigue. Finally, outreach strategies should be reviewed and refined over time as customer behavior and economic conditions change, ensuring that marketing efforts remain effective, efficient, and aligned with business objectives.
