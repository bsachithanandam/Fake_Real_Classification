# Fake review Classification

Experimented various traditional machine learning and deep learning models to classify reviews into fake and real. The models are trained using custom dataset.

For traditional machine learning models, features like average word count, average sentence count, sentiment etc are extracted from the reviews. Sentiment is calculated as a weighted average of sentiment of each sentence. The sentiment of each sentence is extracted using DistilBERT.

For deep learning models, the word embeddings are extracted from BERT and these word embeddings are used to train Feed Forward Network. For LSTM and Bi-LSTM, the reviews are passed into the network just like that. The model which is a combination of BERT and Feed Forward Network has the highest accuracy of 96% amoung deep models and XGBoost has the highest accuracy of 83%.
