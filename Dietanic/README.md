# Titanic Survivors Prediction


The sinking of the RMS Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This sensational tragedy shocked the international community and led to better safety regulations for ships.

One of the reasons that the shipwreck led to such loss of life was that there were not enough lifeboats for the passengers and crew. Although there was some element of luck involved in surviving the sinking, some groups of people were more likely to survive than others, such as women, children, and the upper-class.

# The Data:


There are two datasets namely 'test' and 'train' which are totally open source available on kaggle. The training set has 891 rows and 12 columns whereas the test set contains 418 rows and 11 columns. We have appended the 'test' at the end of 'train' dataset and stored it into a new data frame called 'data'.

# Libraries used:


1. Pandas
2. Matplotlib
3. Seaborn
4. Numpy

# Handling Missing Data:

There were many missing values which had to be filled according to the requirements. The 'Cabin', 'Name', 'Ticket' columns were dropped as they did not contribute to the model building.

# Feature Engineering:


Feature engineering is the process of transforming raw data into features that better represent the underlying problem to the predictive models, resulting in improved model accuracy on unseen data. Feature engineering turn your inputs into things the algorithm can understand.
We created features like **family size**, **age group**, **family group**, **fare per person**, **fare group**. The creation of new features made us understand the dataset better.

# Models Implemented:

## We have implemented 6 Machine Learning models-


1. RandomForest
2. LinearSVC
3. Gaussian Naive Bayes
4. K-Neighbors
5. DecisionTree
6. Logistic Regression

# This Notebook will show basic examples of:


- Data Handling
- Importing Data with Pandas
- Cleaning Data
- Exploring Data through Visualizations with Matplotlib
- Building Machine Learning Models

# Cross Validation:

## K-Fold Cross Validation:

Cross-validation is a resampling procedure used to evaluate machine learning models on a limited data sample. The procedure has a single parameter called k that refers to the number of groups that a given data sample is to be split into.

# Observations:


1. We were able to conclude that women and children had a better chance of survival as compared to men.
2. The passengers who paid more amount of money as the fare were able to survive as they were at a higher deck.
3. Overall only 38% of the passengers could survive the tragic disaster.
4. The age played a major role as we could infer that children were indeed the most likely age group to survive, although this      percentage was still tragically below 60%.


# Output:

After identifying the important features which actually predcited the survival of a passenger, we were able to predict the survival of the test dataset using the **RandomForest Algorithm** with a very good score. 
The output of the code is to **predict the survival(0-Die,1-Survive)** of the passenger who boarded the Titanic.


