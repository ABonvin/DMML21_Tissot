# Team Tissot - Data Mining and Machine Learning Project
Unil Kaggle - Detecting the difficulty level of French texts

**Project description:**

Create a model from data with texts that have label difficulty in order to predict the difficulty level of any french text. This is used to help english speaking people that are learning french to find an appropriate text to practise reading. 

**Team Participants**
- Arnaud Bonvin
- Vakisan Tharmakulasinkam
- Tarald Dysthe

Youtube Video: https://www.youtube.com/watch?v=lFMVf7B4Zbo

**Our approach:**

- We did the first part of the notebook as asked
- We used a sequential model from Keras (TF)
- We tokenized the sentences with spacy (feature 1)
- We vectorized the tokens with a count vectorizer (feature 2)
- First feature aggregation
- Test phase
- We added words length and sentences length (in terms of characters) (feature 3)
- We added a counter for the types of words in each sentence (feature 4)
- We aggregated all features
- We tested + validated  the accuracy increase
- We added a Ngram feature
- We tested + validated  the accuracy increase
- We did hyperparameter optimization 
- We tested with several combinations of ngrams (words and character), it worked best with words bigrams

**Summary of results:**

|              | Logistic regression |      kNN  |   Decision Tree  |   Random Forests   |  Keras.Sequential   |
| ------------ | ------------------- | --------- | ---------------- | ------------------ | --------------------| 
| Precision    | 0.4645              | 0.4197    | 0.3048           | 0.4064             | 0.5247              |
| Recall       | 0.4677              | 0.3543    | 0.3031           | 0.4062             | 0.5267              |
| F1-score     | 0.4640              | 0.3450    | 0.3083           | 0.3925             | 0.5236              |
| Accuracy     | 0.4667              | 0.3542    | 0.3005           | 0.4042             | 0.5225              |

