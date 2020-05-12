# Build-machine-learning-pipelines-pyspark
PySpark is a Python API for Spark released by the Apache Spark community to support Python with Spark. Using PySpark, one can easily integrate and work with RDDs in Python programming language too. There are numerous features that make PySpark such an amazing framework when it comes to working with huge datasets. Whether it is to perform computations on large datasets or to just analyze them, Data Engineers are switching to this tool.

<b>This project is a complete implementation of building pipelines using Pyspark</b>
<br>
<p align="center">
<img src="https://databricks.com/wp-content/uploads/2018/12/PySpark-1024x164.png" alt="pyspark">    
</p>
<br>

## Steps Involved:
* Step 1) Basic operation with PySpark
* Step 2) Data preprocessing
* Step 3) Build a data processing pipeline
* Step 4) Build the classifier
* Step 5) Train and evaluate the model
* Step 6) Tune the hyperparameter
<br>

## Libraries Required:
- pyspark
- py4j(pre installed used by pyspark)


## Dataset:
**Predict whether income exceeds $50K/yr based on census data. Also known as "Census Income" dataset.The given problem is a binary classsification task.**

**Attribute Information:**
```

Listing of attributes:

label to be predicted(income) : >50K, <=50K.

age: continuous.
workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.
fnlwgt: continuous.
education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.
education-num: continuous.
marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.
occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.
relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.
race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.
sex: Female, Male.
capital-gain: continuous.
capital-loss: continuous.
hours-per-week: continuous.
native-country: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands.

```
<br>

## Model Used:
Major focus of this project is to work with large amount of data using Spark cluster computing concept.
Logistic Regression is used for the given binary classification task.

## License & References:
- The original dataset can be acessed at <a href="http://archive.ics.uci.edu/ml/datasets/adult">UCI REPOSITORY</a>
```
Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science. 
```
