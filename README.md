# credit-risk-classification
In this analysis, machine learning techniques were employed to assess a dataset from a peer-to-peer lending services company, aiming to create a model capable of identifying the creditworthiness of borrowers.

## Key Factors Considered:
The analysis took into account several factors, such as the loan size, interest rate, borrower's income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

## Methodology:
The dataset, consisting of 77,536 data points, was divided into training and testing sets. An initial logistic regression model (Logistic Regression Model 1) was constructed using the LogisticRegression module from scikit-learn, which was then applied to the testing dataset.

## Resampling Process:
To address the class imbalance, the training data was resampled using the RandomOverSampler module from imbalanced-learn. This resulted in an equal number of data points for both low-risk (0) and high-risk (1) loans, based on the original dataset.

## Results:
Logistic Regression Model 1:
- Precision: 93% (100% precise in predicting low-risk loans, 87% precise in predicting high-risk loans)
- Accuracy: 94%
- Recall: 95% (100% recall in predicting low-risk loans, 89% recall in predicting high-risk loans)

Logistic Regression Model 2:
- Precision: 93% (100% precise in predicting low-risk loans, 87% precise in predicting high-risk loans)
- Accuracy: 100%
- Recall: 100%

## Conclusion:
Logistic Regression Model 2 exhibits fewer false negative predictions and higher accuracy and recall overall. While neither model achieves above 90% precision in predicting high-risk loans, Logistic Regression Model 2, with its higher accuracy and recall rates, is recommended for use.