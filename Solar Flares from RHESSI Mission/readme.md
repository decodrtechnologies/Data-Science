# Solar Flares from RHESSI Mission:

## Background:

A solar flare is a sudden flash of increased brightness on the Sun, usually observed near its surface and a sunspot group. Powerful flares are often, but not always, accompanied by a coronal mass ejection. Even the most powerful flares are barely detectable in the total solar irradiance. RHESSI's  (Reuven Ramaty High Energy Solar Spectroscopic Imager) s a NASA solar flare observatory. Its primary mission is to explore the basic physics of particle acceleration and explosive energy release in solar flares. You can learn more about the RHESSI through this [link](https://hesperia.gsfc.nasa.gov/hessi/objectives.htm).

In this project, we'll be observing the data available through the Solar Flares from the RHESSI dataset available on Kaggle. 
 
## Dataset Description:

The dataset has 113942 entries with 18 columns. The dataset is obtained from [Kaggle](https://www.kaggle.com/khsamaha/solar-flares-rhessi) which was originally contributed by [RHESSI](https://hesperia.gsfc.nasa.gov/rhessi_data_search/rhessi_data_search_vme.html).

## Attribute Description:

Flare - Numeric - An ID number, ymmddnn, e.g., 2042101 is the first flare found for 21-Apr-2002. 
        These numbers are not time ordered.

Start.date - DateTime - The date when the flare occurred

Start.time - DateTime - Flare start time

Peak -DateTime - Flare peak time

End - String - Flare end time

Dur[s] - Numeric - Duration of flare in seconds

Peak[c/s] - Numeric - Peak count rate in corrected counts, peak counts/second

Total Counts - Numeric -  Total of counts in corrected counts, counts in energy range

Energy [keV] - String - The highest energy band in which the flare was observed.

X pos [asec] -  Numeric -  Flare position in arcsec from sun center

Y pos [asec] - Numeric -  Flare position in arcsec from sun center

Radial [asec] - Radial distance in arcsec from sun center

active.region.ar - String - No Description

flag.1 - String - No Description

flag.2 - String - No Description

flag.3 - String - No Description

flag.4 -  String - No Description

flag.5 -  String - No Description


### Flags - Quality Codes:

Flare Flag Codes:

List item
        a0 - In attenuator state 0 (None) sometime during flare
        
        a1 - In attenuator state 1 (Thin) sometime during flare
        
        a2 - In attenuator state 2 (Thick) sometime during flare
        
        a3 - In attenuator state 3 (Both) sometime during flare
        
        An - Attenuator state (0=None, 1=Thin, 2=Thick, 3=Both) at peak of flare
        
        DF - Front segment counts were decimated sometime during flare
        
        DR - Rear segment counts were decimated sometime during flare
        
        ED - Spacecraft eclipse (night) sometime during flare
        
        EE - Flare ended in spacecraft eclipse (night)
        
        ES - Flare started in spacecraft eclipse (night)
        
        FE - Flare ongoing at end of file
        
        FR - In Fast Rate Mode
        
        FS - Flare ongoing at start of file
        
        GD - Data gap during flare
        
        GE - Flare ended in data gap
        
        GS - Flare started in data gap
        
        MR - Spacecraft in high-latitude zone during flare
        
        NS - Non-solar event
        
        PE - Particle event: Particles are present
        
        PS - Possible Solar Flare; in front detectors, but no position
        
        Pn - Position Quality: P0 = Position is NOT valid, P1 = Position is valid
        
        Qn - Data Quality: Q0 = Highest Quality, Q11 = Lowest Quality
        
        SD - Spacecraft was in SAA sometime during flare
        
        SE - Flare ended when spacecraft was in SAA
        
        SS - Flare started when spacecraft was in SAA

## Libraries Used:

Pandas

Matplotlib

Sklearn

Seaborn

Numpy

## Run:

The entire coding is done by using the jupyter notebook. It can be installed by following the steps given in this [link](https://jupyter.org/install). 

## Algorithm:

The dataset can be dealt with various models. Here I am using the Decision Tree Classifier and the Random Forest Classifier  to predict the data and compare them.  

### Decision Tree Classifier:

Decision tree learning is one of the predictive modeling approaches that is used in statistics, data mining, and machine learning. It uses a decision tree (as a predictive model) to go from observing about an item (represented in the branches) to concluding about the item's target value (represented in the leaves). Tree models where the target variable can take a discrete set of values are called classification trees; in these tree structures, leaves represent class labels, and branches represent conjunctions of features that lead to those class labels. Decision trees where the target variable can take continuous values (typically real numbers) are called regression trees.

Advantages:

It is easier to understand and interpret. This can handle both numerical and categorical data. It requires little data preparation. It is possible to validate a model using statistical tests. It performs well with large datasets.

Disadvantages:

Trees can be very non-robust. A small change in the training data can result in a large change in the tree and consequently the final predictions. Decision-tree learners can create over-complex trees that do not generalize well from the training data(This is known as overfitting). For data including categorical variables with different numbers of levels, information gain in decision trees is biased in favor of attributes with more levels. 

### Random Forest Classifier:

Random forests or random decision forests are an ensemble learning method for classification, regression, and other tasks that operate by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees. Random decision forests correct for decision trees' habit of overfitting to their training set.


## Tasks:

Here, we are learning to do:

Data Handling

Importing Data with Pandas

Cleaning Data

Exploring Data through Visualizations with Matplotlib

Building Machine Learning Models

Validation

## License:

Solar Flares from RHESSI Mission dataset used in the problem is available open-source on Kaggle and the license is available at this [link](https://creativecommons.org/publicdomain/zero/1.0/).
