# Drug Sentiment Analysis

### Problem Statement

This is a typical NLP task where we have to predict the sentiment of the users from their reviews.

### Data Description
[Data Source](https://archive.ics.uci.edu/ml/datasets/Drug+Review+Dataset+%28Drugs.com%29)

The dataset provides patient reviews on specific drugs along with related conditions and a 10 star patient rating reflecting overall patient satisfaction.

**Attribute Information:**

1. drugName (categorical): name of drug
2. condition (categorical): name of condition
3. review (text): patient review
4. rating (numerical): 10 star patient rating
5. date (date): date of review entry
6. usefulCount (numerical): number of users who found review useful

### Exploratory Data Analysis

Through our EDA we were able to find some interesting facts about our data. Below are the things that we found 
* The top condition were pain, birth control and high blood pressure.
* Most the conditions have multiple drugs.
* A single drug can be used for multiple conditions.
* The number of reviews has increased in last 3 years.
* As the ratings has increased average yearly rating has decresed.
* Ratings of the users are extreme. They only rate when they find the drug very effective or the drug shows some side effects.
* Most of the usefulCounts are distributed between 0 and 200.

### Data Pre-Processing
* Check null values. And delete them if they are neligible.
* Check for Duplicate records and remove them.
* Check for Noise like special characters or data with no meaning and remove them.

## Pre-Processing Reviews
* **Remove HTML tags**
     * Using BeautifulSoup from bs4 module to remove the html tags. We have already removed the html tags with pattern "64</_span_>...", we will use get_text() to remove the html tags if there are any.
* **Remove Stop Words**
     * Remove the stopwords like "a", "the", "I" etc.
* **Remove symbols and special characters**
     * We will remove the special characters from our reviews like '#' ,'&' ,'@' etc.
* **Tokenize**
     * We will tokenize the words. We will split the sentences with spaces e.g "I might come" --> "I", "might", "come"
* **Stemming**
     * Remove the suffixes from the words to get the root form of the word e.g 'Wording' --> "Word"
     
## TfidfVectorizer (Term frequency - Inverse document frequency)
**TF - Term Frequency** :- \
How often a term t occurs in a document d.\
TF = (_Number of occurences of a word in document_) / (_Number of words in that document_)\
**Inverse  Document Frequency**\
IDF = log(Number of sentences / Number of sentence containing word)\
**Tf - Idf = Tf * Idf**

## Model Building
* Split dependent and independent features.
* Split the data into train and test in 67 : 33 ratio.
* Fit MultinomialNB and RandomForestClassifier on training set, predict and check accuracy.

## Conclusion
After applying the TfidfVectorizer to transform our reviews in Vectors and applying NaiveBayes and RandomForestClassifier we see that RandomForestClassifier outperforms MulinomialNB. We have achieved accuracy of 89.7 % after applying RandomForestClassifier without any parameter tuning. We can tune the parameters of our classifier and improve our accuracy.
