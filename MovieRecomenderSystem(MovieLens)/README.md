# Building a Movie Recommender System using MovieLens Dataset
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

 * Collaborative filtering is makes recommendations on the basis of a combination of factors defining your experience and experiences of other people.
 * First, we make an user vs item matrix.
     * Each row represents an user and each column represents items like movie, product or websites.
 * Second, we compute similarity scores between users.
     * Each row represents an user and each row is a vector.
     * We then compute similarity of these rows(users).
 * Third, we find users who are similar to a particular user based on past behaviours
 * Finally, we generate recommendations and recommend movies that the user has not experienced before.

## MovieLens 1M dataset

# Context

These files contain 1,000,209 anonymous ratings of approximately 3,900 movies 
made by 6,040 MovieLens users who joined MovieLens in 2000.

Users were selected at random for inclusion. All selected users had rated at least 20 movies.  

# Content

No demographic information is included. Each user is represented by an id, and no other information is provided.

The data are contained in 3 files.

RATINGS FILE DESCRIPTION
================================================================================

All ratings are contained in the file "ratings.dat" and are in the
following format:

UserID::MovieID::Rating::Timestamp

- UserIDs range between 1 and 6040 
- MovieIDs range between 1 and 3952
- Ratings are made on a 5-star scale (whole-star ratings only)
- Timestamp is represented in seconds since the epoch as returned by time(2)
- Each user has at least 20 ratings

USERS FILE DESCRIPTION
================================================================================

User information is in the file "users.dat" and is in the following
format:

UserID::Gender::Age::Occupation::Zip-code

All demographic information is provided voluntarily by the users and is
not checked for accuracy.  Only users who have provided some demographic
information are included in this data set.

- Gender is denoted by a "M" for male and "F" for female
- Age is chosen from the following ranges:

    *  1:  "Under 18"
    * 18:  "18-24"
    * 25:  "25-34"
    * 35:  "35-44"
    * 45:  "45-49"
    * 50:  "50-55"
    * 56:  "56+"

- Occupation is chosen from the following choices:

    *  0:  "other" or not specified
    *  1:  "academic/educator"
    *  2:  "artist"
    *  3:  "clerical/admin"
    *  4:  "college/grad student"
    *  5:  "customer service"
    *  6:  "doctor/health care"
    *  7:  "executive/managerial"
    *  8:  "farmer"
    *  9:  "homemaker"
    * 10:  "K-12 student"
    * 11:  "lawyer"
    * 12:  "programmer"
    * 13:  "retired"
    * 14:  "sales/marketing"
    * 15:  "scientist"
    * 16:  "self-employed"
    * 17:  "technician/engineer"
    * 18:  "tradesman/craftsman"
    * 19:  "unemployed"
    * 20:  "writer"


MOVIES FILE DESCRIPTION
================================================================================

Movie information is in the file "movies.dat" and is in the following
format:

MovieID::Title::Genres

- Titles are identical to titles provided by the IMDB (including
year of release)
- Genres are pipe-separated and are selected from the following genres:

    * Action
    * Adventure
    * Animation
    * Children's
    * Comedy
    * Crime
    * Documentary
    * Drama
    * Fantasy
    * Film-Noir
    * Horror
    * Musical
    * Mystery
    * Romance
    * Sci-Fi
    * Thriller
    * War
    * Western

- Some MovieIDs do not correspond to a movie due to accidental duplicate
entries and/or test entries
- Movies are mostly entered by hand, so errors and inconsistencies may exist

## Associated tasks

	IN ORDER:
    - Data_preprocessing 
    - Building the Content_Based and Collaborative Filtering Models
    - Building the SVD model
		
	


## Files and Folders

	- dat folder containing movies.dat, ratings.dat, users.dat and README.md
	- Images folder containing various images
    - Jupyter Notebooks 


## License
The original datasets can be found in http://grouplens.org/datasets/movielens/-

Citation:
F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4, Article 19 (December 2015), 19 pages. 
DOI=http://dx.doi.org/10.1145/2827872

ACKNOWLEDGEMENTS
===============================================================================
Thanks to Shyong Lam and Jon Herlocker for cleaning up and generating the data
set.
## Contact
	
Further information on the GroupLens Research project, including research 
publications, can be found at the following web site:
        
        http://www.grouplens.org/

GroupLens Research currently operates a movie recommender based on 
collaborative filtering:

        http://www.movielens.org/
