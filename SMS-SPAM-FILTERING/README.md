# SMS-SPAM-FILTERING
Spam filtering/detection is one of the major applications of Machine Learning in the interwebs today. Pretty much all of the major email service providers have spam detection systems built in and automatically classify such mail as 'Junk Mail'.
<br>
<p align="center">
<img src="https://t3n9sm.c2.acecdn.net/wp-content/uploads/2013/08/SMS-spam.jpg" alt="Smiley face" width="300" height="300">    
</p>

## Problem Description:
Our aim is to create a model that can classify dataset SMS messages as spam or not spam, based on the training we give to the model. Usually spam messages have words like 'free', 'win', 'winner', 'cash', 'prize' and the like in them as these texts are designed to catch your eye and in some sense tempt you to open them. Also, spam messages tend to have words written in all capitals and also tend to use a lot of exclamation marks. To the recipient, it is usually pretty straightforward to identify a spam text and our objective here is to train a model to do that for us!

Being able to identify spam messages is a binary classification problem as messages are classified as either 'Spam' or 'Not Spam' and nothing else. Also, this is a supervised learning problem, as we will be feeding a labelled dataset into the model, that it can learn from, to make future predictions.

## Steps:
- Importing Libraries
- Exploring the Dataset
- Exploratory Data Analysis
> * Univariate Analysis
> * Text Analysis 
- Feature Engineering - CountVectorisation
- preprocessing the data before loading into model
- Predictive analysis 
- Conclusion

## Libraries Required:
- Sklearn 
- Matplotlib
- pandas
- numpy
- Seaborn
- Collections

## License & References:
This is an opensource dataset which can be found on UCI Repository. 
```
[1] Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of  California, School of Information and Computer Science. 

[2] http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/
````

## Understanding our Dataset:
We will be using a [The SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection) from the UCI Machine Learning repository which has a very good collection of datasets for experimental research purposes. The direct data link is [here](https://archive.ics.uci.edu/ml/machine-learning-databases/00228/).

The given dataset is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam.
<br>

Here's a preview of the data:
```
ham         Fine if thats the way u feel. Thats the way its gota b
spam	    England v Macedonia - dont miss the goals/team news. Txt ur national team to 87077 eg ENGLAND to 87077 Try:WALES, SCOTLAND 4txt/ú1.20 POBOXox36504W45WQ 16+
ham	    Is that seriously how you spell his name?
ham	    I‘m going to try for 2 months ha ha only joking
ham	    So ü pay first lar... Then when is da stock comin...
ham	    Aft i finish my lunch then i go str down lor. Ard 3 smth lor. U finish ur lunch already?
```
The columns in the data set are currently not named and as you can see, there are 2 columns.

The first column takes two values, 'ham' which signifies that the message is not spam, and 'spam' which signifies that the message is spam.

The second column is the text content of the SMS message that is being classified.

> Instructions:
> * Download the dataset,already given in the repo or use the download link.
> * Import the dataset into a pandas dataframe using the read_table method. Because this is a tab separated dataset we will be using '\t' as the value for the 'sep' argument which specifies this format.
> * Also, rename the column names by specifying a list ['label, 'sms_message'] to the 'names' argument of read_table().
> * Print the first five values of the dataframe with the new column names.
<br>

## Exploratory Data Analysis
- Univairate analysis to analyse the distribution of spam/ham messages. 
- Text analysis (important when dealing with text data): analysing the more frequent words  in spam/ham messages,lengths of most spam messages.
- **Stop words Removal:**
<p align="center">
    <img src ="https://i2.wp.com/xpo6.com/wp-content/uploads/2009/04/stop-words.png?fit=837%2C499" height="300" width="500"><br>src:http://xpo6.com</img>
<p align="center">
    

> * We see that the majority of frequent words in msgs are **'the', 'to', 'a', 'or' and so on. These are called stop words and are a part of english grammer,but they don't really provide any semantic meaning ot msgs,we need to find the actual vocabulary words which contribute to the meaning**</b><p>
> * With stop words we refer to the most common words in a lenguage, there is no simgle, universal list of stop words. <p>
> * <b>Using skearn , we will import the stopwords dataset listed,and remove them from our messages and again analyse the messages</b>

```
from sklearn.feature_extraction import text
stop = text.ENGLISH_STOP_WORDS
#removing all the stop-words from the messages(complete dataset)
data['msgs']=data['msgs'].apply(lambda x: ' '.join([word for word in x.split() if word not in (stop)]))
```
- Presenting a Comparitive text analysis before and after removing stopwords.

## Feature Engineering:
#### **First we need to understand how to Prepare Text Data for Machine Learning**
#### **1. Intution/logic:**
- Text data requires special preparation before you can start using it for predictive modeling.
- The text must be parsed to remove words, called tokenization. 
- Then the words need to be encoded as integers or floating point values for use as input to a machine learning algorithm, called feature extraction (or vectorization).
-scikit-learn library offers easy-to-use tools to perform both tokenization and feature extraction of your text data
- **Since we cannot work with words directly we convert text to fixed-length vectors of numbers - also called Bag-of-words model** 
#### **So Intution is to input Vectors --> model -->output class(spam/ham)**

#### **2. Vectorization:**
- Using BOW model,we assign each word a unique number. 
- Then any document we see can be encoded as a fixed-length vector with the length of the vocabulary of known words. 
- The value in each position in the vector could be filled with a count or frequency of each word in the encoded document.
- An encoded vector is returned with a length of the entire vocabulary and an integer count for the number of times each word appeared in the document.
```
-  eg. The cat ate the mouse 
            attribute name assigned to words : The ->1 , cat ->2 , ate->3 , mouse->4
            considering the above sentence -count the occurance of each word 
            so vector is [2 1 1 1]
```            
-The above logic is applied for complete corpus(text dataset)
-IMP: First stopwords are removed before vectorisation.

(Note: This is just a basic intution for understanding in detail pls refer <html><a href="https://machinelearningmastery.com/prepare-text-data-machine-learning-scikit-learn/"><b>this link</b></a></html>) 

#### **3. Scikit learn Count Vectorizers:** 
- Count Vectorizers provides a simple way to both tokenize a collection of text documents and build a vocabulary of known words, but also to encode new documents using that vocabulary.    
#### Below is an example for reference:
```
from sklearn.feature_extraction.text import CountVectorizer
# list of text documents
text = ["The quick brown fox jumped over the lazy dog."]
# create the transform
vectorizer = CountVectorizer()
# tokenize and build vocab
vectorizer.fit(text)
# summarize
print(vectorizer.vocabulary_)
# encode document
vector = vectorizer.transform(text)
# summarize encoded vector
print(vector.shape)
print(type(vector))
print(vector.toarray())

output:
{'the': 7, 'quick': 6, 'brown': 0, 'fox': 2, 'jumped': 3, 'over': 5, 'lazy': 4, 'dog': 1}
(1, 8)
<class 'scipy.sparse.csr.csr_matrix'>
[[1 1 1 1 1 1 1 2]]


```
- Do the same for all our messages int the dataset.


## Preprocessing data before loading into model:
Now that we have a basic understanding of what our dataset looks like, lets convert our labels to binary variables, 0 to represent 'ham'(i.e. not spam) and 1 to represent 'spam' for ease of computation.

You might be wondering why do we need to do this step? The answer to this lies in how scikit-learn handles inputs. Scikit-learn only deals with numerical values and hence if we were to leave our label values as strings, scikit-learn would do the conversion internally(more specifically, the string labels will be cast to unknown float values).

Our model would still be able to make predictions if we left our labels as strings but we could have issues later when calculating performance metrics, for example when calculating our precision and recall scores. Hence, to avoid unexpected 'gotchas' later, it is good practice to have our categorical values be fed into our model as integers.

> Instructions:
> * Convert the values in the 'label' column to numerical values using map method as follows: {'ham':0, 'spam':1} This maps the 'ham' value to 0 and the 'spam' value to 1.


## Machine learning models:
- Test-train split(use cross-validation)
- **Do a comaprison between each classifier's performance and select the best one**

> * Multinomial NaiveBayes
> * Gaussian NaiveBayes
> * LogisticRegression
> * DecisionTree
> * RandomForestClassifier
> * AdaBoostClassifier

extra:
    can also try any other classifiers.
    Try your models without removing the stop words and compare the results.
    use Gridsearch CV to tune algos

