# Twitter User Gender Classifier using NLP
The detailed work can be found on the gender_classifier_nlp.ipynb file.

## Background 

Due to the advancements in the field of Natural Language Processing(NLP), the advanced techniques can now be employed in varied use cases one of the significant uses being parsing blocks/paragraphs of text and deriving relevant information from them.
One such use case is determining/predicting the gender of the individual from his/her messages or in our case tweets.

## Twitter User Gender Classification Dataset

**Context**

This data set was used to train a CrowdFlower AI gender predictor. [You can read all about the project here](https://www.crowdflower.com/using-machine-learning-to-predict-gender/). Contributors were asked to simply view a Twitter profile and judge whether the user was a male, a female, or a brand (non-individual). The dataset contains 20,000 rows, each with a user name, a random tweet, account profile and image, location, and even link and sidebar color.

**Content**

The dataset contains the following fields:

 * unitid: a unique id for user
 * _golden: whether the user was included in the gold standard for the model; TRUE or FALSE
 8 unitstate: state of the observation; one of finalized (for contributor-judged) or golden (for gold standard observations)
 * trustedjudgments: number of trusted judgments (int); always 3 for non-golden, and what may be a unique id for gold standard observations
 * lastjudgment_at: date and time of last contributor judgment; blank for gold standard observations
 * gender: one of male, female, or brand (for non-human profiles)
 * gender:confidence: a float representing confidence in the provided gender
 * profile_yn: "no" here seems to mean that the profile was meant to be part of the dataset but was not available when contributors went to judge it
 * profile_yn:confidence: confidence in the existence/non-existence of the profile
 * created: date and time when the profile was created
 * description: the user's profile description
 * fav_number: number of tweets the user has favorited
 * gender_gold: if the profile is golden, what is the gender?
 * link_color: the link color on the profile, as a hex value
 * name: the user's name
 * profileyngold: whether the profile y/n value is golden
 * profileimage: a link to the profile image
 * retweet_count: number of times the user has retweeted (or possibly, been retweeted)
 * sidebar_color: color of the profile sidebar, as a hex value
 * text: text of a random one of the user's tweets
 * tweet_coord: if the user has location turned on, the coordinates as a string with the format "[latitude, longitude]"
 * tweet_count: number of tweets that the user has posted
 * tweet_created: when the random tweet (in the text column) was created
 * tweet_id: the tweet id of the random tweet
 * tweet_location: location of the tweet; seems to not be particularly normalized
 * user_timezone: the timezone of the user

**Acknowledgements**

Data was provided by the [Data For Everyone Library](https://www.crowdflower.com/data-for-everyone/) on [Crowdflower](https://www.crowdflower.com/).

Data for Everyone library is a collection of open data jobs that have come through their platform. They're available free of charge for the community, forever.

**Inspiration**

Here are a few questions you might try to answer with this dataset:

 * How well do words in tweets and profiles predict user gender?
 * What are the words that strongly predict male or female gender?
 * How well do stylistic factors (like link color and sidebar color) predict user gender?

## Associated tasks

	IN ORDER:
    -Data Inspection
    -Regular Expressions, Stopwords and Lemmatization
    -Train and Test Split
    -Naive Bayes Algorithm
    -Random Forest Algorithm


## Files

	- README.md
	- gender-classifier-DFE-791531.csv : Data file
    - gender_classifier_nlp.ipynb: Jupyter Notebook file.


## License

[CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/)
