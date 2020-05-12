# Glass Classification and Prediction
The detailed work can be found on the Glass_Classification.ipynb file.
## Background 

The study of classification of types of glass was motivated by criminological investigation. At the scene of the crime, the glass left can be used as evidence...if it is correctly identified!

## Glass Classification Database

**Context**

This is a Glass Identification Data Set from UCI. It contains 10 attributes including id. The response is glass type(discrete 7 values).

**Content**

Attribute Information:

 * Id number: 1 to 214 (removed from CSV file)
 * RI: refractive index
 * Na: Sodium (unit measurement: weight percent in corresponding oxide, as are attributes all the below mentioned attributes)
 * Mg: Magnesium
 * Al: Aluminum
 * Si: Silicon
 * K: Potassium
 * Ca: Calcium
 * Ba: Barium
 * Fe: Iron
 * Type of glass: (class attribute)
    -- 1 buildingwindowsfloatprocessed 
    -- 2 buildingwindowsnonfloatprocessed 
    -- 3 vehiclewindowsfloatprocessed
    -- 4 vehiclewindowsnonfloatprocessed (none in this database)
    -- 5 containers
    -- 6 tableware
    -- 7 headlamps

**Acknowledgements**


Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Glass+Identification)


Creator:
B. German
Central Research Establishment
Home Office Forensic Science Service
Aldermaston, Reading, Berkshire RG7 4PN

Donor:
Vina Spiehler, Ph.D., DABFT
Diagnostic Products Corporation
(213) 776-0180 (ext 3014)

**Inspiration**

Data exploration of this dataset reveals two important characteristics :
1) The variables are highly corelated with each other including the response variables:
So which kind of ML algorithm is most suitable for this dataset Random Forest , KNN or other? Also since dataset is too small is there any chance of applying PCA or it should be completely avoided?

2) Highly Skewed Data:
Is scaling sufficient or are there any other techniques which should be applied to normalize data? Like BOX-COX Power transformation?

## Associated tasks

	IN ORDER:
    -Predicting with Linear Regression
    -Predicting Using Logistic Regression
    -Class Probablilites and Class Predictions
    -Comparing Predictions
    -Model Evaluation
		


## Files

	- README.md
	- glass.csv : Data file
    - Glass_Classification.ipynb: Jupyter Notebook file.


## License
[Database Contents License (DbCL) v1.0](https://opendatacommons.org/licenses/dbcl/1.0/)
