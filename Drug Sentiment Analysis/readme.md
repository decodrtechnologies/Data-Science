# Drug Sentiment Analysis

### Problem Statement

This is a typical NLP task where we have to predict the sentiment of the users from their reviews.

The dataset provides patient reviews on specific drugs along with related conditions and a 10 star patient rating reflecting overall patient satisfaction. We have to create a target feature out of ratings and predict the sentiment of the reviews.

### Data Description
[Data Source](https://archive.ics.uci.edu/ml/datasets/Drug+Review+Dataset+%28Drugs.com%29)

The data is split into a train (75%) a test (25%) partition.

**Attribute Information:**

1. drugName (categorical): name of drug
2. condition (categorical): name of condition
3. review (text): patient review
4. rating (numerical): 10 star patient rating
5. date (date): date of review entry
6. usefulCount (numerical): number of users who found review useful

The structure of the data is that a patient with a unique ID purchases a drug that meets his condition and writes a review and rating for the drug he/she purchased on the date. Afterwards, if the others read that review and find it helpful, they will click usefulCount, which will add 1 for the variable.

### Exploratory Data Analysis

The purpose of EDA is to find out interesting insights and irregularities in our Dataset. We will look at Each feature and try to find out interesting facts and patterns from them. And see if there is any relationship between the variables or not.

Through our EDA we will able to find some interesting facts about our data and features which can be really helpful while building models. 

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

## Parameter Tuning
After building base model,try different set of parameters to increase the accuracy of your model. You can use GridSearchCV or RandomizedSearchCV to get the right set of parameters.

## License
    {Source:

    Surya Kallumadi
    Kansas State University
    Manhattan, Kansas, USA
    surya '@' ksu.edu

    Felix Gräßer
    Institut für Biomedizinische Technik
    Technische Universität Dresden
    Dresden, Germany
    felix.graesser '@' tu-dresden.de
        }
## Citation Request:

Felix Gräßer, Surya Kallumadi, Hagen Malberg, and Sebastian Zaunseder. 2018. Aspect-Based Sentiment Analysis of Drug Reviews Applying Cross-Domain and Cross-Data Learning. In Proceedings of the 2018 International Conference on Digital Health (DH '18). ACM, New York, NY, USA, 121-125. DOI: [Web Link](https://dl.acm.org/doi/10.1145/3194658.3194677)

