# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis. Create a predictive model to classify loans into eitehr healthy or high-risk loans based on financial information.
* Explain what financial information the data was on, and what you needed to predict. The following financial information was used for the model; loan size, interest rate borrower income,	debt to income, num of accounts, derogatory marks and total debt.  
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`). Loan status was the variable I was trying to predict.  If it was a healthy or high-risk loan.
* Describe the stages of the machine learning process you went through as part of this analysis. I split the data and then used sklearn to split the data into train and test sets using train-test_split. Then did a logistic regression model with the trained data. Then continued with predictions using the testing data and evaluated the model's performance using the confusion matrix and classification report.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms). Logistic regression was used to predict loan status.  Logistic regression is commonly used when the target variable has two classes. In this case healthy(0) and high-risk(1).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    Machine Learning Model 1:
    *Accuracy: 99%, which means that the model correctly predicts a loan as healthy 99% of the instances
    *Precision: For class 0(healthy loan), the precision is 100%. This indicates that when predicting a healthy loan the model is accurate 100% of the instances.  For class 1(high-risk loan), the precision is 84%. This means that the model is accurate 84% of the instances when predicting a high-risk loan.
    *Recall: For class 0, the recall is 99%. This suggests that the model correctly identifies 99% of healthy loans. For class 1, the recall is 94%.  The model identifies 94% of high-risk loans. 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best? The logistic regression model worked well having 99% accuracy. Also with high precision and recall scores on both classes it indicates that the model performs well indentifying healthy and high-risk loans.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? ) Performance does depend on the problem we are trying to solve. Both precision and recall are important metrics. Where precision measures the accuracy of positive predictions and recall measures the ability of the model to find all the relevant instances. It is important to predict '1''s (healthy loans) because if you don't then you could be missing out on potential good business. However, it is crucial to identify high-risk loans because giving loans to high-risk applicants could result in significant financial losses.


If you do not recommend any of the models, please justify your reasoning.
