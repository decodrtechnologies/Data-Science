# MLP Implementation from scratch:
In this project we are going to implement Multi-Layer Perceptron Neural Network from scratch to classify different species of iris flower by using features such as sepal length,sepal width,petal length,petal width. We will be doing forward propagation, backward propagation, weight initialization, gradient descent from scratch.

# Problem Description:
Our aim is to classify different species of iris flower by using features such as sepal length,sepal width,petal length,petal width.
This will be done with the help of certain features of the given dataset.
You can download the dataset from the provide link.
https://archive.ics.uci.edu/ml/machine-learning-databases/iris/

# Background of the Dataset:

The Iris dataset was used in R.A. Fisher's classic 1936 paper, The Use of Multiple Measurements in Taxonomic Problems, and can also be found on the UCI Machine Learning Repository.

It includes three iris species with 50 samples each as well as some properties about each flower. One flower species is linearly separable from the other two, but the other two are not linearly separable from each other.

# Attributes of Dataset:

The columns in this dataset are:

1. SepalLength (Cm)
2. SepalWidth (Cm)
3. PetalLength (Cm)
4. PetalWidth (Cm)
5. Species
Predicted attribute: class of iris plant

# Relevant Papers:
Fisher,R.A. "The use of multiple measurements in taxonomic problems" Annual Eugenics, 7, Part II, 179-188 (1936); also in "Contributions to Mathematical Statistics" (John Wiley, NY, 1950).
[http://rexa.info/paper/2fb499aa4d6a7071a6ba53c679ccca7055813114]

Duda,R.O., & Hart,P.E. (1973) Pattern Classification and Scene Analysis. (Q327.D83) John Wiley & Sons. ISBN 0-471-22361-1. See page 218.
[http://rexa.info/paper/e6b7a3a8c46efef785a6ab735be07dafa0713ff3]

Dasarathy, B.V. (1980) "Nosing Around the Neighborhood: A New System Structure and Classification Rule for Recognition in Partially Exposed Environments". IEEE Transactions on Pattern Analysis and Machine Intelligence, Vol. PAMI-2, No. 1, 67-71.
[http://rexa.info/paper/acf9d77f6470a326f784fd50b08b7dd60be5fb9a]

Gates, G.W. (1972) "The Reduced Nearest Neighbor Rule". IEEE Transactions on Information Theory, May 1972, 431-433.
[http://rexa.info/paper/876f54b2ebfecb6a796590237abf245cf28d3c74]

See also: 1988 MLC Proceedings, 54-64.



# Algorithm and Functions Used:

## Multi Layer Perceptron:

A multilayer perceptron (MLP) is a class of feedforward artificial neural network (ANN). ... MLP utilizes a supervised learning technique called backpropagation for training. Its multiple layers and non-linear activation distinguish MLP from a linear perceptron. It can distinguish data that is not linearly separable.

Multilayer perceptrons are often applied to supervised learning problems: they train on a set of input-output pairs and learn to model the correlation (or dependencies) between those inputs and outputs. Training involves adjusting the parameters, or the weights and biases, of the model in order to minimize error. Backpropagation is used to make those weigh and bias adjustments relative to the error, and the error itself can be measured in a variety of ways, including by root mean squared error (RMSE).

![Image description](https://pathmind.com/images/wiki/perceptron_formula.png)

## Relu Activation Function:

In a neural network, the activation function is responsible for transforming the summed weighted input from the node into the activation of the node or output for that input.

The rectified linear activation function is a piecewise linear function that will output the input directly if is positive, otherwise, it will output zero. It has become the default activation function for many types of neural networks because a model that uses it is easier to train and often achieves better performance.
In order to use stochastic gradient descent with backpropagation of errors to train deep neural networks, an activation function is needed that looks and acts like a linear function, but is, in fact, a nonlinear function allowing complex relationships in the data to be learned.

The function must also provide more sensitivity to the activation sum input and avoid easy saturation.
![](https://miro.medium.com/max/1400/1*XxxiA0jJvPrHEJHD4z893g.png)


## Softmax Function:

Softmax is an activation function which converts its inputs – likely the logits, a.k.a. the outputs of the last layer of your neural network when no activation function is applied yet – into a discrete probability distribution over the target classes. Softmax ensures that the criteria of probability distributions – being that probabilities are nonnegative realvalued numbers and that the sum of probabilities equals 1 – are satisfied. This is great, as we can now create models that learn to maximize logit outputs for inputs that belong to a particular class, and by consequence also maximize the probability distribution. Simply taking argmax then allows us to pick the class prediction, e.g. showing it on-screen in object detectors, image classifiers and text classifiers.

The Softmax function allows us to express our inputs as a discrete probability distribution. Mathematically, this is defined as follows:
Intuitively, this can be defined as follows: for each value (i.e. input) in our input vector, the Softmax value is the exponent of the individual input divided by a sum of the exponents of all the inputs.

## Forward Propagation:

The neural network will feed forward the input data. The data will be computed at each layer using f(x) = wx + b function as w = weight values, x is input values, and b is the bias of the layer. Then after that value is calculated at each layer, it will be put through the layer's associated activation function to keep moving forward through the neural network.
The input X provides the initial information that then propagates to the hidden units at each layer and finally produce the output y^. The architecture of the network entails determining its depth, width, and activation functions used on each layer. Depth is the number of hidden layers. Width is the number of units (nodes) on each hidden layer since we don’t control neither input layer nor output layer dimensions. There are quite a few set of activation functions such Rectified Linear Unit, Sigmoid, Hyperbolic tangent, etc. Research has proven that deeper networks outperform networks with more hidden units. Therefore, it’s always better and won’t hurt to train a deeper network (with diminishing returns).

## Backward Propagation:

This is the step of the process where the neural network learns, as it identifies the error of the output nodes. This establishes a loss value and a gradient or slope for that value at each node. When the data is fed back through the network, each value goes through gradient descent where the local minimum of its specific gradient is calculated so that it can adjust new values to the parameters of the neural networks to minimize loss the next time data is fed through the network.
It Allows the information to go back from the cost backward through the network in order to compute the gradient. Therefore, loop over the nodes starting at the final node in reverse topological order to compute the derivative of the final node output with respect to each edge’s node tail. Doing so will help us know who is responsible for the most error and change the parameters in that direction.

# Libraries Used:

* Numpy
* Pandas
* Sklearn
* Matplotlib
* Seaborn

# Steps Involved:

1. Importing Libraries
2. Reading the Dataset
3. Exploratory Data Analysis
> * Uni-variate Analysis
> * Bi-variate Analysis
> * Multi-variate Analysis
4. Data Preprocessing
5. Functions for the neural network
6. Training our Model
7. Testing our Model
8. Conclusion

# License:

This is an opensource dataset which can be found on UCI Repository.

Citation

Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

@misc{Dua:2019 , author = "Dua, Dheeru and Graff, Casey",
year = "2017",
title = "{UCI} Machine Learning Repository",
url = "http://archive.ics.uci.edu/ml",
institution = "University of California, Irvine, School of Information and Computer Sciences" }


