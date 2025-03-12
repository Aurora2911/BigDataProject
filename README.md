# BigDataProject
The structure of this document is based on the industrial standard CRISP-DM (CRoss Industry Standard Process for Data Mining).  However, since this is an academic project for a university exam, the Evaluation and Deployment phases will not be performed, as it is unnecessary to extend the process beyond model development and technical assessment.

## Process Phases
1. Business Understanding
- Objective: Predict flight departure delays to enhance airport operational management.
- Key Performance Indicators (KPIs): Operational efficiency and customer satisfaction.

2. Data Understanding
- Data Source: Kaggle dataset available at

  https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023/data?select=flights_sample_3m.csv 
- Preliminary Analysis: Identification of missing values and inconsistencies in date and time formats.

3. Data Preparation
- Data Cleaning: Removal of irrelevant columns and handling of missing values.
- Feature Selection: Identification of the most relevant variables using Mutual Information.

4. Modeling
Tested Algorithms:
- Bagging: Random Forest, Extra Trees.
- Boosting: AdaBoost, Gradient Boosting, XGBoost.
- Data Partitioning: 80% training, 20% test.
- Evaluation Metrics: MAE, MSE, RMSE.

5. Results
- Gradient Boosting achieved the highest accuracy (MAE: 4.55, RMSE: 14.74) but required significant training time.
- XGBoost provided the best trade-off between accuracy and computational efficiency.
- Bagging techniques (Random Forest, Extra Trees) demonstrated lower predictive performance.
- AdaBoost was the least effective model.

## Conclusions
Boosting techniques outperformed Bagging methods in predicting flight departure delays. 
XGBoost emerged as the most balanced model in terms of predictive performance and training efficiency, whereas Gradient Boosting provided the highest accuracy at the expense of increased computational time.
