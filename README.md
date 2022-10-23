# Credit_Risk_Analysis
Looking at known data, I am using linear regression and random forest models to predict potential credit default

## Overview of the analysis
Using multiple models and methods, the purpose of this analysis is to see if I can create a model that effectively predicts whether a customer is high or low risk for credit worthyness.

First, I shaped and cleaned the data to me needs:
![Alt text](https://github.com/thegreatkeej/Credit_Risk_Analysis/blob/main/images/Picture1.png)

Second, I split the data up for testing and training:
![Alt text](https://github.com/thegreatkeej/Credit_Risk_Analysis/blob/main/images/Picture2.png)

Third, I created a model and a confusion matrix:
![Alt text](https://github.com/thegreatkeej/Credit_Risk_Analysis/blob/main/images/Picture3.png)
## Results

### Credit Risk Resampling
•	Using random Oversampling with a Logistic Regression model: 

	Balanced Accuracy:     65.7%

	Precision:  Low Risk= 99.99%            High Risk=      1%

	Recall:        Low Risk= 60%            High Risk=     71%


•	Using SMOTE Oversampling with a Logistic Regression model: 

	Balanced Accuracy:     66.2%

	Precision:  Low Risk= 99.99%            High Risk=      1%

	Recall:        Low Risk= 63%            High Risk=     69%


•	Using random Undersampling with a Logistic Regression model: 

	Balanced Accuracy:     54.4%

	Precision:  Low Risk= 99.99%            High Risk=      1%

	Recall:        Low Risk= 40%            High Risk=     69%


•	Using Combination Sampling with a Logistic Regression model: 

	Balanced Accuracy:     69%

	Precision:  Low Risk= 99.99%            High Risk=      1%

	Recall:        Low Risk= 57%            High Risk=     80%


### Credit Risk Ensemble
•	Using a Balanced Random Forest Classifier model: 

	Balanced Accuracy:     87.3%

	Precision:  Low Risk= 99.99%            High Risk=     3%

	Recall:        Low Risk= 87%            High Risk=     70%


•	Using an Easy Ensemble AdaBoost Classifier model: 

	Balanced Accuracy:     94.2%

	Precision:  Low Risk= 99.99%            High Risk=     9%

	Recall:        Low Risk= 94%            High Risk= 92%

## Summary
The Easy Ensemble AdaBoost Classifier model performed the best regarding predicting a high risk customer. I reccommend using a Naive Bayes model on the data set. Naive Bayes works well on imbalanced sets. Another change would be to normalize all feature values and to run the model using the top (3) most significant features. I believe that would produce better results.