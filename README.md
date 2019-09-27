# YelpReviews

This project leverages concepts of Natural Language Processing (NLP) to calculate word sentiment level based on user reviews from Yelp.

The purpose of this analysis is to calculate word sentiment level based on the average star rating (out of 5) of reviews in which each word appears.  The data source, `yelp_academic_dataset_review_small.json` (too large to be uploaded to this repository), contains a subset of 156,602 reviews from Yelp's open dataset.  In this program, the NLTK module is used to tokenize reviews by word, then subsequently lemmatize each of them.  Words are filtered by the NLTK words corpus (234,377 frequently used words), and the stopwords (NLTK stopwords corpus, 127 words) are removed.  The reviews then demonstrate 28,155 unique words.  The 500 most negative and 500 most positive reviews are written to a CSV, `words_sentiment_level.csv`.
