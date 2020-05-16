AVIATION ACCIDENT ANALYSIS
---------------------------------------------------

**Project:**

    :This project is meant to explore, analyse and visualize aviation accidents and related factors such as reasons, survival rates, fatalities, locations etc. Further, the following factors are needed to be analysed:
      -The planes crashed per year.
      -People aboard per year during crashes.
      -People dead per year during crashes.
      -People survived per year during crashes.


![alt text](https://www.aopa.org/-/media/Images/AOPA-Main/News-and-Media/Publications/Pilot-Magazine/2020/2003/2003t_accident/2003t_accident_16x9.jpg "Title Img")

Dataset - Airplane Crashes and Fatalities since 1908
----------------------------------------------------

**Data Set Characteristics:**

    :This dataset includes:
        -All civil and commercial aviation accidents of scheduled and non-scheduled passenger airliners worldwide, which resulted in a            fatality (including all U.S. Part 121 and Part 135 fatal accidents).
        -All cargo, positioning, ferry and test flight fatal accidents.
        -All military transport accidents with 10 or more fatalities.
        -All commercial and military helicopter accidents with greater than 10 fatalities.
        -All civil and military airship accidents involving fatalities.
        -Aviation accidents involving the death of famous people.
        -Aviation accidents or incidents of noteworthy interest.
        
    :Attribute Information:
        -Date:      Date of accident, in the format - January 01, 2001
        -Time:      Local time, in 24 hr. format unless otherwise specified
        -Location:  Location of the accident
        -Operator:  Airline or operator of the aircraft
        -Flight:    #Flight number assigned by the aircraft operator
        -Route:     Complete or partial route flown prior to the accident
        -Type:      Aircraft type
        -Registration:ICAO registration of the aircraft
        -cn/In:     Construction or serial number / Line or fuselage number
        -Aboard:    Total aboard (passengers / crew)
        -Fatalities:Total fatalities aboard (passengers / crew)
        -Ground:    Total killed on the ground
        -Summary:   Brief description of the accident and cause if known


    :Missing Attribute Values: 
        -Date               0
        -Time            2219
        -Location          20
        -Operator          18
        -Flight #        4199
        -Route           1706
        -Type              27
        -Registration     335
        -cn/In           1228
        -Aboard            22
        -Fatalities        12
        -Ground            22
        -Summary          390

    :Creator:  Sauro Grandi

    :Date: September, 2016




STEPS INVOLVED
-------------------------------
  1. Go to Template_Aviation.ipynb to work on the project.
  2. The data analysis is done using two files, Dataset1 and Dataset2.
  3. Implementation is available in Airplane Crashes (Analysis&Visualization).ipynb

Install
-------------------------------
    Supported Python version
        -Python version used in this Project:3.5+

Libraries used
------------------------------
    Pandas
    Matplotlib
    Numpy
    Seaborn
    Datetime

License
--------------------------------
    The dataset is covered by the following license: Open Database License (ODbL) v1.0
    https://opendata.socrata.com/Government/Airplane-Crashes-and-Fatalities-Since-1908/q2te-8cvq
    
Contact
----------------------------------
    Dataset Link-  https://www.kaggle.com/saurograndi/airplane-crashes-since-1908
    Project Link-  https://github.com/decodrtechnologies/Data-Science/tree/master/Aviation%20Accident%20Analysis

Run
------------------------------
    To run this project you will need an active Pythond distribution such as Anaconda or ActivePython

    To execute the project, run the following command in a python supported prompt such as Anaconda Prompt:
    ipython notebook Template_Aviation.ipynb
    
    Goodluck!
