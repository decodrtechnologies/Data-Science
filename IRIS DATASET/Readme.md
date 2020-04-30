# Iris Dataset

In this project we are going to classify different species of iris flower by using features such as sepal length,sepal width,petal length,petal width.

## License:-

The license for the above used dataset is given in the below link:-
https://creativecommons.org/publicdomain/zero/1.0/

## Dataset Information:-

The dataset has been taken from: https://www.kaggle.com/uciml/iris

The Iris dataset was used in R.A. Fisher's classic 1936 paper, The Use of Multiple Measurements in Taxonomic Problems, and can also be found on the UCI Machine Learning Repository.

It includes three iris species with 50 samples each as well as some properties about each flower. One flower species is linearly separable from the other two, but the other two are not linearly separable from each other.

## Attribute Information:-

The columns in this dataset are:

1. Id
2. SepalLength (Cm)
3. SepalWidth (Cm)
4. PetalLength (Cm)
5. PetalWidth (Cm)
6. Species

Predicted attribute: class of iris plant

## Libraries Used:-

1. Numpy
2. Matplotlib
3. Seaborn
4. Pandas
5. Sklearn

## Classification Algorithm Used:-

AdaBoost, short for Adaptive Boosting, is a machine learning meta-algorithm formulated by Yoav Freund and Robert Schapire, who won the 2003 Gödel Prize for their work. It can be used in conjunction with many other types of learning algorithms to improve performance. The output of the other learning algorithms ('weak learners') is combined into a weighted sum that represents the final output of the boosted classifier. AdaBoost is adaptive in the sense that subsequent weak learners are tweaked in favor of those instances misclassified by previous classifiers. AdaBoost is sensitive to noisy data and outliers. In some problems it can be less susceptible to the overfitting problem than other learning algorithms. The individual learners can be weak, but as long as the performance of each one is slightly better than random guessing, the final model can be proven to converge to a strong learner.

Every learning algorithm tends to suit some problem types better than others, and typically has many different parameters and configurations to adjust before it achieves optimal performance on a dataset, AdaBoost (with decision trees as the weak learners) is often referred to as the best out-of-the-box classifier. When used with decision tree learning, information gathered at each stage of the AdaBoost algorithm about the relative 'hardness' of each training sample is fed into the tree growing algorithm such that later trees tend to focus on harder-to-classify examples.

We have used Decision Tree Classifier and Support Vector Classifier as base estimators while implementing AdaBoost Algorithm.
