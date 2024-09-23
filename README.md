
Credit Risk Analysis Report

The purpose of this project was to analyse a histroical data set of loan applicants provided by a Bank to build a predictive model that would assess the borrowers' credit worthiness for loan applications in the future. The Bank could then use this predictive model in the future to grant loans to healthy loan applicants and minimize granting to those who would default on the loans.

The data set consisted of 77, 536 applicants and the data file consisted of the following fields:

a)Size of the loan
b)Interest rate on the loan
c)Borrower's income
d)Debt_to_Income ratio
e)The number of of accounts that the borrower uses regularly
f)Derogatory marks on the borrower's credit report
g)The borrower's total debt
h)loan status - '0' indicates a healthy loan applicant and '1' indiactes an applicant that defaulted and is considered a high risk


After removing the loan status column from the data set, the data was split into training and testing data. The default percentages were used to spilt the data which was 75% for training and 25% for testing.  The training data was then fitted to a logistic regression model and then the model was used to predict the test data. A confusion matrix and a classification report was generated to evaluate the model performance.


1)The accuracy - The accuuracy shows how often a classification machine learning model is correct overall.
The weighted accuracy of the Logistic Regression model was  99% for both precision and recall. The weighted accuracy takes the mean of all per class scores weighted by sample size for each class.
The Macro accuracy is an unweighted mean and was 92% and 95% for healthy loans and high risk loans resoectively.
The weighted accuracy is a better measure and we can conclude that the regression model had an overall accuracy of 99% which indicates it is a good model.

2)Precision  - The precision value shows how often a machine learning model is correct when predicting the target class.
For this model the precision was 100% for healthy loan applicants and was 85% for high risk loan applicants. Therefore the model does a better job at predicting healthy loan applicants than hgih risk applicants while the value still falls within an acceptable rate.


3)Recall Score - Recall score is a metric that measures how well a machine learning model can identify positive instances in a data set.  The recall score for healthy loan applicants was 99% and the recall score for high risk applicants was 91% which indicates that the model performs better at identifying healthy loan applicants than high risk applicants.

Summary 

Overall this logistic regression model predicts the healthy loans('0') at a very high percentage(100%). The precision value of 1.00 indicates this. High risk loans('1) are predicted at 85% which is lower than the prediction of healthy loans but is still within an acceptable range. Tt is mportant to be able to predict the '1's correctly as these are the high risk loans that would affect the financial health of the Bank.  Out of a total number of 19,384 applicants predicted by this model, 18663 were true positives, 56 were false positives, 102 were false negatives and 563 were true negatives.Overall the model is better at predicting healthy loan applicants than high risk applicants.  As the true negatives are a high enough number, I would recommend this model and believe the Bank would benefit by using this model 
