# HVAC Occupancy Detection:
In this project, you will be using a dataset for predicting room occupancy with using environmental observations such as temperature, humidity and CO2 level. This is an experimental dataset, these predictions might help Heating, Ventilating and Air Conditioning (HVAC) sector. For instance, we are using sensors like thermostats to get information about the environment and with that info our system decides to heat or not situation. But if the thermostat set manually by a occupant before and there is no more occupants in the environment, what then? The system won't shutdown until it gets set values, and this situation will lead high energy consumption.

# Problem Description:
Our aim is to detect the occupancy of a person in a room using the given environmental factors. For this we are going to implement 2-3 models on this dataset and compare thier performances. We will use k-Nearest neighbours and SVM as our machine learning models and then compare their performance with a Neural Network inplementation of this dataset.
This will be done with the help of certain features of the given dataset.
You can download the dataset from the provide link.
https://archive.ics.uci.edu/ml/machine-learning-databases/00357/

# Background of the Dataset:

Three data sets are submitted, for training and testing. Ground-truth occupancy was obtained from time stamped pictures that were taken every minute.
For the journal publication, the processing R scripts can be found in:
https://github.com/LuisM78/Occupancy-detection-data

# Relevant Papers:
Accurate occupancy detection of an office room from light, temperature, humidity and CO2 measurements using statistical learning models. Luis M. Candanedo, VÃ©ronique Feldheim. Energy and Buildings. Volume 112, 15 January 2016, Pages 28-39.


# Algorithm Used:

## k-Nearest Neighbours:

KNN can be used for both classification and regression predictive problems. However, it is more widely used in classification problems in the industry.
Model comparison KNN algorithm fairs across all parameters of considerations. It is commonly used for its easy of interpretation and low calculation time.
K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases based on a similarity measure (e.g., distance functions).

## SVM (Support Vector Machine):

A support vector machine (SVM) is a supervised machine learning model that uses classification algorithms for two-group classification problems. After giving an SVM model sets of labeled training data for each  category, they’re able to categorize new text.

## Neural Networks:

A neural network is a series of algorithms that endeavors to recognize underlying relationships in a set of data through a process that mimics the way the human brain operates. In this sense, neural networks refer to systems of neurons, either organic or artificial in nature. Neural networks can adapt to changing input; so the network generates the best possible result without needing to redesign the output criteria. The concept of neural networks, which has its roots in artificial intelligence, is swiftly gaining popularity in the development of trading systems.

A neural network works similarly to the human brain’s neural network. A “neuron” in a neural network is a mathematical function that collects and classifies information according to a specific architecture. The network bears a strong resemblance to statistical methods such as curve fitting and regression analysis.

A neural network contains layers of interconnected nodes. Each node is a perceptron and is similar to a multiple linear regression. The perceptron feeds the signal produced by a multiple linear regression into an activation function that may be nonlinear.

# Libraries Used:

* Numpy
* Pandas
* Sklearn
* Matplotlib
* Seaborn
* Plotly
* Keras

# Steps Involved:

1. Introduction
2. Importing Libraries
3. Exploring the Dataset
3. Exploratory Data Analysis
> * Uni-variate Analysis
> * Multi-variate Analysis
4. Data Preprocessing
5. Model Implementation
> * K-Nearest Neighbours
> * SUpport Vector Machine
6. Classification with Neural Networks
7. Comparing Performances of SVM and Neural Network
8. Conclusion

# License:

This is an opensource dataset which can be found on UCI Repository.

Citation

Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

@misc{Dua:2019 , author = "Dua, Dheeru and Graff, Casey",
year = "2017",
title = "{UCI} Machine Learning Repository",
url = "http://archive.ics.uci.edu/ml",
institution = "University of California, Irvine, School of Information and Computer Sciences" }


