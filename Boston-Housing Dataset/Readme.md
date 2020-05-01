Boston Housing Dataset-Regression
---------------------------------------------------
    This project applies basic machine learning concepts on data collected for
    housing prices in the Boston, Massachusetts area to predict the selling price of a
    new home.

    In this we are going to use 3 Different Regression Model:
 * [Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
 * [Lasso Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Lasso.html)
 * [Random Forest Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)

![alt text](https://github.com/abhisngh/Regression-Boston-Dataset/blob/master/Images/boston_readme.jpg "Logo Title Text 1")

Boston house prices dataset
---------------------------

**Data Set Characteristics:**  

    :Number of Instances: 506

    :Number of Attributes: 13 numeric/categorical predictive. Median Value (attribute 14) is usually the target.

    :Attribute Information (in order):
        - CRIM     per capita crime rate by town
        - ZN       proportion of residential land zoned for lots over 25,000 sq.ft.
        - INDUS    proportion of non-retail business acres per town
        - CHAS     Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
        - NOX      nitric oxides concentration (parts per 10 million)
        - RM       average number of rooms per dwelling
        - AGE      proportion of owner-occupied units built prior to 1940
        - DIS      weighted distances to five Boston employment centres
        - RAD      index of accessibility to radial highways
        - TAX      full-value property-tax rate per $10,000
        - PTRATIO  pupil-teacher ratio by town
        - B        1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
        - LSTAT    % lower status of the population
        - MEDV     Median value of owner-occupied homes in $1000's

    :Missing Attribute Values: None

    :Creator: Harrison, D. and Rubinfeld, D.L.

    This is a copy of UCI ML housing dataset.
    https://archive.ics.uci.edu/ml/machine-learning-databases/housing/


    This dataset was taken from the StatLib library which is maintained at Carnegie Mellon University.

    The Boston house-price data of Harrison, D. and Rubinfeld, D.L. 'Hedonic
    prices and the demand for clean air', J. Environ. Economics & Management,
    vol.5, 81-102, 1978.   Used in Belsley, Kuh & Welsch, 'Regression diagnostics
    ...', Wiley, 1980.   N.B. Various transformations are used in the table on
    pages 244-261 of the latter.

    The Boston house-price data has been used in many machine learning papers that address regression
    problems.   

.. topic:: References

   - Belsley, Kuh & Welsch, 'Regression diagnostics: Identifying Influential Data and Sources of Collinearity', Wiley, 1980. 244-261.
   - Quinlan,R. (1993). Combining Instance-Based and Model-Based Learning. In Proceedings on the Tenth International Conference of Machine Learning, 236-243, University of Massachusetts, Amherst. Morgan Kaufmann.


Linear Regression
----------------------------
    Linear regression attempts to model the relationship between two variables by fitting a linear equation to observed data. One variable is considered to be an explanatory variable, and the other is considered to be a dependent variable.
    For example, a modeler might want to relate the weights of individuals to their heights using a linear regression model.
    Before attempting to fit a linear model to observed data, a modeler should first determine whether or not there is a relationship between the variables of interest. This does not necessarily imply that one variable causes the other (for example, higher SAT scores do not cause higher college grades), but that there is some significant association between the two variables.

Lasso Regression
------------------------
    LASSO stands for Least Absolute Shrinkage and Selection Operator. I know it doesn’t give much of an idea but there are 2 key words here – ‘absolute‘ and ‘selection‘.

    Lets consider the former first and worry about the latter later.

    Lasso regression performs L1 regularization, i.e. it adds a factor of sum of absolute value of coefficients in the optimization objective. Thus, lasso regression optimizes the following:

    Objective = RSS + α * (sum of absolute value of coefficients)
    Here, α (alpha) works similar to that of ridge and provides a trade-off between balancing RSS and magnitude of coefficients. Like that of ridge, α can take various values. Lets iterate it here briefly:

    α = 0: Same coefficients as simple linear regression
    α = ∞: All coefficients zero (same logic as before)
    0 < α < ∞: coefficients between 0 and that of simple linear regression

Random Forest Regressor
------------------------------
    A Random Forest is an ensemble technique capable of performing both regression and classification tasks with the use of multiple decision trees and a technique called Bootstrap Aggregation, commonly known as bagging.

    The basic idea behind this is to combine multiple decision trees in determining the final output rather than relying on individual decision trees. If you want to read more on Random Forests, I have included some reference links which provide in depth explanations on this topic.


STEPS INVOLVED
-------------------------------
  1. Go for Exploration_Template.ipynb for Analysis of the Dataset
  2. The implemented part is in Boston-Regression.ipynb, i.e solution.


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
* [Boston Housing Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_boston.html)
* [BSD License](https://github.com/scikit-learn/scikit-learn/blob/master/COPYING)

Contact
----------------------------------
 * [Boston-Regression](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_boston.html)
 * [Project_Link](https://github.com/decodrtechnologies/Data-Science)

Run
------------------------------
    To run this project you will need some software, like Anaconda, which provides
    support for running .ipynb files (Jupyter Notebook).

    After making sure you have that, you can run from a terminal or cmd next lines:
    ipython notebook Boston-Regression.ipynb
