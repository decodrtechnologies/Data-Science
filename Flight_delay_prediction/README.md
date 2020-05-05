# Flight Delay Prediction
## Problem Statement 
Use the given dataset to predict the Flight delay.The dataset contains all the flights in the month of January 2019 and January 2020. There are more than 400,000 flights in the month of January itself throughout the United States.      
Download dataset - https://www.kaggle.com/divyansh22/flight-delay-prediction/download

## Dataset Attributes
**DAY_OF_MONTH** - Day of Month    
**DAY_OF_WEEK**- Day of Week    
**OP_UNIQUE_CARRIER** - Unique Carrier Code. When the same code has been used by multiple carriers, a numeric suffix is used for earlier users, for example, PA, PA(1), PA(2).  
**OP_CARRIER_AIRLINE_ID** -An identification number assigned by US DOT to identify a unique airline (carrier). A unique airline (carrier) is defined as one holding and reporting under the same DOT certificate regardless of its Code, Name, or holding company/corporation.  
**OP_CARRIER** -Code assigned by IATA and commonly used to identify a carrier. As the same code may have been assigned to different carriers over time, the code is not always unique.      
**TAIL_NUM**- Tail Number   
**OP_CARRIER_FL_NUM** -Flight Number    
**ORIGIN_AIRPORT_ID** -Origin Airport, Airport ID. An identification number assigned by US DOT to identify a unique airport.  
**ORIGIN_AIRPORT_SEQ_ID** -Origin Airport, Airport Sequence ID. An identification number assigned by US DOT to identify a unique airport at a given point of time.    
**ORIGIN**- Origin Airport          
**DEST_AIRPORT_ID** -Destination Airport, Airport ID. An identification number assigned by US DOT to identify a unique airport.   
**DEST_AIRPORT_SEQ_ID** -Destination Airport, Airport Sequence ID. An identification number assigned by US DOT to identify a unique airport at a given point of time.     
**DEST** -Destination Airport     
**DEP_TIME**-Actual Departure Time (local time: hhmm)      
**DEP_DEL15**-Departure Delay Indicator, 15 Minutes or More (1=Yes, 0=No)      
**DEP_TIME_BLK**-Departure Time Block, Hourly Intervals       
**ARR_TIME**-Actual Arrival Time (local time: hhmm)         
**ARR_DEL15**-Arrival Delay Indicator, 15 Minutes or More (1=Yes, 0=No)       
**CANCELLED**-Cancelled Flight Indicator (1=Yes, 0=No)        
**DIVERTED**-Diverted Flight Indicator (1=Yes, 0=No)        
**DISTANCE**-Distance between airports (miles)          

## Libraries Used
* Numpy
* Pandas
* Seaborn
* Matplotlib
* sklearn

## Steps involved
1. Importing relevant python Libraries
2. Exploring the Dataset
3. Exploratory Data Analysis
4. Data Preprocessing
5. Model Building
6. Validation
7. Conclusion

## Licence
This data is collected from the Bureau of Transportation Statistics, Govt. of the USA. This data is open-sourced under U.S. Govt. Works.
The dataset is under following licence - https://www.usa.gov/government-works/

## Source
This dataset is sourced from - https://www.kaggle.com/divyansh22/flight-delay-prediction/       
Reference - https://www.kaggle.com/jintolonappan/gbm-tf2-boostedtreesclassifier-export-to-serve
