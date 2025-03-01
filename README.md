# Customer Churn Prediction and Prevention, with Boosted Decision Trees (BDT) and Neural Networks

#### **_If you could predict which customers will leave your business, what would you do to keep them? Using AI-powered machine learning, I analyze churn drivers and propose targeted retention strategies._**



**Overview**: Losing (churning) customers costs money, and signing new customers is more expensive than retaining existing customers.  I analysis a dataset which captures a snapshot of customers at a central European bank in order to predict which customers are most likely to churn ([Kaggle, Bank Customer Churn](https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn/data)). The dataset includes customer use of bank products, their personal profiles, and their financial status. Through my analysis, I build a profile of churning customers and understand the most relevant factors in their decision to leave, in order to advise on business actions the bank can take to prevent this and retain custom.

**Methodology**: I utilise Exploratory Data Analysis (EDA) to get a meaningful understanding of the data and to make key predictions for customer churn.  I then train and optimise (with [Optuna](https://optuna.org/)) two Machine Learning classification algorithms to make predictions on unseen cross-validation and test datasets:
- Boosted Decision Tree (BDT) with [XGBoost](https://xgboost.readthedocs.io/en/stable/)
- Neural Network with [Tensorflow](https://www.tensorflow.org/)

I cross-check the ML algorithms against my EDA insights through the importance of different features in the data, using [SHAP Values](https://shap.readthedocs.io/en/latest/index.html).

**Key Business Insights**: The main casual indicators for customers to churn, confirmed by EDA and both ML algorithms, are:
- Age (45+)
- High-balance accounts
- High product use
- Location (Germany)
- Gender (females slightly more likely to leave than males)

The conclusion of this study is that this bank failed to retain older wealthier customers with high product use. These are customers who were highly engaged and may have expected VIP treatment. Almost every customer who churns also leaves a complaint with the bank, suggesting a degree of dissatisfaction with the service.

To retain such customers in the future <span style="color:red">**I would recommend the following actions:**</span>

- **Exclusive benefits for high-balance customers with multiple products**:
  - Priority Customer Services
  - Premium Credit Cards
  - Wealth Tiers and Loyalty Benefits
- **Specialised offers for older customers**:
  - Retirement Savings Accounts
  - Fixed-Income Investment Plans
  - Personalised Financial Advisory Services
- **Localised strategies for German customers**
  - Survey German customers to understand why they are leaving

If the bank wishes to perform more targeted interventions, the predictions of the ML algorithms may be used to provide a list of high-churn-risk customers to contact. This would be a worthwhile effort: the prediction has a 65% precision meaning that the majority of calls made will be to customers who are planning to leave, this maximises the customer service efficiency without hassling the vast majority of customers who intend to stay. Further, the prediction has a 61% churning-customer recall, meaning that the majority of customers who are planning to leave will be included in the high-churn-risk list.

**Contact**

If you have any questions, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/jacob-kempster-b75628114/) or check out the below for a deeper dive into this case study!

#### **_What strategies has your business used to retain high-value customers? Let me know in the comments!_**

