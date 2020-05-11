# Gym Crowd Analysis with PCA :
The data of number of people in a gym is made and collected from a university. the dataset contains 26,000 people counts (per 10 minutes) over one year

## License : 
License of the dataset can be viewed from [here](https://opendatacommons.org/licenses/dbcl/1.0/)

## Objective : 
To predict how crowded a university gym would be at a given time of day (and some other features, including weather)

<img src="https://dcoidtxb1uy9c.cloudfront.net/wp-content/uploads/2014/05/img_4728-copy-2.jpg">

## Data Source and Description: 
The dataset other than number of people counts also contains information about the weather and semester-specific information that might affect how crowded it is. The label is the number of people, which has to be predicted given some subset of the features.

**Label**:

- Number of people

**Features**:

     1. date (string; datetime of data)
     2. timestamp (int; number of seconds since beginning of day)
     3. dayofweek (int; 0 [monday] - 6 [sunday])
     4. is_weekend (int; 0 or 1) [boolean, if 1, it's either saturday or sunday, otherwise 0]
     5. is_holiday (int; 0 or 1) [boolean, if 1 it's a federal holiday, 0 otherwise]
     6. temperature (float; degrees fahrenheit)
     7. isstartof_semester (int; 0 or 1) [boolean, if 1 it's the beginning of a school semester, 0 otherwise]
     8. month (int; 1 [jan] - 12 [dec])
     9. hour (int; 0 - 23)
     
## Libraries used : 
- **numpy**
- **pandas**
- **seaborn**
- **matplotlib**
- **sklearn**

## Data Processing : 
- **OneHotEncoding**
- **Feature Scaling**

## Exploratory Data Analysis :

     - Uni-Variate Analysis : Histograms , Distribution plot
     - Bi-Variate Analysis : Pair Plots
 
 ## Principal component analysis:
 
 - Principal component analysis has been implemented and thouroughly explained in the notebook
 
 ## Modelling : Random Forest
    
      - Random Forest without PCA : Random forest model scores are seen without PCA implementation
      - Random Forest with PCA : Random forest model scores are seen with PCA implementation 
      
## Conclusion :

Based on different model performance, best model is chosen 
