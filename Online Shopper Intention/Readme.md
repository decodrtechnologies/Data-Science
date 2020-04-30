# Online Shopper's Intention:
In this project, you'll build your first Online Shopper Intention Model using Random Forest Classifier
and use it to predict whether a customer will purchase something or not.
Is is a type of classification problem.

# Problem Description:
Our aim is to create a model that can classify Customer Shopping instance  as 'successful' or 'not sucessful', 
based on the training we give to the model. This will be done with the help of certain features of the given dataset.
You can download the dataset from the provide link.
https://archive.ics.uci.edu/ml/machine-learning-databases/00468/

# Background of the Dataset:

Source
1. C. Okan Sakar
Department of Computer Engineering, Faculty of
Engineering and Natural Sciences, Bahcesehir University,
34349 Besiktas, Istanbul, Turkey

2. Yomi Kastro
Inveon Information Technologies Consultancy and Trade,
34335 Istanbul, Turkey

The dataset consists of feature vectors belonging to 12,330 sessions.
The dataset was formed so that each session
would belong to a different user in a 1-year period to avoid
any tendency to a specific campaign, special day, user
profile, or period.

# Knowing your Dataset:
* The dataset consists of 10 numerical and 8 categorical attributes.
* The 'Revenue' attribute can be used as the class label.
* "Administrative", "Administrative Duration", "Informational", "Informational Duration", "Product Related"
and "Product Related Duration" represent the number of different types of pages visited by the visitor in 
that session and total time spent in each of these page categories.
* The values of these features are derived from the URL information of the pages visited by the user and updated
in real time when a user takes an action, e.g. moving from one page to another.
* The "Bounce Rate", "Exit Rate" and "Page Value" features represent the metrics measured by
"Google Analytics" for each page in the e-commerce site.
* The value of "Bounce Rate" feature for a web page refers to the percentage of visitors who enter the site from that page
and then leave ("bounce") without triggering any other requests to the analytics server during that session.
* The value of "Exit Rate" feature for a specific web page is calculated as for all pageviews to the page, the percentage
that were the last in the session.
* The "Page Value" feature represents the average value for a web page that a user visited before completing an e-commerce transaction.
* The "Special Day" feature indicates the closeness of the site visiting time to a specific special day
(e.g. Mother’s Day, Valentine's Day) in which the sessions are more likely to be finalized with transaction.
The value of this attribute is determined by considering the dynamics of e-commerce such as the duration between
the order date and delivery date. For example, for Valentina’s day, this value takes a nonzero value between February 2
and February 12, zero before and after this date unless it is close to another special day, and its maximum value of 1 on February 8.
* The dataset also includes operating system, browser, region, traffic type, visitor type as returning or new visitor
, a Boolean value indicating whether the date of the visit is weekend, and month of the year.

# Algorithm Used:

## Random Forest Classifier

* Random Forest Classifier is an ensemble algorithm. Ensembled algorithms are those which combines more than one
algorithms of same or different kind for classifying objects. For example,
running prediction over Naive Bayes, SVM and Decision Tree and then taking vote for final consideration of class for test object.
* This works well because a single decision tree may be prone to a noise, 
but aggregate of many decision trees reduce the effect of noise giving more accurate results.

# Libraries Used:

* Numpy
* Pandas
* Sklearn
* Matplotlib
* Seaborn
* Dabl
* Shap

# Steps Involved:
1. Importing Libraries
2. Exploring the Dataset
3. Exploratory Data Analysis
> * Univariate Analysis
> * Bi-variate Analysis
> * Multi-variate Analysis
4. Data Preprocessing
5. Model Building
> * Random Forest Classifier
6. Hyperparameters Tuning
> * Random Search
7. Conclusion

# License:

This is an opensource dataset which can be found on UCI Repository.

**Citation**

Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

@misc{Dua:2019 ,
author = "Dua, Dheeru and Graff, Casey",<br>
year = "2017",<br>
title = "{UCI} Machine Learning Repository",<br>
url = "http://archive.ics.uci.edu/ml",<br>
institution = "University of California, Irvine, School of Information and Computer Sciences" }
