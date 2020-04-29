# Mushroom Classification Dataset:

## Background:

A mushroom or toadstool is the fleshy, spore-bearing fruiting body of a fungus, typically produced above ground, on soil, or its food source. Mushroom hunting refers to the gathering mushrooms in the wild, especially for food. Mushroom hunting has gained popularity over the years. In this project, we'll be classifying mushrooms as edible or poisonous using the Mushroom Classification dataset available on Kaggle. 
 
## Dataset Description:

The dataset has 8124 entries with 23 columns. The dataset is obtained from [Kaggle](https://www.kaggle.com/uciml/mushroom-classification) which was originally contributed by [UCI Machine Learning repository](http://archive.ics.uci.edu/ml/datasets/Mushroom).

## Attribute Description:

class: edible(e) or poisonous(p)

cap-shape: bell(b), conical(c), convex(x), flat(f), knobbed(k), sunken(s)

cap-surface: fibrous(f), grooves(g), scaly(y), smooth(s)

cap-color: brown(n), buff(b), cinnamon(c), gray(g), green(r), pink(p), purple(u), red(e), white(w), yellow(y)

bruises: bruises(t), no bruises(f)

odor: almond(a), anise(l), creosote(c), fishy(y), foul(f), musty(m), none(n), pungent(p), spicy(s)

gill-attachment: attached(a), descending(d), free(f), notched(n)

gill-spacing: close(c), crowded(w), distant(d)

gill-size: broad(b), narrow(n)

gill-color: black(k), brown(n), buff(b), chocolate(h), gray(g), green(r), orange(o), pink(p), purple(u), red(e), white(w), yellow(y)

stalk-shape: enlarging(e), tapering(t)

stalk-root: bulbous(b), club(c), cup(u), equal(e), rhizomorphs(z), rooted(r), missing(?)

stalk-surface-above-ring: fibrous(f), scaly(y), silky(k), smooth(s)

stalk-surface-below-ring: fibrous(f), scaly(y), silky(k), smooth(s)

stalk-color-above-ring: brown(n), buff(b), cinnamon(c), gray(g), orange(o), pink(p), red(e), white(w), yellow(y)

stalk-color-below-ring: brown(n), buff(b), cinnamon(c), gray(g), orange(o), pink(p), red(e), white(w), yellow(y)

veil-type: partial(p), universal(u)

veil-color: brown(n), orange(o), white(w), yellow(y)

ring-number: none(n), one(o), two(t)

ring-type: cobwebby(c), evanescent(e), flaring(f), large(l), none(n), pendant(p), sheathing(s), zone(z)

spore-print-color: black(k), brown(n), buff(b), chocolate(h), green(r), orange(o), purple(u), white(w), yellow(y)

population: abundant(a), clustered(c), numerous(n), scattered(s), several(v), solitary(y)

habitat: grasses(g), leaves(l), meadows(m), paths(p), urban(u), waste(w), woods(d)

## Libraries Used:

Pandas
Matplotlib
Sklearn
Seaborn
Numpy

## Run:

The entire coding is done by using the jupyter notebook. It can be installed by following the steps given in this [link](https://jupyter.org/install). 

## Algorithm:

The dataset can be dealt with various models. Here I am using Logistic regression, Linear Discriminant Analysis, and Quadratic Discriminant Analysis to predict the data. 

### Logistic Regression:

Logistic regression is a statistical model that uses a logistic function to model a binary dependent variable, although many more complex extensions exist. In regression analysis, logistic regression (or logit regression) is estimating the parameters of a logistic model (a form of binary regression). Mathematically, a binary logistic model has a dependent variable with two possible values, such as pass/fail which is represented by an indicator variable, where the two values are labeled "0" and "1". In the logistic model, the log-odds (the logarithm of the odds) for the value labeled "1" is a linear combination of one or more independent variables ("predictors"). The independent variables can each be a binary variable (two classes, coded by an indicator variable) or a continuous variable (any real value). The corresponding probability of the value labeled "1" can vary between 0 (certainly the value "0") and 1 (certainly the value "1"). The logistic regression model takes real-valued inputs and predicts the probability of the input belonging to the default class (class 0). If the probability is greater than 0.5, then output is a prediction for the default class (class 0) otherwise, it's for the other class (class 1).

Advantages: It is a widely used technique because it is very efficient and does not require too many computational resources. It’s highly interpretable, doesn’t require input features to be scaled, and doesn't require any tuning. It’s easy to regularize and provides well-calibrated predicted probabilities.

Disadvantages: We can’t solve non-linear problems with logistic regression since it’s decision surface is linear. Logistic regression is not a useful tool unless you have already identified all the important independent variables.

### Linear and Quadratic Dimension Analysis:
The discriminant analysis includes methods that can be used for both classification and dimensionality reduction. Linear discriminant analysis (LDA) is particularly popular because it is both a classifier and a dimensionality reduction technique. Quadratic discriminant analysis (QDA) is a variant of LDA that allows for non-linear separation of data. 

## Tasks:

Here, we are learning to do
1. Importing the necessary libraries
2. Exploring the Dataset
3. Exploratory Data Analysis
4. Data Preprocessing
5. Building Models
6. Validation

### License:

Mushroom Classification dataset used in the problem is available open-source on Kaggle and the license is available at this [link](https://creativecommons.org/publicdomain/zero/1.0/).
