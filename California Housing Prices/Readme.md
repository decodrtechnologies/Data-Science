# California Housing Data

This is the dataset used in the second chapter of Aurélien Géron's recent book 'Hands-On Machine learning with Scikit-Learn and TensorFlow'.
It serves as an excellent introduction to implementing machine learning algorithms because it requires rudimentary data cleaning, has an easily understandable list of variables and sits at an optimal size between being to toyish and too cumbersome.

The data contains information from the 1990 California census.

## License : 

License for this dataset cam be accessed [here](https://creativecommons.org/publicdomain/zero/1.0/)

<img src="https://www.mercurynews.com/wp-content/uploads/2018/04/aerial-jah1.jpg">

## Objective : 

To predict the prices of houses in Californa based on their different specifications and locations

## Data Description : 

The Dataset is built using the 1990 California census data. It contains one row per census block group. A block group is the smallest geographical unit for which the U.S. Census Bureau publishes sample data (a block group typically has a population of 600 to 3,000 people).

The information was collected on the variables using all the block groups in California from the 1990 Census. In this sample a block group on average includes 1425.5 individuals living in a geographically compact area. Naturally, the geographical area included varies inversely with the population density. Distances were computed among the centroids of each block group as measured in latitude and longitude and all the districts reporting zero entries for the independent and dependent variables were excluded. The final data contained 20,640 observations on 9 variables. The dependent variable is ln(median house value). The other variables are as follows: 

    1. longitude: A measure of how far west a house is; a higher value is farther west
    2. latitude: A measure of how far north a house is; a higher value is farther north
    3. housingMedianAge: Median age of a house within a block; a lower number is a newer building
    4. totalRooms: Total number of rooms within a block
    5. totalBedrooms: Total number of bedrooms within a block
    6. population: Total number of people residing within a block
    7. households: Total number of households, a group of people residing within a home unit, for a block
    8. medianIncome: Median income for households within a block of houses (measured in tens of thousands of US Dollars)
    9. medianHouseValue: Median house value for households within a block (measured in US Dollars)
    10. oceanProximity: Location of the house w.r.t ocean/sea

## Libraries Used : 
 - pandas
 - numpy
 - matplotlib
 - seaborn
 - sklearn

## Exploratory Data Analysis : 

    - Univariate Analysis : Boxplots , Histograms and Barplot
    - Bi-Variate Analysis : Scatter Matrix
    - multi-Variate Analysis : Scatter plots

## Data Cleaning and Manipulations:

Data is cleaned , missing values are handled etc and data is manipulated to make more meaningful attributes or remove redundant ones

## Straitified Sampling : 
Idea is explained and implementation of stratified sampling is done in this section

## Modelling and HyperTuning : 

Three regression algorithms i.e 
    
    -Linear Regression
    -Decision Tree
    -Random Forest 

are explained thoroughly and implemented in this section.

HyperTuning with the help of GridSearch is also explained extensively and used to find best parameters 

## Conclusion : 

All models are analysed and the best one is chosen

## Acknowledgements :
This data was initially featured in the following paper:
Pace, R. Kelley, and Ronald Barry. "Sparse spatial autoregressions." Statistics & Probability Letters 33.3 (1997): 291-297.
and I encountered it in 'Hands-On Machine learning with Scikit-Learn and TensorFlow' by Aurélien Géron.

## Source :
Aurélien Géron wrote:
This dataset is a modified version of the California Housing dataset available from:
[Luís Torgo's](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html) page (University of Porto)

## Contact : 
**Kushagra Thakral** : `kthakral@ch.iitr.ac.in`
