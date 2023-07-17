# credit-risk-classification

Overview of the Analysis
In this credit-risk-classification challenge, we created Logistic Regression Models with two sets of data to test and predict the healthy loan vs high-risk loan. We looked at several factors, such as loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, and total debt status that could affect the loan status. We first used the original data to run Logistic Regression model, and then used resampled data to run Logistic Regression model again to compare and contrast. 


First, we used to original data and created Logistic Regression Model. This data gave us a very high volume of healthy loan (75,036) vs high-risk loan (2500). We then trained and tested dataset using train_test_split. The accuracy of this model was 94.4%. The precision for the healthy loan was 100% whereas for high-risk loan was 87%. Also the recall for healthy loan was 100% vs high-risk loan 89%. It is harder to identify high rish loans because the sample data is too small compared to the healthy loan. 

           precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      0.89      0.88       625

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384


We then used resampled training data and created Logistic Regression Model. Through this resampled training data, the number of data points was the same between the ones for healthy loan and high-risk loan. The accuracy score of this model was 99.6% (vs 94.4% previously). The precision for healthy loan and high risk loan remained at 100% and 87%, respectively, but the recall for high-risk loan rose upto 100%.  

             precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      1.00      0.93       625

    accuracy                           1.00     19384
   macro avg       0.94      1.00      0.96     19384
weighted avg       1.00      1.00      1.00     19384



The logistic regression model performed better with oversampled data, providing us more accuracy when predicting high-risk loan. This is crucial because we need to identify the danger of high-risk loans prior to granting access to loans. For healthy loan, both model seem to work, but the oversampled data provides a better comparison. 
