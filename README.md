# yelp-reviews-sent-classifier
## Description
The objective of the task was to develop a sentiment classifer using a dataset that contains 650k yelp reviews. The dataset has sentiment labels varying from level 1 to level 5 with level 1 being strong negative to level 5 being strong positive and level 3 being neutral. Text preprocessing was done on the yelp reviews, followed by feature extraction to convert the text to a numerical representation that can be used in statistical models. Statistical models were then used to develop a classifer to predict the sentiment label of the yelp reviews in the testing dataset.

Several preprocessing steps including case normalization, removing non alpha-numeric words, removing stop words, stemming and lemmatization were attempted. Removing stop words decreased the accuracy of the statistical models. Stemming and lemmatization did not improve the prediction accuracy and were taking too much time for computation. Hence, the final preprocessing steps done for the yelp reviews were case normalization and removing non-alphanumeric words. 

Unigram and Bigram features were extracted from the reviews. Term Frequency (TF) and Term Frequency Inverse Document Frequency (TF-IDF) representations were attempted; TF-IDF representation yielded a slightly higher accuracy in the statistical models.The number of features used in the final classifer were 10,000; this was finalised after experimenting with different number of features.  

Several statistical models including multinomial Naive Bayes, Multinomial Logistic Regression and Linear Support Vector Classifier were used to develop the sentiment classifer. Multinomial Logistic Regression was found to have the highest predictive power for this dataset and used in the final classifer.

*Note that this code only contains the preprocessing steps, feature extraction and statistical model for the final classifer.*

## Packages required
* pandas 
* nltk
* numpy
* sklearn
* matplotlib
