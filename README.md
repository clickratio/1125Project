# 1125Project

Introduction
The purpose of this project is to investigate the possilibity of implementing early-stage prevention and recommendation based on user post sentiments trending towards specific issues such as depression or suicides.


Directory and Files:
Pickle - Model data repository
data - raw training data (.csv)
training - codes for model building (.ipynb)
PythonGUI.ipynb - Main application, a simple GUI that allows for text input and prediction/recommendation
PythonGUI_LSTM.ipynb - Testing application for LSTM model. Model not included thus will very likely not work.

Data:
training.1600000.processed.noemoticon.csv
Tweets extracted using the twitter API . The tweets have been annotated (0 = negative, 2 = neutral, 4 = positive) and they can be used to detect sentiment analysis. Contains 1,600,000 datapoints
Source - https://www.kaggle.com/datasets/kazanova/sentiment140

Suicide_Detection.csv
A collection of posts from "SuicideWatch" and "depression" subreddits of the Reddit platform. Collected using Pushshift API. Date Range are as follows: "SuicideWatch" from Dec 16, 2008(creation) till Jan 2, 2021. "depression" posts were collected from Jan 1, 2009, to Jan 2, 2021. The entire .csv contains 232,074 datapoints
Source - https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch

rec.csv
simple self made recommendation list

Training:
Sentiment.ipynb
Sentiment analysis training, codes are adapted from kaggle source with very slight changes, thus credit goes to kaggle user NIKIT PERIWAL
Credit and Source: https://www.kaggle.com/code/stoicstatic/twitter-sentiment-analysis-for-beginners

DepSentiment.ipynb
Mood analusis training, due to testing various preprocessing, vectorization, and model building, its a compilation fo best practices from sentiment analysis training and few other sources included below.
Credit and Source:
https://www.kaggle.com/code/abhijitsingh001/suicidal-thought-detection
https://www.kaggle.com/code/nouranmuhammad/suicide-detection-using-reddit-data

suicide_detection_using_reddit_data.ipynb
ensemble learning trial (to test for differences in model), model straight from kaggle
Credit and Source: https://www.kaggle.com/code/nouranmuhammad/suicide-detection-using-reddit-data

Main Application:
Contains snipples of training codes, operation should be self explanatory. If there is an error, uncomment the "del app".
