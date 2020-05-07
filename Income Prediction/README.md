# PCA for Logistic Regression

**Principal Component Analysis** is an important **dimensionality reduction technique** that can be used to reduce a larger set of feature variables into a smaller set that still contains most of the variance in the larger set.
## Problem Description : 

Our aim is to create a model that can predict whether a person's income exceeds $50K/yr based on census data. Also known as "Census Income" dataset.


## Understanding our Dataset :
We will be using a [Adult Data Set](https://archive.ics.uci.edu/ml/datasets/Adult) from the UCI Machine Learning repository which has a very good collection of datasets for experimental research purposes. The direct data link is [here](https://archive.ics.uci.edu/ml/machine-learning-databases/adult/).
Extraction was done by Barry Becker from the 1994 Census database.
  
  
### Dataset Source :

**Donor**
<br>
Ronny Kohavi and Barry Becker
<br>
Data Mining and Visualization
<br>
Silicon Graphics.
<br>
e-mail: ronnyk '@' live.com for questions.

## The Curse of Dimensionality :

Generally, real world datasets contain thousands or millions of features to train for. This is very time consuming task as this makes training extremely slow. In such cases, it is very difficult to find a good solution. This problem is often referred to as the curse of dimensionality.


**The curse of dimensionality** refers to various phenomena that arise when we analyze and organize data in high dimensional spaces (often with hundreds or thousands of dimensions) that do not occur in low-dimensional settings. The problem is that when the dimensionality increases, the volume of the space increases so fast that the available data become sparse. This sparsity is problematic for any method that requires statistical significance.


In real-world problems, it is often possible to reduce the number of dimensions considerably. This process is called **dimensionality reduction**. It refers to the process of reducing the number of dimensions under consideration by obtaining a set of principal variables. It helps to speed up training and is also extremely useful for data visualization.


The most popular dimensionality reduction technique is Principal Component Analysis (PCA), which is discussed below.

## Introduction to Principal Component Analysis (PCA) :


**Principal Component Analysis (PCA)** is a dimensionality reduction technique that can be used to reduce a larger set of feature variables into a smaller set that still contains most of the variance in the larger set. 

### Preserve the variance

PCA, first identifies the hyperplane that lies closest to the data and then it projects the data onto it. Before, we can project the training set onto a lower-dimensional hyperplane, we need to select the right hyperplane. The projection can be done in such a way so as to preserve the maximum variance. This is the idea behind PCA.

### Principal Components

PCA identifies the axes that accounts for the maximum amount of cumulative sum of variance in the training set. These are called Principal Components. PCA assumes that the dataset is centered around the origin. Scikit-Learn’s PCA classes take care of centering the data automatically.

### Projecting down to d Dimensions

Once, we have identified all the principal components, we can reduce the dimensionality of the dataset down to d dimensions by projecting it onto the hyperplane defined by the first d principal components. This ensures that the projection will preserve as much variance as possible.

## License :

This is an opensource dataset which can be found on UCI Repository.

**Citation**
<br>
Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

## **Now, let's get to the implementation!**
