# E Coli Dataset:

## Background:

E Coli Escherichia coli, also known as E. coli, is a Gram-negative, facultative anaerobic, rod-shaped, coliform bacterium of the genus Escherichia that is commonly found in the lower intestine of warm-blooded organisms.

In this project, we'll be observing the data available through the E Coli dataset available on Kaggle and predicting the sites where its available. 
 
## Dataset Description:

The dataset has 336 entries with 9 columns. The dataset is obtained from [Kaggle](https://www.kaggle.com/kannanaikkal/ecoli-uci-dataset) which was originally contributed by [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Ecoli).

## Attribute Description:

SEQUENCE_NAME - Accession number for the SWISS-PROT database

MCG -  McGeoch's method for signal sequence recognition.

GVH  - Von Heijne's method for signal sequence recognition.

LIP  - Von Heijne's Signal Peptidase II consensus sequence score. Binary attribute

CHG  - Presence of charge on N-terminus of predicted lipoproteins. Binary attribute

AAC  - Score of discriminant analysis of the amino acid content of outer membrane and periplasmic proteins.

ALM1 - Score of the ALOM membrane spanning region prediction program.

ALM2 - Score of ALOM program after excluding putative cleavable signal regions from the sequence

SITE - Its the class distribution. The class is the localization site. The parameters in the SITE are, 

  1. cp  (cytoplasm)                                   
  
  2. im  (inner membrane without signal sequence)                     
  
  3. pp  (perisplasm)                                    
  
  4. imU (inner membrane, uncleavable signal sequence)  
  
  5. om  (outer membrane)                               
  
  6. omL (outer membrane lipoprotein)                     
  
  7. imL (inner membrane lipoprotein)                     
  
  8. imS (inner membrane, cleavable signal sequence)      

## Libraries Used:

Pandas

Matplotlib

Sklearn

Seaborn

Numpy

## Run:

The entire coding is done by using the jupyter notebook. It can be installed by following the steps given in this [link](https://jupyter.org/install). 

## Algorithm:

The dataset can be dealt with various models. Here I am using the KNN Classifier and the and Support Vector Machine to predict the sites where its available and compare the analysis between both the alogorithms.  

### KNN Classifier:

K-nearest neighbor algorithm (K-NN) is a non-parametric method used for classification and regression. In both cases, the input consists of the k closest training examples in the feature space. The output depends on whether K-NN is used for classification or regression. 

### Support Vector Machine: 

Support-vector machines (SVMs, also support vector networks) are supervised learning models with associated learning algorithms that analyze data used for classification and regression analysis. Given a set of training examples, each marked as belonging to one or the other of two categories, an SVM training algorithm builds a model that assigns new examples to one category or the other, making it a non-probabilistic binary linear classifier (although methods such as Platt scaling exist to use SVM in a probabilistic classification setting).


## Tasks:

Here, we are learning to do

Data Handling

Importing Data with Pandas

Cleaning Data

Exploring Data through Visualizations with Matplotlib

Building Machine Learning Models

Validation

## License:

The E Coli dataset used in the problem is available open-source on Kaggle and the license is obtained from UCI Machine Learning Repository available at this [link](https://archive.ics.uci.edu/ml/citation_policy.html).
