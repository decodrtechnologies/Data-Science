# CREATE CUSTOMER SEGMENTATION ON WHOLESALE DATASET

In this project we will be using unsupervised approach to segment the customers.

## PROBLEM STATEMENT: 

Our aim here is to build a model that can segment the customer based on model training and dataset available.

### DATA

We will be using a [Wholesale customers dataset](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers#) 
from the [UCI Machine learning repository](https://archive.ics.uci.edu/ml/index.php) which has a very good collection of datasets.

Features used in this project:
- FRESH
- MILK
- GROCERY
- FROZEN
- DETERGENTS_PAPER
- DELICATESSEN

**Source:**

Margarida G. M. S. Cardoso, margarida.cardoso '@' iscte.pt, ISCTE-IUL, Lisbon, Portugal

### LICENSE : 
This is an opensource dataset which can be found on UCI Repository.

Citation :
Abreu, N. (2011). Analise do perfil do cliente Recheio e desenvolvimento de um sistema promocional. Mestrado em Marketing, ISCTE-IUL, Lisbon

Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

@misc{Dua:2019 ,
author = "Dua, Dheeru and Graff, Casey",
year = "2017",
title = "{UCI} Machine Learning Repository",
url = "http://archive.ics.uci.edu/ml",
institution = "University of California, Irvine, School of Information and Computer Sciences" }


### Requirements

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. 

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [Matplotlib](http://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [Scikit-learn](http://scikit-learn.org/)

### Run

In a terminal or command window, navigate to the top-level project directory `Wholesale Customer segmentation/`
(that contains this README) and run one of the following commands:


ipython notebook Wholesale Customer segmentation_task.ipynb

or

jupyter notebook Wholesale Customer segmentation_task.ipynb


This will open the Jupyter Notebook software and project file in your browser.

### STEPS :
1. Importing Libraries
2. Exploring the Dataset
3. Exploratory Data Analysis
> * Univariate analysis
> * Multivariate analysis
4. Data Preprocessing
> * Feature scaling
> * Outlier detection
5. Feature Transformation
> * PCA
6. Model Building : Clustering 
> * Gaussian Mixture model
7. Conclusion

