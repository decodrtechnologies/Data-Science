CIFAR 10 using Convolutional Neural Networks
---------------------------------------------------
  In this Project we are going to use CNNs to predict classes of various images.
  Main objective is to classify images for 10 different classes.
  We will also be comparing our results with other algorithms and asses the performance of the work. 

![alt text](https://storage.googleapis.com/kaggle-competitions/kaggle/3649/media/cifar-10.png "Logo Cover")

The Dataset
--------------------------------------------
The CIFAR-10 data consists of 60,000 32x32 color images in 10 classes, with 6000 images per class. There are 50,000 training images and 10,000 test images in the official data.<br>
**Data Set Characteristics:**

    :Number of Images: 60000

    :Number of Classes: 10

    :Class List:
        -airplane 
        -automobile 
        -bird 
        -cat 
        -deer 
        -dog 
        -frog 
        -horse 
        -ship 
        -truck

        The classes are completely mutually exclusive. There is no overlap between automobiles and trucks.<br> 
        "Automobile" includes sedans, SUVs, things of that sort. "Truck" includes only big trucks. Neither includes pickup trucks.


    :Missing Attribute Values: None

    :Class Distribution: uniform

    :Creators:   Alex Krizhevsky, Vinod Nair, and Geoffrey Hinton

Here is the link to the dataset.
https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz

This database is also available on Kaggle:

https://www.kaggle.com/c/cifar-10/overview

    .. topic:: References

   - [Learning Multiple Layers of Features from Tiny Images] (https://www.cs.toronto.edu/~kriz/learning-features-2009-TR.pdf), Alex Krizhevsky, 2009.

Convolutional Neural Networks
------------------------
    In deep learning, a convolutional neural network (CNN, or ConvNet) is a class of deep neural networks, most commonly applied to analyzing visual imagery. They are also known as shift invariant or space invariant artificial neural networks (SIANN), based on their shared-weights architecture and translation invariance characteristics.

    Advantages
    -3D volumes of neurons. The layers of a CNN have neurons arranged in 3 dimensions: width, height and depth.[citation needed] where each neuron inside a convolutional layer is connected to only a small region of the layer before it, called a receptive field. Distinct types of layers, both locally and completely connected, are stacked to form a CNN architecture.
    -Shared weights: In CNNs, each filter is replicated across the entire visual field. These replicated units share the same parameterization (weight vector and bias) and form a feature map. This means that all the neurons in a given convolutional layer respond to the same feature within their specific response field. 
    -Pooling: In a CNN's pooling layers, feature maps are divided into rectangular sub-regions, and the features in each rectangle are independently down-sampled to a single value, commonly by taking their average or maximum value.

    Disadvantages
    Computationally expensive and demands high grade GPUs to run properly.

![alt text](https://miro.medium.com/max/3480/1*uUYc126RU4mnTWwckEbctw@2x.png "Image algo")


STEPS INVOLVED
-------------------------------
  1. Go for Template-CIFAR10.ipynb to work on this project.
  2. The implementation is in cifar-10-cnn-keras.ipynb, i.e solution.
  3. Output predictions are in solution_predictions.csv


Install
-------------------------------
    Supported Python version
        -Python version used in this Project:3.5+

Libraries used
------------------------------
  [Pandas](https://pandas.pydata.org/)
  [Numpy](https://numpy.org/)
  [Matplotlib](https://matplotlib.org/)
  [Sklearn](https://scikit-learn.org/stable/)
  [Seaborn](https://seaborn.pydata.org/)
  [Keras]
  [Tesorflow]

License
--------------------------------
  [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
 
Contact
----------------------------------
  [Dataset Link](https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz)
  [Project Link](https://github.com/decodrtechnologies/Data-Science)

Run
------------------------------
    To run this project you will need an active Pythond distribution such as Anaconda or ActivePython

    To execute the project, run the following command in a python supported prompt such as Anaconda Prompt:
    ipython notebook Template-CIFAR10.ipynb
    
    Goodluck!
