# Web-Scrapying

Web scraping is a computer software technique of extracting information from websites. 
This technique mostly focuses on the transformation of unstructured data (HTML format) on the web into structured data (database or spreadsheet). 

## PROBLEM STATEMENT: 

Crawl popular websites & create a database of Indian movie celebrities with their images and details.

### Website : IMDB

### Requirements

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. 

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [lxml](https://pypi.org/project/lxml/)
- [opencv](https://opencv.org/)

### Run

In a terminal or command window, navigate to the top-level project directory `
IMDB WEB-SCRAPYING/` (that contains this README) and run one of the following commands:


ipython notebook Imdb web-scaryping.ipynb

or

jupyter notebook Imdb web-scaryping.ipynb


This will open the Jupyter Notebook software and project file in your browser.

### Steps :
1. Importing Libraries
2. List down the URLs
3. Create the class to extract details from a url
> * Title of the page
> * Content in the page
  > * Name of actor
  > * Image Url
  > * Details
  > * Image
4. Create Dataframe
5. Remove duplicates
6. Display
7. Store in csv

