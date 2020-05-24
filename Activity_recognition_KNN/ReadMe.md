# Human Activity Recogonition Using Smartphones - KNeighbors Classifier

In this project you will design a robust activity recogonition system based on the smartphones.
As you know mobile devices have accelerometer as the sensor which collects the activities.
These activities can be classified using K-nearest neighbour. 


### REQUIREMENT
1. Pandas
2. Numpy
3. Matplotlib
4. Scikit Learn

### Data
We will be using a [human-activity-recognition-with-smartphones](https://www.kaggle.com/uciml/human-activity-recognition-with-smartphones) from the Kaggle platform which has a very good collection of datasets.

The file we will be using is present in following directory :  ` input/`
It is under license CCO and it is by UCI machine learning repositories
 
### Attribute Information:

For each record in the dataset it is provided:
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope.
- A 561-feature vector with time and frequency domain variables.
- Its activity label.
- An identifier of the subject who carried out the experiment.

### [License](https://creativecommons.org/publicdomain/zero/1.0/)

### STEPS :
1. Importing Libraries
2. Exploring the Dataset
3. Exploratory Data Analysis
4. Data Preprocessing
5. Model Building
    >* KNeighborsClassifier
6. Evaluation
7. Conclusion

### Citation Request:
- Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. A Public Domain Dataset for Human Activity Recognition Using Smartphones. 21th European Symposium on Artificial Neural Networks, Computational Intelligence and Machine Learning, ESANN 2013. Bruges, Belgium 24-26 April 2013.

### Run

In a terminal or command window, navigate to the top-level project directory ` Activity_recognition_KNN/` (that contains this README) and run one of the following commands:


ipython notebook Activity recognition_KNN_task.ipynb
or

jupyter notebook Activity recognition_KNN_task.ipynb


This will open the Jupyter Notebook software and project file in your browser.

### Further readings:
- https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm
- https://machinelearningmastery.com/how-to-model-human-activity-from-smartphone-data/
