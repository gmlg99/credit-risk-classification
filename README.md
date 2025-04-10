# credit-risk-classification
The goal of this project was to build a logistic regression model that predicts the likelihood of a loan being high-risk. Using historical lending data, we created and tested models with both original and resampled training data to evaluate their ability to identify credit risk.

### Model with Original Data
- **Accuracy:** 99%
- **Precision (High-Risk Loans):** 0.88  
- **Recall (High-Risk Loans):** 0.68  

The model predicted healthy loans well but struggled to catch many high-risk loans. This imbalance made the model unreliable for identifying borrowers likely to default.

### Model with Resampled Data
- **Accuracy:** 99%
- **Precision (High-Risk Loans):** 0.91  
- **Recall (High-Risk Loans):** 0.99  

After applying oversampling to balance the training data, the model became much more effective at identifying both types of loans, especially high-risk ones. This adjustment significantly improved the recall and made the results more balanced.


The resampled logistic regression model is better suited for detecting high-risk loans. Its high recall score for riskier borrowers helps reduce the chance of approving risky loans. Because of its balanced performance, this version of the model is a strong candidate for use by the company.

This project was completed as part of a beginner data analytics bootcamp. It is intended for educational purposes only. All work was guided by course materials and publicly available documentation as well as external sources for help with errors.
