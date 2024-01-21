# CS5262 Programming Project

### Background

The project goal is to detect if new payment transactions are fraudulent or not. The dataset to use is https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022. This dataset is realistic, and imbalanced, and have removed PII (personal identifiable information) for the privacy purpose. In this project, I want to answer what kind of user segment and behavior is flagged as fraudulent which could potentially answer data scientists and engineers to develop features to prevent these frauds. I also want to use various classification algorithms to see which algorithm performs the best. This dataset is from NeurIPS 2022 and a detailed publication is here https://arxiv.org/abs/2211.13358.

### Project Description

The project is to answer business questions like what kind of behaviors are flagged as fraudulent and guide developer teams to develop proper prevention mechanism to block fraudulent transactions in future. Another aspect of project is to test and implement various classification algorithms to see which can performs the best.

### Metrics

- True Positive - A legitimate fradulent account is classified as fraudulent
- True Negative - A non-fraudulent account is classified as non-fraudulent
- False Positive - A legitimate non-fraudulent account is classified as fraudulent
- False Negative - A fraudulent account is classified as non-fraudulent


