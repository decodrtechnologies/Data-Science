# Chi-Square-Feature-Selection

## Feature Selection
Feature selection is a process where you automatically select those features in your data that contribute most to the prediction variable or output in which you are interested. The benefits of performing feature selection before modeling your data are:

* Avoid Overfitting: Less redundant data gives performance boost to the model and results in less opportunity to make decisions based on noise
* Reduces Training Time: Less data means that algorithms train faster

## Chisquare for feature Selection:
One common feature selection method that is used with text data is the Chi-Square feature selection. The χ2 test is used in statistics to test the independence of two events. More specifically in feature selection we use it to test whether the occurrence of a specific term and the occurrence of a specific class are independent. More formally, given a document D, we estimate the following quantity for each term and rank them by their score:

For each feature (term), a corresponding high χ2 score indicates that the null hypothesis H0 of independence (meaning the document class has no influence over the term's frequency) should be rejected and the occurrence of the term and class are dependent. In this case, we should select the feature for the text classification.


## STEPS¶

- First compute the observed count for each class. This is done by building a contingency table from an input X (feature values) and y (class labels).

- Each entry i, j corresponds to some feature i and some class j, and holds the sum of the ith feature's values across all samples belonging to the class j.

- Note that although the feature values here are represented as frequencies, this method also works quite well in practice when the values are tf-idf values, since those are just weighted/scaled frequencies.

<br>

## Libraries Required:
- Sklearn 
- pandas
- numpy
- scipy

## Data:
The template notebook contains the dummy data for practicing out the chisquare test feature selection.
