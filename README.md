# Fake_News_Classification
This repository contains files for creating fake news classifiers. 

The first contains data preprocessing, EDA, LDA, text-vectorization, and 6 trained models. 
Preprocessing involved replacing null values with blank spaces and ensuring that I was working with a balanced dataset.
For my EDA, I created several visualizations to begin learning about the dataset. The first is a simple bar chart showing the distribution of instances labeled as 'reliable' and 'unreliable,' which shows that it is a balanced dataset with approximately 10,000 instances of each. The second was a pair of wordclouds to highlight the most frequent words for both the real and fake news. These word clouds reveal that there is an apparent difference in the content of articles labeld as real and fake; take, for instanc,e the fact that "Hillary Clinton" appears only in the fake news wordcloud. 
I also created three LDA models. An LDA model with 5 topics was overall the most useful, and shows the frequency of which government-related terms appear in the datset. 
I used scikit-learn's CountVectorizer and Tfidf-Vectorizer to vectorize my text before training my models. For each type of model I created, I trained one on the CountVectorized text and one on the Tfidf-Vectorized text.
I explored three kinds of models: Logistic Regression, Random Forest, and SGD Classifier. Overall, the SGD Classifier saw the best performance. 


The second file uses TensorFlow to create a Dense Sequential Network, a CNN network, a hybrid CNN-RNN, and a Bidirectional LSTM network. I used functions provided by keras and tensorflow to preprocess the text, applying tokenization and padding. Overall, the networks that used LSTM cells saw the best performance (the hybrid CNN-RNN and the Bidirectional LSTM network); however, the Bidirectional LSTM network seemed more prone to overfitting. 
