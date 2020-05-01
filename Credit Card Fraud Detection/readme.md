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
![sampling](https://imgur.com/a/5n7sclj)
* **Random Over Sampling**
    
    In over sampling we make the instances of minority class equal to the majority class. Suppose out of  100 there are only 2 fraud cases. By over sampling  we make the instances of fraud cases from 2 to 100 by duplicating.
        
* **Random Down Sampling**

    In random down sampling we make the instances of majority class equal to minority class. In our previous example down sampling will result in 2 cases of frauds and 2 cases of non-frauds.

Each of these techniques possess challenges as well. If our dataset is very big then over sampling will make our dataset even bigger. And there will be time complexity as we are almost doubling the dataset and if we Down sample the minority classes we will miss the instances and specific patterns present in our dataset.

## Model Building Process 
     Load Data
     EDA
         Look for patterns in data
     DATA Preprocessing
         Standardize features
     Model Building
         Choosing right ML Algorithm
         Parameter tuning
         Set Threshold
     Model Evaluation
         roc_auc_score

## License 
https://opendatacommons.org/licenses/dbcl/1.0/

## Citations
[1] Andrea Dal Pozzolo, Olivier Caelen, Reid A. Johnson and Gianluca Bontempi. Calibrating Probability with Undersampling for Unbalanced Classification. In Symposium on Computational Intelligence and Data Mining (CIDM), IEEE, 2015

[2]Dal Pozzolo, Andrea; Caelen, Olivier; Le Borgne, Yann-Ael; Waterschoot, Serge; Bontempi, Gianluca. Learned lessons in credit card fraud detection from a practitioner perspective, Expert systems with applications,41,10,4915-4928,2014, Pergamon

[3]Dal Pozzolo, Andrea; Boracchi, Giacomo; Caelen, Olivier; Alippi, Cesare; Bontempi, Gianluca. Credit card fraud detection: a realistic modeling and a novel learning strategy, IEEE transactions on neural networks and learning systems,29,8,3784-3797,2018,IEEE

[4]Dal Pozzolo, Andrea Adaptive Machine learning for credit card fraud detection ULB MLG PhD thesis (supervised by G. Bontempi)

[5]Carcillo, Fabrizio; Dal Pozzolo, Andrea; Le Borgne, Yann-Aël; Caelen, Olivier; Mazzer, Yannis; Bontempi, Gianluca. Scarff: a scalable framework for streaming credit card fraud detection with Spark, Information fusion,41, 182-194,2018,Elsevier

[6]Carcillo, Fabrizio; Le Borgne, Yann-Aël; Caelen, Olivier; Bontempi, Gianluca. Streaming active learning strategies for real-life credit card fraud detection: assessment and visualization, International Journal of Data Science and Analytics, 5,4,285-300,2018,Springer International Publishing

[7]Bertrand Lebichot, Yann-Aël Le Borgne, Liyun He, Frederic Oblé, Gianluca Bontempi Deep-Learning Domain Adaptation Techniques for Credit Cards Fraud Detection, INNSBDDL 2019: Recent Advances in Big Data and Deep Learning, pp 78-88, 2019

[8]Fabrizio Carcillo, Yann-Aël Le Borgne, Olivier Caelen, Frederic Oblé, Gianluca Bontempi Combining Unsupervised and Supervised Learning in Credit Card Fraud Detection Information Sciences, 2019
