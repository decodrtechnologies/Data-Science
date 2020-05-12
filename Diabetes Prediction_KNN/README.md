# Diabetes Classification and Prediction using KNN
The detailed work can be found on the Diabetes_Prediction_KNN.ipynb file with individual explanation before every cell. 

## Background 
In pattern recognition, the k-nearest neighbors algorithm (k-NN) is a non-parametric method used for classification and regression.In both cases, the input consists of the k closest training examples in the feature space. The output depends on whether k-NN is used for classification or regression:

 * In k-NN classification, the output is a class membership. An object is classified by a plurality vote of its neighbors, with the object being assigned to the class most common among its k nearest neighbors (k is a positive integer, typically small). If k = 1, then the object is simply assigned to the class of that single nearest neighbor.

 * In k-NN regression, the output is the property value for the object. This value is the average of the values of k nearest neighbors.

k-NN is a type of instance-based learning, or lazy learning, where the function is only approximated locally and all computation is deferred until function evaluation.

Both for classification and regression, a useful technique can be to assign weights to the contributions of the neighbors, so that the nearer neighbors contribute more to the average than the more distant ones. For example, a common weighting scheme consists in giving each neighbor a weight of 1/d, where d is the distance to the neighbor.

The neighbors are taken from a set of objects for which the class (for k-NN classification) or the object property value (for k-NN regression) is known. This can be thought of as the training set for the algorithm, though no explicit training step is required.

A peculiarity of the k-NN algorithm is that it is sensitive to the local structure of the data. 

We will be using the Pima Indians Diabetes Databetes dataset and try to derive predictions using the K-Nearest Neighbours algorithm.

## Pima Indians Diabetes Database

**Context**

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.

**Content**

The datasets consists of several medical predictor variables and one target variable, Outcome. 
Predictor variables includes :
 * Number of pregnancies 
 * BMI 
 * Insulin Level
 * Age
 * Glucose
 * Blood Pressure
 * Skin Thickness
 * Diabetes Pedigree Function

**Acknowledgements**

Smith, J.W., Everhart, J.E., Dickson, W.C., Knowler, W.C., & Johannes, R.S. (1988). 
[Using the ADAP learning algorithm to forecast the onset of diabetes mellitus.](http://rexa.info/paper/04587c10a7c92baa01948f71f2513d5928fe8e81). 
In Proceedings of the Symposium on Computer Applications and Medical Care (pp. 261--265). IEEE Computer Society Press.

**Inspiration**

Can you build a machine learning model to accurately predict whether or not the patients in the dataset have diabetes or not?

## Associated tasks

	IN ORDER:
    - Basic EDA and Statistical Analysis
    - Cleaning and plotting the data
    - Scaling the Data
    - Test Train Split and Cross Validation Methods
    - Result Visualization
    - Model Performance Analysis
    - Hyper Parameter Optimization
		
	


## Files

	- README.md
	- diabetes.csv : Data file
    - Diabetes Prediction_KNN.ipynb: Jupyter Notebook file.


## License
[CC0 1.0 Universal-Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)



##ACKNOWLEDGEMENTS
===============================================================================
This dataset is a concatenated and slightly cleaned-up version of the New York City Department of Finance's [Rolling Sales dataset](http://www1.nyc.gov/site/finance/taxes/property-rolling-sales-data.page).
