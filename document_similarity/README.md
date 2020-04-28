# All the News Data Set
The detailed work can be found on the .ipynb file with individual explanation before every cell. 

# Dataset Description 

All the news conatins severl articles, whicha re clustered together. Articles are collected from several websites like, Newyork times, Fox news, Buzzfeed News and many more. 

## All the News Dataset

All the news Dataset contains 10 coloumns which are Document ID, Date, Year, Month, Publication, content, article title, article url and author. for Document Similarity we would be working on Document ID, Content, Article title.


## Background 

Context based similar documents is oen of the best problem in machine learning.
in conetxt based similar documents one needs to find the similarity among the query document and the dataset.
For recommnedations it is really necassary to find the documets. for an example, you can recommned readers , blogs , news articles and many more. several techniques are used to solve such problems like tags, categories and much more. but all the of them are not efficent. hence we need to make use of document similarity concept.

On computational side, the problem can be divided into two sets.

Input: As a input you have a huge dataset, whcih do contains the title of document and its content.
Also, all the documents are poorly classified in different subcategories or categories.

Query.
A set of input documents or document.
K documents needs to be searched based on similarity with the 
## Data Set



## Associated tasks

	- Building a LDA model: 
		in order to solve this problem, one needs to find the relation between the documents and topics, whcih can be done using lDA. based on LDA. A lDA model will create a bag of words and it will provide the signature of uniqueness by listing all the most frequent words in the document.
	
	- Applying LDA model on the Query Document:  
		once the LDA model has be created you need to apply on the document. A LDA model would provide a vector of D as Dimensiion. With the vectorizaton, N documents will be transform into N ponts in D dimension space. When the two points will be close to each other we can say documents are similar.

## Files

	- Readme.txt
	- ipynb File for more brief descripton.
	
## Dataset characteristics
	
All the news Dataset contains, the three csvs, article1.csv, article2.csv and article4.csv.

## License
Following dataset has been aqcuried from the following in link.
https://www.kaggle.com/snapcrack/all-the-news


