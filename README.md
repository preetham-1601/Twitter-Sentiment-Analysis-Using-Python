# Sentiment Analysis of Tweets using Python

## Introduction

The objective of this project is to perform sentiment analysis on a dataset of tweets using Python, determining the sentiment as positive, negative, or neutral. We aim to build a model that accurately predicts the sentiment conveyed in tweets.

## Data Collection

We collected 8266 tweets using the Twitter API with hashtags related to Clemson University like `#ClemsonTigers`, `#ClemsonGrad`, `#ClemsonFamily`, and `#Clemson`. Due to API call limitations, the analysis was conducted on the first 3000 tweets.

## Data Preprocessing

The raw tweet data underwent preprocessing to eliminate URLs, mentions, hashtags, punctuation, and stop words. We employed the `punkt`, `wordnet`, and `lemmatizers` from the NLTK library to prepare the text for feature extraction.

## Model Architecture

Our model is a sequential neural network with the following layers configuration:
- Embedding Layer
- SpatialDropout1D
- Conv1D
- MaxPooling1D
- Dropout
- Bidirectional LSTM
- GlobalMaxPooling1D
- Dense
- Activation Functions: `ReLU` and `Softmax`

The model was compiled with binary cross-entropy loss and the Adam optimizer.

## Results and Evaluation Metrics

The model achieved:
- Accuracy: 0.708
- Precision: 0.702
- Recall: 0.701
- F1-score: 0.701

A confusion matrix was generated, which helped us evaluate the model's performance further.

## Limitations and Potential Improvements

The use of a larger dataset and fine-tuning hyperparameters could potentially enhance the model's performance. Addressing potential bias in data collection and employing a diverse set of hashtags for tweet extraction could also improve the project outcomes.

## Conclusion

The project demonstrates the feasibility of performing sentiment analysis on tweets using Python and NLP techniques. The model presents a solid foundation for sentiment analysis on social media data, with opportunities for further enhancements.

