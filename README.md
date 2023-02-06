# Sentiment-analysis-of-Amazon-jewelery-reviews
The project is focused on text representations and the use of text classification for sentiment analysis. Sentiment analysis is extensively used to study customer behaviors using
reviews and survey responses, online and social media, and healthcare materials for marketing and costumer service applications. 

## Dataset
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Jewelry_v1_00.tsv.gz

The reviews dataset of jeweleries from Amazon contains many attributes, and in this project we are only interested in star-rating and review_body.

## Data Cleaning
Use some data cleaning steps to preprocess the data:
- convert the all reviews into the lower case.
- remove the HTML and URLs from the reviews
- remove non-alphabetical characters
- remove extra spaces
- perform contractions on the reviews, e.g., won’t → will not. Include as
many contractions in English that you can think of.

## Language Model

- TF-IDF features
- Train a Word2Vec model using the training dataset.

## Method

- Feedforward Neural Networks: a network with two hidden layers, each with 50 and 10 nodes, respectively
- Recurrent Neural Networks: 
 - An RNN cell with the hidden state size of 20. To feed your data into our RNN, limit the maximum review length to 20 by truncating longer reviews and padding shorter reviews with a null value (0). 
 - A gated recurrent unit cell.
