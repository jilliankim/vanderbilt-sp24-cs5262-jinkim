# CS5262 Programming Project

### Background

The project goal is to detect if new payment transactions are fraudulent or not. The dataset to use is https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022. This dataset is realistic, and imbalanced, and have removed PII (personal identifiable information) for the privacy purpose. In this project, I want to answer what kind of user segment and behavior is flagged as fraudulent which could potentially answer data scientists and engineers to develop features to prevent these frauds. I also want to use various classification algorithms to see which algorithm performs the best. This dataset is from NeurIPS 2022 and a detailed publication is here https://arxiv.org/abs/2211.13358.

### Project Description

The project is to answer business questions like what kind of behaviors are flagged as fraudulent and guide developer teams to develop proper prevention mechanism to block fraudulent transactions in future. Another aspect of project is to test and implement various classification algorithms to see which can performs the best.

### Metrics

| | Positive | Negative |
|:-:|:-:|:-:|
| Positive | TP | FP |
| Negative | FN | TN |

Row: True Class
Col: Predicted Clas
- True Positive - Observation is Positive, and the model classified as Positive
- True Negative - Observation is Positive, but model classified as Negative
- False Positive - Observation is Negative, and the model classified it as Positive
- False Negative - Observation is Negative, but the model classified it as Positive

### Cost & Revenue

Assuming most users are non-fraudulent, the benefit of the model working would mostly come from TP and the loss would come from FN. Possibly the model can introduce bad user experience if FP is higher, but better safe than sorry.
For a population of 20 million customers, if 2% of the population is fraudulent, and had an average of $500 fraudulent transactions, and only 50% of those fraudulent transactions were caught (FN is high), that would already be $250 million loss. So it is imperative the model is tuned to lower FN rate, and this model can be on a bit conservative side, compensating bad user experience.

#### References
- https://www.jpmorgan.com/insights/payments/fraud-and-risk-management/payment-fraud-controls
- https://www.goldmansachs.com/what-we-do/transaction-banking/insights/payments-fraud.pdf

### Review Comments
- The use of the word legitimate in the metrics somewhat detracts from the readability, as it's implied that 'a non-fraudulent account' is the same as 'a legitimate non-fraudulent account'. Additionally fraudulent is misspelled in the True Positive case. Otherwise, the descriptions of each metric case are self consistent and appear correct.
- There don't appear to be any cost/spending/revenue estimates for any of the metrics cases yet. I'm assuming that is just due to not writing those yet, but I'm writing it in this comment anyways just to be sure.
- It may be a good idea to add a table with the confusion matrix, for the sake of presenting it in the same way that it was presented in class.
