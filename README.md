# Word Embedding and Search Query in NLP

In this program, I created a task that ask for a search query and check through twitter tweets that the query exist in one of these tweets. The goal is to use word embedding with a GloVe model ( more about GloVe here : https://nlp.stanford.edu/projects/glove/).

### To create this program, I followed these steps : 

## 1- Preprocessing all these tweets. 
Since they may have unconventional characters (emoticons, likes, hashtags), a specific preprocessing was used.

## 2- Applying word embedding by using the GloVe model
The selected pre-trained model is 'glove-twitter-100'. It is far from being the most performant GloVe but it's a good beginning.

## 3- Applying word embeddings to the search query.
It return vectors representing the mean of each word of the tweet.

## 4- Calculate the cosine similarity and the Euclidean distance between the search query and each tweet of the dataset. 
More about Euclidean distance : https://en.wikipedia.org/wiki/Euclidean_distance
More about Cosine Similarity : https://en.wikipedia.org/wiki/Cosine_similarity
## 5- Return the top 5 tweets with the smallest distance with each calculated method 
We return then 10 tweets : 
- 5 with the smallest euclidean distance with the search query 
- 5 with the closest to 1 cosine similarity with the search query
