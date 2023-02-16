# twitter-climate-change-data-analysis
Sentiment Analysis on Twitter Climate Change Data

Climate change is a growing concern all over the
world. It is important to take steps now so that
eventual consequences such as: decrease in the
quality of life, increase in diseases, and mass
migrations can be prevented. Monitoring the content and number of tweets
on climate change over time can help us
understand the concerns of the people and
which topics are mostly discussed. In this project, two approaches: supervised
learning with different implementations and
classification with a pretrained model were used
to predict the sentiment expressed in tweets
collected over a period of 10 years. 

## Dataset collection
The data used for the project was collected using
the Twitter API. The tweets were collected for a
period of 10 years starting from 1st January 2013
to 15th October 2022. Since historical data was
required, the
Academic research access was required. The following was used as the query for
the search:
"climate change OR global warming OR #climatech
ange OR #globalwarming lang:en"
For each year, around 5000 tweets were collected
resulting in a total of around 50,000 tweets.
Different details about the tweets were collected
such as: author id, creation time, geo location id,
tweet id, language, like count, reply count and
retweet count along with the actual tweet text.

## Labeled dataset
For training the supervised models, we also require
a labeled dataset. For this purpose, I used the
Twitter Climate Change Sentiment Dataset from [Kaggle](https://www.kaggle.com/datasets/edqian/twitter-climate-change-sentiment-dataset?resource=download).

## Data Preprocessing
For the preprocessing, the following steps were
taken:
* Changing the tweet text to lowercase
* Removing mentions from the tweet
* Removing hashtags from the tweet
* Removing URLs from the tweet
* Removing retweet indication from the
tweet
* Removing special characters from the
tweet

## Machine Learning Model Training and Prediction
The following machine learning algorithms were used for training different models and tested.
* Random Forest Classification
* kNN Classification
* Logistic Regression
* Linear Support Vector Machine Classification
* VADER (pretrained)
* Extra Trees Classifier

## Further Analysis
For further analysis, key words from the collected tweets data were identified. Also, topic modeling with LDA and retweet network analysis were performed.
