# Houses_Kc_Price_Prediction

# Problem Statement:
House Data Price Prediction Using Multiple Regression and Backward Elimination Technique using Sckit-Learn Library.
# Description:
Here in this business problem, we want to find out the prices of Houses in King County,USA. Here we are given many parameters which directly influence the prices of the houses. We need to find the best quoted value for the price considering all the dependent parameters and we need to observe which parameters plays a key role in price determination of the houses.

**Since this is a problem of PREDICTION ANALYSIS we will use MULTIPLE REGRESSION ANALYSIS WITH BACKWARD ELIMINATION TECHNIQUE.**

**What is Multiple Regression and Backward Elimination Technique:**

MULTIPLE REGRESSION: Multiple regression is an extension of simple linear regression. It is used when we want to predict the value of an dependent variable based on the value of two or more other independent variables. The variable we want to predict is called the dependent variable (or sometimes, the outcome, target or criterion variable).

BACKWARD ELIMINATION TECHNIQUE:Backward elimination is a feature selection technique while building a machine learning model. It is used to remove those features(independent variables) that do not have a significant effect on the dependent variable or prediction of output.

 **Steps involved in backward Elimination Technique:**
 
1. Select a significance level to stay in the model (eg. SL = 0.05)
2. Fit the model with all possible independent variables.
3. Consider the independent variable with the highest P-value. If P>SL, go to point 4.).
4. Remove this independent variable .
5. Fit the model without this variable and repeat the step 3.) until the condition becomes false.

# DATA
The kc_house_data excel file contains our complete dataset. This data is colleceted through surveys and by estimation of analysts.
We have total 21613 historical data prices for houses in USA.

 **Independent Variables/Features: All are numerical Data**
1.	id   
2.	date
3.	bedrooms
4.	bathrooms
5.	sqft_living
6.	sqft_lot
7.	floors
8.	waterfront
9.	view
10. condition
11.	grade
12.	sqft_above
13.	sqft_basement
14.	yr_built
15.	yr_renovated
16.	zipcode
17.	lat
18.	long
19.	sqft_living15
20.	sqft_lot15

**Dependent Variable - PRICE**

We have test data whose size is one-third of our training dataset.
The dataset is uniform and consitent and the data have ratio scale of measurement.

# Data Pre-Processing:
1. Load all the relevat python libraries.
2. Load the excel file kc_house_data.
3. There were some null values in tha dataset that have been removed , this is an important step so that regression model can be run successfully.
4. After that we observe that id and date column does not play a key role in price determination , so we need to drop these two columns.
5. Now our data is clean and ready to be processed under Regression Model in Python.

**Libraries Required :**
- Sklearn 
- Matplotlib
- pandas
- numpy
- Seaborn
- Collections

 **Steps :**
1. Importing relevant python Libraries
2. Exploring the Dataset
3. Exploratory Data Analysis
> * Univariate Analysis
4. Data Preprocessing
5. Model Building
> * Regression Model
> * Backward Elimination Technique
6. Validation
> *Regression Matrix (p test-Significance Test)
7. Conclusion

# EDA (Exploratory Data Analysis):
For EDA , Seaborn Data Visualization Library is used which is based on Matplotlib . Several distributions and plots have been depicted to understand the pattern of housing industry.
We have used scikit-learn library for running regression model.
And Finally we have used OLS (Ordinary Least Square Method) for our regression Model. For this we have used Statsmodels Module, which is built on on top of numerical library Numpy. We get a Final Model after running a regression Model with an excellent R squared value of 0.905.

**Our Model is consistent with an excellent R squared value of 0.905. This clearly shows that most of the variation in the prices are very well expalined by these independent features. We have retained all those features whose p value < 0.05.**

# Model Building:
* Split dependent and independent features.
* Split the data into train and test in 67 : 33 ratio.
* Fit Multiple Regression and Backward Elimination Technique on training set, predict and check accuracy.


**Install**
- Supported Python version
    - Python version used in this Project : 3.5+

**Run**
    - To run this project use - Anaconda, which provides support for running .ipynb files (Jupyter Notebook). 
    
    - After making sure you have that, you can run from a terminal or cmd next lines :
    - ipython notebook kc_housing_price.ipynb
   


