# Movies-Recommendation-Engine

Simply put a Recommendation System is a filtration program whose prime goal is to predict the “rating” or “preference” of a user towards a domain-specific item or item. In our case, this domain-specific item is a movie, therefore the main focus of our recommendation system is to filter and predict only those movies which a user would prefer given some data about the user him or herself.

## What are the different filtration strategies?

![](https://editor.analyticsvidhya.com/uploads/88506recommendation%20system.png)

## Overview

The movies are recommended based on the content of the movie you entered or selected. The main parameters that are considered for the recommendations are the genre, director, and top 3 casts. The details of the movies, such as title, genre, runtime, rating, poster, casts, etc., are fetched from [TMDB](https://www.themoviedb.org/documentation/api). The reviews of each individual movie given by the users are "web-scraped" from the IMDB, and the reviews are subjected to sentiment analysis, where the model predicts whether the review is positive or negative.

## Architecture

![image](https://user-images.githubusercontent.com/64821137/205703620-6a74b310-a026-429a-9473-443ee3731a05.png)

## Similarity Score

**How does it decide which item is most similar to the item user likes(or selects in our case)?** Here comes the similarity scores.
   
It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
## How Cosine Similarity works?

Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.

<p align="center">
  <img src="https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png" />
</p>

More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

## Featured Images

![image](https://user-images.githubusercontent.com/64821137/205706552-933d5d30-f939-487b-8d66-97540c285d66.png)

![image](https://user-images.githubusercontent.com/64821137/205706643-55c8eec2-8624-47e4-8493-d10355363cda.png)

![image](https://user-images.githubusercontent.com/64821137/205706720-0ecf176f-35fe-4a25-b405-8b45380b9238.png)

![image](https://user-images.githubusercontent.com/64821137/205706780-ca1dbc13-87cd-4b80-b803-e75b9e3f5e67.png)




