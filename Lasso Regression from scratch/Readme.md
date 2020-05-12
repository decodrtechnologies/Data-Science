# Lasso Regression from scratch:

In this project we are going to implement Lasso Regression which is also known as L-2 Regression from scratch in python.

## What is Lasso Regression?

In statistics and machine learning, lasso (least absolute shrinkage and selection operator; also Lasso or LASSO) is a regression analysis method that performs both variable selection and regularization in order to enhance the prediction accuracy and interpretability of the statistical model it produces. It was originally introduced in geophysics literature in 1986, and later independently rediscovered and popularized in 1996 by Robert Tibshirani, who coined the term and provided further insights into the observed performance.

Lasso was originally formulated for least squares models and this simple case reveals a substantial amount about the behavior of the estimator, including its relationship to ridge regression and best subset selection and the connections between lasso coefficient estimates and so-called soft thresholding. It also reveals that (like standard linear regression) the coefficient estimates do not need to be unique if covariates are collinear.

Though originally defined for least squares, lasso regularization is easily extended to a wide variety of statistical models including generalized linear models, generalized estimating equations, proportional hazards models, and M-estimators, in a straightforward fashion. Lasso’s ability to perform subset selection relies on the form of the constraint and has a variety of interpretations including in terms of geometry, Bayesian statistics, and convex analysis.

<img src ="https://i.stack.imgur.com/HGfzU.png" height="800" width="800">
<br>src:https://i.stack.imgur.com/HGfzU.png</img>

## Libraries Used:

1. Numpy
2. Matplotlib

## Steps to be followed:

1. Importing the Libraries.
2. Defining number of observations and dimensions.
3. Visualizing input and output.
4. Finding weights.
5. Visualizing maximum likelihood function.
6. Defining L-2 Coefficients.
7. MAP v/s maximum likelihood.
