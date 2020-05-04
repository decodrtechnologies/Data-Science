<h1>Blue Book for Bulldozers</h1>

<h2>Problem definition</h2>

Predict the auction sale price for a piece of heavy equipment to create a "blue book" for bulldozers..

<h2>Data</h2>

The data is downloaded from the Kaggle Bluebook for Bulldozers competition: https://www.kaggle.com/c/bluebook-for-bulldozers/data

  -There are 3 main datasets:

   - Train.csv is the training set, which contains data through the end of 2011.

   - Valid.csv is the validation set, which contains data from January 1, 2012 - April 30, 2012 You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.

   - Test.csv is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012. Your score on the test set determines your final rank for the competition.

<h2>Evaluation</h2>

The evaluation metric for this competition is the RMSLE (root mean squared log error) between the actual and predicted auction prices.

For more on the evaluation of this project check: https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation

Note: The goal for most regression evaluation metrics is to minimize the error. For example, our goal for this project will be to build a machine learning model which minimises RMSLE.

<h2>Install</h2>

  - Supported Python version - Python version used in this Project : 3.5+

<h2>Run</h2>

- To run this project use - Anaconda, which provides support for running .ipynb files (Jupyter Notebook).
  - After making sure you have that, you can run from a terminal or cmd next lines :
  - ipython notebook Business Problem Statement.ipynb 
  - ipython notebook 02 - Data-Pre-Processing-EDA-Visualization-Model-Buliding.ipynb
