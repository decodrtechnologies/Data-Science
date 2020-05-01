# Abalone Age Prediction:
## Problem Description:
Predicting the age of abalone from physical measurements. The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope -- a boring and time-consuming task. Other measurements, which are easier to obtain, are used to predict the age. Further information, such as weather patterns and location (hence food availability) may be required to solve the problem. 
<br>
<p align="center">
<img src="https://miro.medium.com/max/2000/1*W3e117artUa9v4JrpjX9Gw.jpeg" alt="abalone" width="500" height="300">    
</p>
<br>

## Steps Involved:
- Importing Libraries
- Importing the Dataset
- Exploratory Data Analysis
> * Univariate Analysis
> * Bivariate Analysis
- Data preprocessing 
> * Outlier Handling
> * Feature Selection and Standardization
- Modeling 
- Evaluation
- Fine tuning using GridSearchCV
- Conclusion
<br>

## Libraries Required:
- Sklearn 
- Matplotlib
- pandas
- numpy
- Seaborn
- scipy

## Data Attribute Information
**Given is the attribute name, attribute type, the measurement unit and a brief description. The number of rings is the value to predict: Since its a Continuous Variable therefore a Regression Problem.**
```
Name / Data Type / Measurement Unit / Description ¶

Sex / nominal / -- / M, F, and I (infant)

Length / continuous / mm / Longest shell measurement

Diameter / continuous / mm / perpendicular to length

Height / continuous / mm / with meat in shell

Whole weight / continuous / grams / whole abalone

Shucked weight / continuous / grams / weight of meat

Viscera weight / continuous / grams / gut weight (after bleeding)

Shell weight / continuous / grams / after being dried

Rings / integer / -- / +1.5 gives the age in years
```
<br>

##  Machine learning models:

```
    Linear Regressor
    SVR
    RandomForest Regressor
    ElasticNet Regression
    Lasso Regression
    Kernel Ridge Regression
    Gradient Boosting Regression
    XGBoost
    LightGBM
    can also try any other classifiers.
   
``` 
- use Gridsearch CV to tune algos

## License & References:
- The original dataset can be acessed at <a href="https://archive.ics.uci.edu/ml/datasets/abalone">UCI REPOSITORY</a>
```
Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science. 
```
