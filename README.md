# Sentiment_Analysis
This ia a Kaggle challenge which is a classification problem for text data that classify phrases on a scale of five values: negative, somewhat negative, neutral, somewhat positive, positive. Obstacles like sentence negation, sarcasm, terseness, language ambiguity, and many others make this task very challenging

You can find this challenge [here](https://www.kaggle.com/c/sentiment-analysis-on-movie-reviews/overview)

# Dataset
The dataset is comprised of tab-separated files with phrases from the Rotten Tomatoes dataset. The train/test split has been preserved for the purposes of benchmarking, but the sentences have been shuffled from their original order. Each Sentence has been parsed into many phrases by the Stanford parser. Each phrase has a PhraseId. Each sentence has a SentenceId. Phrases that are repeated (such as short/common words) are only included once in the data.

train.tsv contains the phrases and their associated sentiment labels. We have additionally provided a SentenceId so that you can track which phrases belong to a single sentence. test.tsv contains just phrases. You must assign a sentiment label to each phrase. The sentiment labels are:

0 - negative 1 - somewhat negative 2 - neutral 3 - somewhat positive 4 - positive

# Implementation

As usually, I do some text preprocessing (words lower case, removing punctuation, removing stopwords, Lemmatization, TfidfVectorizer), then try with three different model: linear SVM, GRU and LSTM.

![](https://github.com/tuananh0305/Sentiment_Analysis/blob/master/images/loss.png)

![](https://github.com/tuananh0305/Sentiment_Analysis/blob/master/images/metrics.png)
