# Jokes Recommender Using Matrix Factorization Techniques via PySpark
The detailed work can be found on the .ipynb file with individual explanation before every cell. 

## Background 

Suppose you're planning to buy a laptop without any idea about the right configuration. So You would check with your friends and colleagues for recommendation and they suggests laptops based on your requirement, their knowledge and current trends in the market of the product(laptop). 
This is the way a Recommendation engine works. 
For instance, Amazon recommends you a laptop based on your previous search history, product popularity and keeps on showing the best recommendations so as to tempt the user to to buy a laptop . All the major companies have recommendation in their products such as Youtube shows recommendations based on your interests and activity and in the same way Netlix suggests you which movie or TV series ti watch next using a Recommendation Engine.

In this project you will implement a movie Recommendation system.
We'll explore how to implement it, before that there are two types of Recommendation Engine:
1. **Content Based Filtering**
2. **Collaborative Filtering**

**Content Based Filtering**

 * Content-based filtering methods are based on a description of the item and a profile of the user's preferences.
 * These methods are best suited to situations where there is known data on an item (name, location, description, etc.), but not on the user
 * The habits of users can change. This situation makes it hard to adapt to the need of the user. However, the attributes of movies don't change with time so recommendation becomes easier.
 * Content-based recommenders treat recommendation as a user-specific classification problem and learn a classifier for the user's likes and dislikes based on an item's features. 
 * In item based recommendation systems, we need to make user vs item matrix that we use also in user based recommender systems.
     * Each row is user and each column is items like movie, product or websites.
     * Then we calculate similarity between columns that are items like movies or stuffs.

**Collaborative Filtering**

 * Collaborative filtering makes recommendations on the basis of a combination of factors defining your experience and experiences of other people.
 * First, we make an user vs item matrix.
     * Each row represents an user and each column represents items like movie, product or websites.
 * Second, we compute similarity scores between users.
     * Each row represents an user and each row is a vector.
     * We then compute similarity of these rows(users).
 * Third, we find users who are similar to a particular user based on past behaviours
 * Finally, we generate recommendations and recommend movies that the user has not experienced before.

## Jester 1.7M jokes ratings dataset

Download the dataset from Kaggle: [Here](https://www.kaggle.com/vikashrajluhaniwal/jester-17m-jokes-ratings-dataset/download)

# Context

Can an automated system recommend a funny joke? Jester is an online joke recommender system developed by Ken Goldberg and the team at UC Berkeley. Users are presented jokes through an HTML client interface and allowed to rate jokes. Once a user rates all jokes in the gauge set, the system recommends new jokes to the user.

# Content

 * The dataset contains over 1.7 million continuous ratings (-10.00 to +10.00) of 150 jokes from 59,132 users.
 * The dataset is collected between November 2006 - May 2009.
 * The complete dataset has two CSV files:-
 * jester_ratings.csv: Each row is formatted as [User ID] [Item ID] [Rating]
 * jester_items.csv: Maps item ID's to jokes
 * The ratings are real values ranging from -10.00 to +10.00.
 * As of May 2009, the jokes {7, 8, 13, 15, 16, 17, 18, 19} are the "gauge set".


## Associated tasks

	IN ORDER:
    - Loading the data into a PySpark Dataframe
    - Splitting into train and test part
    - Fitting an ALS Model
    - Make Predictions
    - Evaluate the model
    - Recommendation jokes
		


## Files and Folders

	- Python notebook template for the assignment
    - README.md


## License
Freely available for research use when acknowledged with the following reference:

[Eigentaste: A Constant Time Collaborative Filtering Algorithm.](http://www.ieor.berkeley.edu/~goldberg/pubs/eigentaste.pdf) Ken Goldberg, Theresa Roeder, Dhruv Gupta, and Chris Perkins. Information Retrieval, 4(2), 133-151. July 2001. 
##ACKNOWLEDGEMENTS
===============================================================================

    The original files have been converted from DAT to CSV format.
    Data Source - http://eigentaste.berkeley.edu/dataset/

## Inspiration
	
Refer to the below research paper to have more ideas about the usefulness of the dataset.

[Eigentaste: A Constant Time Collaborative Filtering Algorithm](https://goldberg.berkeley.edu/pubs/eigentaste.pdf)
