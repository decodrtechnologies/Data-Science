## Wine Dataset- Feature Selection

In this project we are performing the Feature Selection and Using RandomForest Classifier on the Wine Class Prediction Dataset in Sklearn.

![alt text](https://github.com/abhisngh/Feature-Selection-Wine-Dataset/blob/master/wine.jpg "Logo Title Text 1")

Wine dataset
---------------------------

**Data Set Characteristics:**

:Number of Instances: 178 (50 in each of three classes)

:Number of Attributes: 13 numeric, predictive attributes and the class

    :Attribute Information:

 		- 1) Alcohol

 		- 2) Malic acid

 		- 3) Ash

		- 4) Alcalinity of ash

 		- 5) Magnesium

		- 6) Total phenols

 		- 7) Flavanoids

 		- 8) Nonflavanoid phenols

 		- 9) Proanthocyanins

		- 10)Color intensity

 		- 11)Hue

 		- 12)OD280/OD315 of diluted wines

 		- 13)Proline

        	- class:
                - class_0
                - class_1
                - class_2

    :Summary Statistics:

    ============================= ==== ===== ======= =====
                                   Min   Max   Mean     SD
    ============================= ==== ===== ======= =====
    Alcohol:                      11.0  14.8    13.0   0.8
    Malic Acid:                   0.74  5.80    2.34  1.12
    Ash:                          1.36  3.23    2.36  0.27
    Alcalinity of Ash:            10.6  30.0    19.5   3.3
    Magnesium:                    70.0 162.0    99.7  14.3
    Total Phenols:                0.98  3.88    2.29  0.63
    Flavanoids:                   0.34  5.08    2.03  1.00
    Nonflavanoid Phenols:         0.13  0.66    0.36  0.12
    Proanthocyanins:              0.41  3.58    1.59  0.57
    Colour Intensity:              1.3  13.0     5.1   2.3
    Hue:                          0.48  1.71    0.96  0.23
    OD280/OD315 of diluted wines: 1.27  4.00    2.61  0.71
    Proline:                       278  1680     746   315
    ============================= ==== ===== ======= =====

    :Missing Attribute Values: None
    :Class Distribution: class_0 (59), class_1 (71), class_2 (48)
    :Creator: R.A. Fisher
    :Donor: Michael Marshall (MARSHALL%PLU@io.arc.nasa.gov)
    :Date: July, 1988

This is a copy of UCI ML Wine recognition datasets.
https://archive.ics.uci.edu/ml/machine-learning-databases/wine/wine.data

The data is the results of a chemical analysis of wines grown in the same
region in Italy by three different cultivators. There are thirteen different
measurements taken for different constituents found in the three types of
wine.

Original Owners:

Forina, M. et al, PARVUS -
An Extendible Package for Data Exploration, Classification and Correlation.
Institute of Pharmaceutical and Food Analysis and Technologies,
Via Brigata Salerno, 16147 Genoa, Italy.

Citation:

Lichman, M. (2013). UCI Machine Learning Repository
[http://archive.ics.uci.edu/ml]. Irvine, CA: University of California,
School of Information and Computer Science.



## Feature Selection
Feature selection and Data cleaning should be the first and most important step of your model designing.
Top reasons to use feature selection are:

 1. It enables the machine learning algorithm to train faster.
 2. It reduces the complexity of a model and makes it easier to interpret.
 3. It improves the accuracy of a model if the right subset is chosen.
 4. It reduces overfitting.

In this Project we have used the three techinques for Feature Selection, i.e
 * [KBest](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.SelectKBest.html)

  The SelectKBest class just scores the features using a function (in this case f_classif but could be others) and then "removes all but the k highest scoring features".

 * [ExtraTreeClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.ExtraTreesClassifier.html)

 Extremely Randomized Trees Classifier(Extra Trees Classifier) is a type of ensemble learning technique which aggregates the results of multiple de-correlated decision trees collected in a “forest” to output it’s classification result.

 * [Heat Map](https://seaborn.pydata.org/generated/seaborn.heatmap.html)

 A heatmap contains values representing various shades of the same colour for each value to be plotted. Usually the darker shades of the chart represent higher values than the lighter shade. For a very different value a completely different colour can also be used.
 

STEPS INVOLVED
-------------------------------
  1. Go for Exploration Template.ipynb for Analysis of the Dataset
  2. The implemented part is in Feature Selection.ipynb, i.e solution.


Install
-------------------------------
    Supported Python version
        -Python version used in this Project:3.5+

Libraries used
------------------------------
 * [Pandas](https://pandas.pydata.org/)
 * [Matplotlib](https://matplotlib.org/)
 * [Sklearn](https://scikit-learn.org/stable/)
 * [Numpy](https://numpy.org/)
 * [Seaborn](https://seaborn.pydata.org/)

License
--------------------------------
This is open Dataset, that can be found in UCI Repository

* [Wine Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_wine.html)
* [BSD License](https://github.com/scikit-learn/scikit-learn/blob/master/COPYING)

Run
------------------------------
    To run this project you will need some software, like Anaconda, which provides
    support for running .ipynb files (Jupyter Notebook).

    After making sure you have that, you can run from a terminal or cmd next lines:
    ipython notebook Feature Selection.ipynb
