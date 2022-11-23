# Sentiment-analysis-on-tweet

It is a Natural Language Processing Problem where Sentiment Analysis is done by Classifying the Positive tweets from negative tweets by machine learning models for classification,  text mining, text analysis, data analysis and data visualization

# Introduction

Natural Language Processing (NLP) is a hotbed of research in data science these days and one of the most common applications of NLP is sentiment analysis. From opinion polls to creating entire marketing strategies, this domain has completely reshaped the way businesses work, which is why this is an area every data scientist must be familiar with.

Thousands of text documents can be processed for sentiment (and other features including named entities, topics, themes, etc.) in seconds, compared to the hours it would take a team of people to manually complete the same task. 

We will do so by following a sequence of steps needed to solve a general sentiment analysis problem. We will start with preprocessing and cleaning of the raw text of the tweets. Then we will explore the cleaned text and try to get some intuition about the context of the tweets. After that, we will extract numerical features from the data and finally use these feature sets to train models and identify the sentiments of the tweets.

This is one of the most interesting challenges in NLP so I’m very excited to take this journey with you!

# Understand the Problem Statement

Let’s go through the problem statement once as it is very crucial to understand the objective before working on the dataset. The problem statement is as follows:

The objective of this task is to detect the feeling of a tweet. For the sake of simplicity, we say a tweet has positive feeling if it has a happy sentiment associated with it. So, the task is to classify positive or negetive tweets from eachother.

Formally, given a training sample of tweets and labels, where label ‘1’ denotes the tweet is positive and label ‘0’ denotes the tweet is negative, our objective is to predict the labels on the given test dataset.

Positive tweet example:'#FollowFriday @France_Inte @PKuchly57 @Milipol_Paris for being top engaged members in my community this week :)'.

negative tweet example: ‘Everything in the kids section of IKEA is so cute. Shame I'm nearly 19 in 2 months :(‘.


# Tweets Preprocessing and Cleaning

Imagine you are searching for a document in this office space. In which scenario are you more likely to find the document easily? Of course, in the less cluttered one because each item is kept in its proper place. The data cleaning exercise is quite similar. If the data is arranged in a structured format then it becomes easier to find the right information.

The preprocessing of the text data is an essential step as it makes the raw text ready for mining, i.e., it becomes easier to extract information from the text and apply machine learning algorithms to it. If we skip this step then there is a higher chance that you are working with noisy and inconsistent data. The objective of this step is to clean noise those are less relevant to find the sentiment of tweets such as punctuation, special characters, numbers, and terms which don’t carry much weightage in context to the text.

In one of the later stages, we will be extracting numeric features from our Twitter text data. This feature space is created using all the unique words present in the entire data. So, if we preprocess our data well, then we would be able to get a better quality feature space.

To shet light on cleaning data, let's see an example:

Raw tweet: "Thank you for your support :), won't forget http://t.co/ihELksfJjT,@%%*"
Cleaned tweet: ['thank', 'support', 'positiveemoji', 'not_forget']

# Results
We have trained "Logistic Regression" and "Naive Bayes" methods and obtained th following results:

![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)

![Logistic Regression Confusion Matrix](https://github.com/KamalBarati/Sentiment-analysis-on-tweet/blob/main/Logistic Regression confusion matrix.png?raw=true)

![Naive Bayes Confusion Matrix](https://github.com/KamalBarati/Sentiment-analysis-on-tweet/blob/main/Naive Bayes confusion matrix.png?raw=true)


# End Notes

In this article, we learned how to approach a sentiment analysis problem. We started with preprocessing and exploration of data. Then we extracted features from the cleaned text using Bag-of-Words and TF-IDF. Finally, we were able to build a couple of models using both the feature sets to classify the tweets.

We investigate the most frequent word in positive tweeys which is happy symbol ( like "(:" ), and the the most frequent word in negative tweeys which is sad symbol ( like "):" ). Additionaly, we finds the importance of claning data for sentiment analysis on tweets.
