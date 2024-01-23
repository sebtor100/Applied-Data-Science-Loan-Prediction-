# Applied-Data-Science-Loan-Prediction-
Loan Prediction Techniques

# Loan Default Prediction
## Problem Definition
## The Context:
In the contemporary landscape of retail banking, a significant proportion of profits stems from interest accrued through home loans, primarily extended to customers with regular or high income. However, the specter of loan defaulters poses a considerable threat to banks, as non-performing assets (NPAs) can substantially erode profits. Therefore, the approval process for these loans is a multifaceted challenge, traditionally relying on manual assessments of applicants' creditworthiness. Yet, this approach is not only labor-intensive but also susceptible to human errors and biases.

Recognizing the limitations of heuristic-based automation attempts, many banks are turning to the power of data science and machine learning to revolutionize the loan approval process. The goal is to develop machine learning models capable of learning the intricacies of the approval process, eliminating biases, and enhancing efficiency. However, a crucial consideration in this endeavor is to ensure that the machine does not inherit biases ingrained in the historical human approval process.

## The objective:
The primary objective is to build a classification model capable of predicting clients likely to default on their loans. Additionally, the model should provide actionable recommendations to the bank regarding crucial features to consider during the loan approval process.

## Conclusions:
Multiple machine learning models were built and evaluated, with the tuned Random Forest model achieving the best performance on key metrics like F1 score. It had scores of 0.95 for the non-default class and 0.78 for the default class.
The models were able to predict loan defaults with decent accuracy, outperforming a manual lending process. Key drivers of default risk were identified such as number of delinquencies, debt-to-income ratio and credit history length.
There is still room for improvement in model performance, especially for the minority default class. Additional applicant data could further boost accuracy.
## Recomendations:
The tuned Random Forest model should be deployed as the final solution due to its robust performance, interpretability and ability to balance precision and recall.
A two-step loan approval process is recommended. First, applicants should be classified as likely defaulters or not using the Random Forest model. Then a second regression model can predict uitable loan amounts for non-defaulters.
The key drivers of default risk should inform lending policy and credit worthiness evaluation during the manual underwriting process as well. Applicants with long credit history and low debt ratios should be preferred.
Additional data like income stability, payment behavior with other lenders, personal obligations etc. should be collected in loan applications wherever possible. This can feed into incremental model improvements over time.
Appropriate thresholds need to be set for default probability beyond which loans get rejected. These cut-offs require business input based on risk appetite.
