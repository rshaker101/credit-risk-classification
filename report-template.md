# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis:
Determining if the Logisitic Regression model can be accuarte enough to predict healthy loans vs. high risk loans using original data vs. 
resampled data to increase the size of the minority class.
* Explain what financial information the data was on, and what you needed to predict.
loan_status is the prediction.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
original
value_counts:
0    75036
1     2500

oversampled:
0    56271
1    56271
* Describe the stages of the machine learning process you went through as part of this analysis.
1.Prepare the data,
2.Seperate data to features/columns where X and y are the outcome/labels
3.Train_test_split
4.Pick the machine learning model for best classification(LogisticRegression)
5.Fit the model with training data
6.Use the model make predictions with the test data, 25% default test data to be evaluated
7.Evaluate the predictions comparing metrics, confusion matric, classification report.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
SKLearn LogisticRegression
train_test_split
confsuion_matrix
classification_report

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 
  * Accuracy: 0.99,
  * Precision Class 0: 1.00, Class 1: 0.85
  * Recall scores: Class 0: 0.99, Class 1: 0.91



* Machine Learning Model 2:
 * Description of Model 2 
 * Accuracy: 0.99,
 * Precision Class 0: 1.00, Class 1: 0.84
 * Recall scores: Class 0: 0.99, Class 1: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
The Logestic Regression model preformed very well and made very good predictions on '0' healthy loans
for class '0'. recall and precision were very high. As for the '1' class determing high risk loans, the model precision is 0.84 and its recall was 0.91. This shows that the model gives more often false postives. Although the model has a high score it should be tested and evaluated with different data to confirm if it should be used for prediction.
If you do not recommend any of the models, please justify your reasoning.
