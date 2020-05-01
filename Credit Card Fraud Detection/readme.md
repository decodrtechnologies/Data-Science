## Credit Card Fraud Detection

## Problem Statement
Given the transaction history of credit cards we have to predict the transactions as fraudulent or non-fraudulent. 

## Background
Suppose one day you wake up and recieve a message on your text that some amount has been deducted from your card for some purchase of say item 'x'. But you didn't made any purchase from your card, someone with your card cardentials or by any anhyhow has made a purchase through your card.It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. The banks fraud detection system saves you from these kind of fraudulent activities.

## Data Definition
[Data Source](https://www.kaggle.com/mlg-ulb/creditcardfraud)
* The datasets contains transactions made by credit cards in September 2013 by european cardholders.
* This dataset contains 284,807 records and 31 features.  
* Features V1, V2, … V28 are the principal components obtained with PCA. 
* The only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time'.
* Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## Handling Imbalanced Class
To handle class imbalance mostly used techniques are -
![Sampling](https://drive.google.com/open?id=1AUKOGnUrBPkd7gKhSj-I3yPW7SDmljm5)
* **Random Over Sampling**
    
    In over sampling we make the instances of minority class equal to the majority class. Suppose out of  100 there are only 2 fraud cases. By over sampling  we make the instances of fraud cases from 2 to 100 by duplicating.
    
* **Random Down Sampling**

    In random down sampling we make the instances of majority class equal to minority class. In our previous example down sampling will result in 2 cases of frauds and 2 cases of non-frauds.

Each of these techniques possess challenges as well. If our dataset is very big then **over sampling will make our dataset even bigger. And there will be time complexity as we are almost doubling the dataset and if we Down sample the minority classes we will miss the instances and specific patterns present in our dataset.**
