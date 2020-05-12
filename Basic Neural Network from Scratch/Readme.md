# Basic Neural Network from Scratch : 

A Basic neural network having one hidden layer is implemented by building model , predict and loss functions. Plot decision boundary function has already been built to show the decision boundaries in plots. The dataset is created through scikitlearn's inbuilt function and the input and output terms are taken from it. 

## Objective : 

To understand and build a basic one hidden layer Neutral Network from scratch. 

## Neural Network : 

The input `X` has two attributes `X1` and `X2` , the input is passed through one hidden layer with Tanh activation function and then to the output node with softmax activation to give out the probabilities. Cross entropy loss function works well with softmax activation and thus is used here. 

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQediZV_J9oWckQU6SMM1bwIJUF05pYb3QJQQhJ3t3YoFcax5Ve&usqp=CAU">

Further , Neural networks with varying number of nodes in the hidden layer and simple logistic regression are plotted to properly assess and choose the best model.

Neural Networks are thoroughly explained from the basic structure to in depth calculus working behind it in an organised procedure as follows : 

       - Neural Network structure
       - Activation functions : Softmax and Tanh and their necessity 
       - Weight factors and Bias 
       - Forward Propagation
       - Back Propagation
       - Shape of Vectors
       - Differentiation

The structure can be shown as : 

<img src="https://i.stack.imgur.com/iHDtO.png">

## Function Building : 

Following functions are built to implement the neural network properly : 

- **Model Function** : Gives out the updated optimum weight factors and bias after gradient descent after a series of forward and back propagation

- **Predict Function** : Predicts the models output using weight factors and bias of the model function

- **Loss Function** : Calculates the cross entropy loss between the predicted values from above function and the actual values

## Conclusion : 

All the models are analysed and the best model is chosen. 

## Acknowledgements :

Following notebooks and articles have been used for references and are cited :

1. [Implementing a Neural Network from Scratch in Python – An Introduction](http://www.wildml.com/2015/09/implementing-a-neural-network-from-scratch/) by Denny Britz
2. [Classification and Loss Evaluation - Softmax and Cross Entropy Loss](https://deepnotes.io/softmax-crossentropy)
3. [The Softmax function and its derivative](https://eli.thegreenplace.net/2016/the-softmax-function-and-its-derivative/)
4. [Understanding softmax and the negative log-likelihood](https://ljvmiranda921.github.io/notebook/2017/08/13/softmax-and-the-negative-log-likelihood/) by LJ Miranda


