# text-classification
The task of this assignment is to train and evaluate various classifiers to distinguish spam from non-spam (ham) emails using the Enron dataset. The approach is a supervised one due to the fact we already know the category (spam/ham) where an email belongs.

Emails are modeled using two types of text representation. The first one is a bag-of-words model weighted by TC (term count) or TF-IDF (term frequency - inverse document frequency). The second, centroids-of-word-embeddings represents an email by averaging the word embeddings of all words or by summing weighted word embeddings of all words, where the weight of a word is given by TF-IDF.

We choose to experiment with five algorithms: Logistic Regression (LR), SGD, Naïve Bayes (NB), Nearest Neighbors (KNN) and SVM. Also a baseline Dummy classifier predicting always the majority class (ham) is used for comparison.

So in this work we make 25 experiments in total (5 methods x 5 classifiers). A summarization of our system and inner-code working is shown in following figure:
![alt text](https://github.com/soutsios/text-classification/blob/master/inner-working.png)
