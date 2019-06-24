# US-airline-sentiment-analysis

<p align="center"> Kaggel problem/data =https://www.kaggle.com/crowdflower/twitter-airline-sentiment.
    <br> 
</p>

## 🧐 About <a name = "about"></a>
the scope of this projecy to classify the tweets from US airline users to detemined wither it's +ve,-ne or neutral


US airline sentiment analysis using RandomForestClassifier (sklearn)

[avilable data](https://www.kaggle.com/crowdflower/twitter-airline-sentiment)

avilable data as CSV file contain tweet_id, airline_sentiment, name, text, tweet_coord, tweet_created, tweet_location, user_timezone

the most importent airline_sentiment , text(feature)

### Prerequisites
Python==3.0 or higher. 
pandas==23.0. 
nltk==3.3.0. 
scikit-learn==0.19.1. 
recommend to use anaconda3 for dependency installation.

### Installing
recommend to follow the instarction to install [anaconda3](https://www.anaconda.com/distribution/).
After installin run anaconda then create environment and install nltk


### Main Steps:

1. Read data
reading data from CSV using Pandas
download CSV file to the same directory

2. preprocessing
    *remove punc.,special characters,tags and mentions,links, extra spaces
    *lowering all letters 
    *remove stop words( he,she,it,there.this....etc)
    *stemming words to reduce no. of words that give the same meading (added -> add)

3. create bag of words
use the most freq. words as a bag of word then create feacture vector usingt this words get token

4. select model / train (Random Forest)
5. Predicte and Evaluate the Model
               precision    recall  f1-score   support

         -1       0.80      0.90      0.84      2738
          0       0.62      0.46      0.53       947
          1       0.68      0.60      0.64       707

avg / total       0.74      0.75      0.74      4392

