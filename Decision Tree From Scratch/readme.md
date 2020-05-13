## Decision Tree From Scratch

Decision tree is one of the predictive modelling approaches used in machine learning. It uses a decision tree (as a predictive model) to go from observations about an item (represented in the branches) to conclusions about the item's target value (represented in the leaves).

Decision Tree uses Entropy and Information Gain to construct a tree. 

**Entropy :** A decision tree is built top-down from a root node and involves partitioning the data into subsets that contain instances with similar values (homogeneous). CART uses entropy to calculate the homogeneity of a sample.

 Entropy is the measures of impurity, disorder or uncertainty in a bunch of examples.
 
**Till Now we have used scikit learn library to construct a decision tree. In this notebook we will build our own decision tree using Pandas and Nupmy library for iris species Classification.**

## License
This is an opensource dataset which can be found on UCI Repository.

  Citation

    @misc{Dua:2019 ,
    author = "Dua, Dheeru and Graff, Casey",<br>
    year = "2017",<br>
    title = "{UCI} Machine Learning Repository",<br>
    url = "http://archive.ics.uci.edu/ml",<br>
    institution = "University of California, Irvine, School of Information and Computer Sciences" }
