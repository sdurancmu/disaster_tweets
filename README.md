# Disaster Tweets Prediction: NLP, Deep Learning, LSTM

### Project Background

Twitter has become an important communication channel in times of emergency.
The ubiquitousness of smartphones enables people to announce an emergency they’re observing in real-time. Because of this, more agencies are interested in programatically monitoring Twitter (i.e. disaster relief organizations and news agencies).

But, it’s not always clear whether a person’s words are actually announcing a disaster.  A twitter user may use the word 'ablaze" to describe an amazing view of the sky or a horrific forest fire.   

There is an opportunity to use machine learning to predict whether a tweet is discussing a disaster or not.  Lucky for me, Kaggle has compiled a labeled dataset of disaster and non-disaster tweets that is ready for some supervised learning.   

### Approach

I used a bi-directional LSTM augemented by pre-trained word emeddings as my primary means to predict whether a tweet is about a disaster.  In the disaster_tweets_nb.ipynb file you can see the following steps in my process:

1) EDA
2) Pre-processing tweets (removing stopwords, spell checking, removing punctuation, etc.)
3) Prep data for LSTM Model (tokenizing tweets, importing word emdeddings)
4) Define LSTM model (create model structure and define hyperparameters)
5) Train/Tune Model 
6) Make Predictions on Kaggle dataset

### *Update

After experimenting with a new approach utilizing BERT (via huggingface transformer package), I have improved my score (0.81887) and ranking (824) in the kaggle competition, with no changes to preprocessing. Code in disaster_tweets_nb_BERT.ipynb.

### TO DO

1) Improve preprocessing of tweets.  For example, saw others mapping common shorthand like 'lol' to 'laugh out loud', etc

