# Team Tissot - Data Mining and Machine Learning Project
Unil Kaggle - Detecting the difficulty level of French texts

**Project description:**

Create a model from data with texts that have label difficulty in order to predict the difficulty level of any french text. This is used to help english speaking people that are learning french to find a appropriate text to practise reading. 

**Team Participants**
- Arnaud Bonvin
- Vakisan Tharmakulasinkam
- Tarald Dysthe

**Our approach:**

- Tokenized with spacy
- Vectorized the tokens with a count vectorizer
- Test phase
- Added words length + sentences length (in terms of characters) as features
- Test + validation of accuracy increase
- Added n gram features
- Test with several combination of ngrams (words and character), best with words bigrams

**Summary of results:**

|              | Logistic regression |      kNN  |   Decision Tree  |   Random Forests   |  Keras.Sequential   |
| ------------ | ------------------- | --------- | ---------------- | ------------------ | --------------------| 
| Precision    | 0.4645              | 0.4197    | 0.3048           | 0.4064             | 0.5247              |
| Recall       | 0.4677              | 0.3543    | 0.3031           | 0.4062             | 0.5267              |
| F1-score     | 0.4640              | 0.3450    | 0.3083           | 0.3925             | 0.5236              |
| Accuracy     | 0.4667              | 0.3542    | 0.3005           | 0.4042             | 0.5225              |

