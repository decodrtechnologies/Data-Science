# Facial Recognition using PCA and SVM:
## Problem Description:
Problem statement Facial recognition is an important and more preferred bio metric when compared to other bio metrics. One of the primary reason is that it requires no physical interaction on behalf of the user. For face recognition there are two types of comparisons:

- Verification: In this the system compares the given individual to that the individual says they are and responds with a yes or a no.

- Identification: This is where the system compares the given individual to all the other individuals in the database and recognizes that person.

**In this project we implement the Identification system using Machine Learning concepts such as Principal Component Analysis (PCA) and Support Vector Machine (SVM).**
This technique is one of the basic techniques and thus used in many early face recognition applications. But it has some caveats such as this algorithm required cropped face images with proper light and pose for training. It is very useful in learning the essence of PCA and dimensionality reduction.  

<br>
<p align="center">
<img src="https://raw.githubusercontent.com/samarth0174/PCA-MINIPROJECT/master/dataset_image.png" alt="faces" width="500" height="500">    
</p>
<br>

## Dataset Used:
The dataset used in this example is a preprocessed excerpt of the "Labeled Faces in the Wild", aka LFW_ Download (233MB). 
**The Dataset is available as a part of Sklearn API**.

This dataset is a collection of JPEG pictures of famous people collected over the internet, all details are available on the official website:

    http://vis-www.cs.umass.edu/lfw/

Each picture is centered on a single face. The typical task is called Face Verification: given a pair of two pictures, a binary classifier must predict whether the two images are from the same person.

An alternative task, Face Recognition or Face Identification is: given the picture of the face of an unknown person, identify the name of the person by referring to a gallery of previously seen pictures of identified persons.

Both Face Verification and Face Recognition are tasks that are typically performed on the output of a model trained to perform Face Detection. The most popular model for Face Detection is called Viola-Jones and is implemented in the OpenCV library. The LFW faces were extracted by this face detector from various online websites.

```
   Classes      | 5749
Samples Total   | 13233
Dimensionality  | 5828
   Features     | real, between 0 and 255
``` 
## Steps Involved:
- Importing Libraries
- Loading the Dataset
- Data Exploration
- Splitting the dataset 
- Compute PCA(eigen faces) 
- Train a SVM classification model
- * Using GridSearch to find best Parameters
- Model Evaluation
- Conclusion

## Libraries Required:
- Sklearn 
- Matplotlib
- pandas
- numpy

## Important Concepts:
- PCA(Eigen Faces) - <a href="https://scikit-learn.org/stable/auto_examples/applications/plot_face_recognition.html">Reference</a>
- SVM

## License & Reference:
The original dataset can be refered from **www.cs.umass.edu/lfw/** 
```
Source:
Gary B. Huang, Manu Ramesh, Tamara Berg, and Erik Learned-Miller.
Labeled Faces in the Wild: A Database for Studying Face Recognition in Unconstrained Environments.
University of Massachusetts, Amherst, Technical Report 07-49, October, 2007.
```
