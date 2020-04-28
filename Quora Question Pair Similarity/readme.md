<h1> Quora Question Pair Similarity</h1>

Description : Quora is a place to gain and share knowledge about anything. 
It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. 
This empowers people to learn from each other and to better understand the world.

<h2>Problem Statement</h2>

- Identify which questions asked before on quora are duplicates of the questions that have already been asked.
- This can be very useful for providing answers to answers that have already been answered.
- To check weather predicting pair of questions are duplicates or not.
- Source : https://www.kaggle.com/c/quora-question-pairs

<h2>Real world/Business Objectives and Constraints</h2>

- The cost of a mis-classification can be very high.
- You would want a probability of a pair of questions to be duplicates so that you can choose any threshold of choice.
- No strict latency concerns.
- Interpretability is partially important.

<h2>Data Description</h2>
  
- The goal of this competition is to predict which of the provided pairs of questions contain two questions with the same meaning. 
- The ground truth is the set of labels that have been supplied by human experts. 
- The ground truth labels are inherently subjective, as the true meaning of sentences can never be known with certainty.
- Human labeling is also a 'noisy' process, and reasonable people will disagree. 
- As a result, the ground truth labels on this dataset should be taken to be 'informed' but not 100% accurate, and may include incorrect labeling. 
- We believe the labels, on the whole, to represent a reasonable consensus, but this may often not be true on a case by case basis for individual items in the dataset.
  
<h2>Data fields</h2>

- id - the id of a training set question pair
- qid1, qid2 - unique ids of each question (only available in train.csv)
- question1, question2 - the full text of each question
- is_duplicate - the target variable, set to 1 if question1 and question2 have essentially the same meaning, and 0 otherwise. 

<h2>Data Overview</h2>

- All data file sources avilable on - https://www.kaggle.com/c/quora-question-pairs/data
- Data will be in a file Train.csv
- Train.csv contains 5 columns : qid1, qid2, question1, question2, is_duplicate
- Size of Train.csv - 60MB
- Number of rows in Train.csv = 404,290  
  
<h2>Example Data point</h2>
  
- "id","qid1","qid2","question1","question2","is_duplicate"
- "0","1","2","What is the step by step guide to invest in share market in india?","What is the step by step guide to invest in share market?","0"
- "1","3","4","What is the story of Kohinoor (Koh-i-Noor) Diamond?","What would happen if the Indian government stole the Kohinoor (Koh-i-Noor) diamond back?","0"
- "7","15","16","How can I be a good geologist?","What should I do to be a great geologist?","1"
- "11","23","24","How do I read and find my YouTube comments?","How can I see all my Youtube comments?","1"
  
<h2>Machine Leaning Problem Type</h2>
It is a binary classification problem, for a given pair of questions we need to predict if they are duplicate or not.

<h2>Performance Metric</h2>
- Source: https://www.kaggle.com/c/quora-question-pairs#evaluation

- Metric(s):
  
  - log-loss : https://www.kaggle.com/wiki/LogarithmicLoss
  - Binary Confusion Matrix

  
  
  
  
  
