# RANDOM FOREST

*Random forest builds multiple decision trees and merges them together to get a more accurate and stable prediction.*

One big advantage of random forest is that it can be used for both **classification** and **regression problems**, which form the majority of current machine learning systems.

Random forest adds additional randomness to the model, while growing the trees. Instead of searching for the most important feature while splitting a node, it searches for the best feature among a random subset of features. This results in a wide diversity that generally results in a better model.

Therefore, in random forest, only a random subset of the features is taken into consideration by the algorithm for splitting a node. You can even make trees more random by additionally using random thresholds for each feature rather than searching for the best possible thresholds (like a normal decision tree does).

**WHY RANDOM FOREST ?**
- The same random forest algorithm or the random forest classifier can use for both classification and the regression task.
- Random forest classifier will handle the missing values.
- When we have more trees in the forest, random forest classifier won’t overfit the model.
- Can model the random forest classifier for categorical values also.

## PROBLEM STATEMENT: 

Our Aim  is to implement **RANDOM FOREST** from scratch

### PREREQUISITE : 

DECISION TREE ALGORITHM

- Refer the Code present in the [Decision_tree_functions](https://github.com/decodrtechnologies/Data-Science/blob/master/Random_Forest_from_scratch/decision_tree_functions.py) to know the implementation of Decision tree.
- Our focus in this Notebook is to implement Random forest using the knowledge of Decision tree.

### DATA
We will be using a [Red Wine quality](https://www.kaggle.com/uciml/red-wine-quality-cortez-et-al-2009) from the Kaggle platform which has a very good collection of datasets.
  
The data is presented in CSV format.

Features:
- fixed acidity
- volatile acidity
- citric acid
- residual sugar
- chlorides
- free sulfur dioxide
- total sulfur dioxide
- densitythe density 
- pHdescribes
- sulphatesa wine 
- alcohol
- quality (OUTPUT VARIABLE)
  
Note that prices have been adjusted for dividends and splits.

### LICENSE OF DATASET : [LICENSE](http://opendatacommons.org/licenses/dbcl/1.0/)

### Requirements

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. 

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)

Refer to this file for decision tree code :
- [Decision_tree_functions](https://github.com/decodrtechnologies/Data-Science/blob/master/Random_Forest_from_scratch/decision_tree_functions.py)

### Run

In a terminal or command window, navigate to the top-level project directory `Random_Forest_from_scratch/` (that contains this README) and run one of the following commands:


ipython notebook Random_Forest_from_scratch_task.ipynb

or

jupyter notebook Random_Forest_from_scratch_task.ipynb

This will open the Jupyter Notebook software and project file in your browser.

### Steps :
1. Importing Libraries
2. Exploring the Dataset
4. Data Preprocessing
5. Model Building
> * RANDOM FOREST MODEL
> * Size of Testing dataset : Size of Training dataset = 20 : 80
6. Evaluation
7. Conclusion

