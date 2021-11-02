# Task-20-capstone-3
This Capstone Project is about a basic form of Natural Language Processing (NLP) called Sentiment Analysis. 


This task will be broken down into the following steps:
(1) Get the dataset
(2) Preprocessing the Data
(3) Build the Model
(4) Train the model
(5) Test the Model
(6) Predict Something

1. Get the dataset
For this task, we will be using a small portion of the Multi-Domain Sentiment
Dataset, which contains product reviews from Amazon. The full dataset contains
reviews for products under the categories: kitchen, books, DVDs, and electronics,
but we will only be looking at reviews for the book category.

2. Preprocessing the Data
In order to feed this data into our network, all input reviews must have the same
length. Since the reviews differ heavily in terms of lengths, we either need to trim
or pad the reviews so that they are the same length. For this task, we will set the
length of reviews to the mean length, which is around 4 words. If reviews are
shorter than 4 words we will need to pad them with zeros, if they are longer than 4
words we will trim them to this length by cutting off any words after this. Keras
offers a set of preprocessing routines that can do this for us. In order to pad our
reviews, we will need to use the pad_sequences function.

3. Build the Model
This network has the following architecture:
  (1). Embedding layer
  (2). SpatialDropout1D(0.2)
  (3). BatchNormalization()
  (4). LSTM(32)
  (5). Dense(2, activation='softmax')

5 and 4 Test the Model + Train the model
here the model will be traind and tested with diffrent out put dimentions of 10,25,50,100 and the one with the best score will be selceted as the final model 

6. Predict Something
Finally, we will use our model to predict something with the text provided 
  
