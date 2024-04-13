# Upgrad-Capstone-Project - FindDefault (Credit card fraud detection)

FindDefault - Credit Card Fraud Detection 

Problem Statement:
We have to build a classification model to predict whether a transaction is fraudulent or not for a credit card company.

A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.

The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.


Business Problem Overview:
Banking fraud, in todays world poses a significant threat to this goal for different banks. In terms of substantial financial losses, trust and credibility, this is a concerning issue to both banks and customers alike and difficult for banks to retain genuine customers.It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. 

In the banking industry, credit card fraud detection using machine learning is not just a trend but a necessity for them to put proactive monitoring and fraud prevention mechanisms in place. Machine learning is helping these institutions to reduce time-consuming manual reviews, costly chargebacks and fees, and denials of legitimate transactions.

Understanding and Defining Fraud :
Trust and credibility, is a concerning issue to both banks and customers alike and difficult for banks to retain genuine customers.It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.  Apart from this, the other ways are:
• Manipulation/alteration of genuine cards
• Creation of counterfeit cards
• Stolen/lost credit cards
• Fraudulent telemarketing

Data Understanding:
This dataset presents transactions that occurred in two days, Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with Principal Component Analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in others.

Project Pipeline:
The project pipeline can be briefly summarized in the following four steps:
• Data Understanding: Here, you need to load the data and understand the features present in it. This would help you choose the features that you will need for your final model.
• Exploratory data analytics (EDA): Normally, in this step, you need to perform univariate and bivariate analyses of the data,handle missing values, outliers if any followed by feature transformations, if necessary. For the current data set, feature scaling would be performed on Amount & time feature. You can check for any skewness in the data and try to mitigate it, as it might cause problems during the model-building phase.
• Train/Test Split: Now you are familiar with the train/test split, which you can perform in order to check the performance of your models with unseen data. Here, for validation, you can use the k-fold cross-validation techniques such as kfold, repeatedkfold, stratifiedkfold use gridsearchcv to find the best optimal hyperparameter. You need to choose an appropriate k value so that the minority class is correctly represented in the test folds.
• Model-Building/Hyperparameter Tuning: This is the final step at which you can try different models and fine-tune their hyperparameters until you get the desired level of performance on the given dataset. You should try and see if you get a better model by the various sampling techniques.
• Model Evaluation: Evaluate the model and its performance using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. Choose an appropriate evaluation metric which reflects this business goal. Use appropriate techniques to balance the data. and then check the models performance. Since it is binary classification we will perform Logistic Regression & other classification model building. 
