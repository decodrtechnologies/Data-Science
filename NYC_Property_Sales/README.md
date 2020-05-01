# Regression Analysis using NYC Property Sales Dataset
The detailed work can be found on the regression-nyc.ipynb file with individual explanation before every cell. 

## Background 
Regression analysis is defined as a method that examines the relationship between one or more independent variables and a dependent variable by plotting points on a graph and through statistical analysis; used to identify and weight analytical factors and to make forecasts.

Regression analysis is used by many different professions to determine the impact different variables may or may not have on a dependent variable. For instance, some companies will use regression analysis to determine if the number of days it rains impact sales. Any business that has access to data can study different variables to determine it's impact. This analysis, if performed correctly, can be very useful for businesses.

Too often in real estate, the process of valuation can come across as a high-brow exercise of thumb-sucking. The realtor will come over, kick the proverbial tires, and then produce an estimated value with very little “quantitative” insight. Perhaps the process is exacerbated by the emotional attachment that owning property brings given that for many, a house will be the largest financial investment made in a lifetime.

Regression analysis is one tool or method that real estate appraisers use in or to determine value adjustments. When appraisers use regression analysis they will compare the sale price (dependent variable) to many independent variables. Appraisers can use statistical data and analyze it.

If you have enough data, regression analysis can be used to see the relationship of several different variables in relationship to the sale price.   When looking at a large number of sales within a neighborhood certain variables can be determined by using a regression analysis. 

We will be using the New York City Property sales dataset and try to derive insights using Regression Analysis

## NYC Property Sales dataset

# Context

This dataset is a record of every building or building unit (apartment, etc.) sold in the New York City property market over a 12-month period. 

# Content

This dataset contains the location, address, type, sale price, and sale date of building units sold. A reference on the trickier fields:

 * BOROUGH: A digit code for the borough the property is located in; in order these are Manhattan (1), Bronx (2), Brooklyn (3), Queens (4), and Staten Island (5).
 * BLOCK; LOT: The combination of borough, block, and lot forms a unique key for property in New York City. Commonly called a BBL.
 * BUILDING CLASS AT PRESENT and BUILDING CLASS AT TIME OF SALE: The type of building at various points in time. See the glossary linked to below.

For further reference on individual fields see the [Glossary of Terms](http://www1.nyc.gov/assets/finance/downloads/pdf/07pdf/glossary_rsf071607.pdf). For the building classification codes see the [Building Classifications Glossary](http://www1.nyc.gov/assets/finance/jump/hlpbldgcode.html).

Note that because this is a financial transaction dataset, there are some points that need to be kept in mind:

 * Many sales occur with a nonsensically small dollar amount: $0 most commonly. These sales are actually transfers of deeds between parties: for example, parents transferring ownership to their home to a child after moving out for retirement.
 * This dataset uses the financial definition of a building/building unit, for tax purposes. In case a single entity owns the building in question, a sale covers the value of the entire building. In case a building is owned piecemeal by its residents (a condominium), a sale refers to a single apartment (or group of apartments) owned by some individual.

## Inspiration

What can you discover about New York City real estate by looking at a year's worth of raw transaction records? Can you spot trends in the market, or build a model that predicts sale value in the future?

## Associated tasks

	IN ORDER:
    - Loading Libraries and Dataset
    - Data Inspection and Visualization
    - Data Pre Processing
    - Modelling the data using Linear, Lasso, Ridge and Random Forest Regressor
		
	


## Files

	- README.md
	- nyc-rolling-sales.csv : Data file
    - regression-nyc.ipynb: Jupyter Notebook file.


## License
[CC0 1.0 Universal-Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)



## ACKNOWLEDGEMENTS
===============================================================================
This dataset is a concatenated and slightly cleaned-up version of the New York City Department of Finance's [Rolling Sales dataset](http://www1.nyc.gov/site/finance/taxes/property-rolling-sales-data.page).
