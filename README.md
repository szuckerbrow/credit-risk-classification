# credit-risk-classification
Machine learning techniques are used to analyze a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Overview of the Analysis

The purpose of this analysis was to use a variety of factors to classifier a loan as 'healthy' or 'high risk'

Factors considered in the analysis based on the data included:
- loan size
- interest rate
- borrower income
- debt to income ratio
- number of accounts
- derogatory marks
- total debt
- loan status

* The dataset contained 77,536 data points.
 

## Stages of the machine learning process
To complete this analysis, the following steps were taken:
- Separate the data into labels and features (independent and dependent variables)
- Split the data into training and testing sets
- Fit a logistic regression model using the training data
- Make predictions using the testing features data
- Evaluate the models performance using a confusion matrix and classification report

### Logistic Regression model
In this analysis, a logistic regression model was used. A logistic regression is a supervised machine learning algorithm that accomplishes binary classification by predicting the probability of an outcome. In this analysis, it was used to determine if a loan should be considered healthy (0) or high-risk (1). This was an appropriate model because the data was linearly separable and logistic regression models perform best when working with a larger sample size.

## Results

The logistic regression model performs very well in predicting both the 0 (healthy loan) and 1 (high-risk loan) labels, as indicated by the precision, recall, and F1-score metrics.

For the healthy loan class: 
- precision is 1.00, meaning when the model predicts a loan as healthy, it is correct 100% of the time.
- recall is 0.99, suggesting that the model captures 99% of the actual healthy loans.
- f1-score is 1.00, indicating a perfect balance between precision and recall.

For the high risk loan class:
- precision is 0.85, implying that when the model predicts a loan as high-risk, it is correct around 85% of the time.
- recall is 0.91, meaning the model captures 91% of the actual high-risk loans.
- f1-score is 0.88, which is a harmonic mean of precision and recall for this class.

These metrics collectively suggest that the logistic regression model is highly effective in predicting both classes, with particularly strong performance in identifying healthy loans and reasonably good performance in detecting high-risk loans.

## Summary
### Lender Recommendation
After completing this analysis, I recommend using this Logistic Regression Model to determine if loans should be classified as healthy or high-risk. In this context, it is safer for the lender to incorrectly label a loan as high-risk vs incorrectly labelling a loan as healthy. When loans were labeled healthy, the model was correct 100% of the time, so the lender can feel secure providing that loan. 

### Borrower Impact
There was more inaccuracy when labelling loans as high-risk. Although this is unfortunate for the potential borrowers, this is a safer model for the lender. Although prioritizing the lender's safety is necessary, it's essential to acknowledge the potential consequences for borrowers who may be unfairly categorized as high-risk.
