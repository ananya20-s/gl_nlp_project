## Sentiment Analysis and Text Summarization of News articles using NLP techniques
![np3](https://github.com/user-attachments/assets/398b6296-8e9d-4de6-8758-65a6bd4fba94)



### Description
This project was developed as part of the Post Graduation Program in AI/ML.
The aim is to develop solution that can use News articles content and predict its sentiment(positive/negative/neutral).
The same is used to analyse its impact on stock prices of a particular company.
The key events are summarised for each week for both positive and negative sentiments.


### Features
 - Build a ML classifier that can identify the sentiments using embeddings and any one traditional ML method
 - Identify the best model and publish metrics on the test set
 - Summarise news events on a weekly basis by identifying top 3 events for positive and negative news.
 

### Dataset
The new articles dataset with sentiment labels is provided as part of the course



### Results

 - Perform text preprocessing using Regular expressions and NLTK
 - Obtain embeddings for Word2Vec, GloVe and Sentence Transformers and fit all into different Random Forest Classifiers
 - Given data imbalance, AUC score and F1 Score was considered and RF trained on Transformer embeddings RF model performed best
 - After Hyper param tuning, model had AUC score of 60% and F1 Score of 30% 
 - For summarization, used a HuggingFace model to obtain key events in JSON format
 - Used json_normalise to create a dataframe to capture the summary


### Technologies Used
- **Tools:** Python, Google Colab
- **Libraries:** Pandas, Numpy, Scikit learn,Matplotlib, PyTorch, Transformers, Word2Vec, Glove


### Next Steps

 - For Sentiment Analysis, Model performance is satisfactory but can be improved by training the classifier on a larger dataset
 - For Text Summarization, can experiment with other HuggingFace models (BERT/LLama, etc)
