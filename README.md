# Credit-Risk-Classification

An overview of the analysis: The purpose of this analysis is to create a model that can predict the creditworthiness of borrowers. Our dataset consists of historical lending activity from a peer-to-peer lending services company that contains features in the dataset like the size of each loan, the interest rate, the income of each borrower, debt to income ratio of each borrower, the number of accounts each borrower has, derogatory marks, and total debt. The loan status is also included in the data set and this is what we want to predict using the features just noted. By splitting our data set we are able to use some of the data as "training" data for our model to learn from. After training the model, we will use the rest of the data set to test how well our model can predict the status of the loan versus the actual loan status. For this analysis we will be using a Linear Regression model.

The results:  
- accuracy score: The model scored an accuracy score of 99% with the testing data. As such, this model did a great job predicting the loan status given all the other features of the borrower and a loan's details.
- precision score: The model scored a precision score of 87% when predicting high-risk loans and 100% when predicting loans in good standing. This is a pretty good score, however, there is room for improvement for predicting the true positive outcomes for high-risk loans. It may be due to the limited amount of high-risk loans in our training dataset for the model to learn from.
- recall score: The model scored a recall score of 89% when predicting high risk loans and 100% for healthy loans. The recall measures the amount of false negatives. In this case, the model does basically a perfect job in not falsely categorizing healthy loans. However, there is a very minor chance of falsely categorizing a high-risked laon as healthy. For this use case, we would rather have it inversed, as we would rather categorize a loan as high risk and it be healthy versus we think it will be healthy and it is high risk. Again, it may be due to the limited amount of high-risk loans in our training dataset for the model to learn from.

A summary: Overall, this model is a pretty good model. There is room for improvement when predicting if a loan is high-risk. As mentioned, we would rather categorize a loan as high risk and it be healthy versus we think it will be healthy and it is high risk. As such, I would suggest a company train the model with more high-risk loans within the training data before using this model.
