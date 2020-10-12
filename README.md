# Tripadvisor_reviews_rating_NLP

## Project Overview

I created a tool that classifies Tripadvisors reviews into three categories: negative, neutral, positive.

*   Created a tool that classifies Tripadvisors reviews into three categories (accuracy: 85%).
*   Data collection on Kaggle website: https://www.kaggle.com/andrewmvd/trip-advisor-hotel-reviews.
*   Exploratory Data analysis using Wordcloud.
*   Text preprocessing: removed punctuations, stemming, word embedding ...
*   Created a simple LSTM model.
*   Testing model for inference on one sentence.


## Code and Resources Used

**Python Version:** 3.7

**Data Collection:** https://www.kaggle.com/andrewmvd/trip-advisor-hotel-reviews

## About the dataset

The dataset contains 20k reviews crawled from Tripadvisor labeled from 1 star to 5 stars. Stop words have already been removed from the reviews. This dataset can be used to predict review rating or to explore key aspects that make hotels good or bad.

## Exploratory Data Analysis

I wanted to use wordcloud to check if there is major differences in terms of frequences of use of words. The major differences between positive and neutral/negatives reviews is the presence of 'n't'. It seems that people mostly use 'n't' to showcase their dissatisfaction. 

![alt text](https://github.com/gaetanlop/Tripadvisor_reviews_rating_NLP/blob/main/images/wordcloud.PNG)
![alt text](https://github.com/gaetanlop/Tripadvisor_reviews_rating_NLP/blob/main/images/ratings_counts.PNG)

## Text preprocessing

First of all, I removed all non alphabetic characters from the reviews, then I applied stemming. After that, I transformed each reviews to a sequence of integers using tokeniser from keras. Then, I used padding to make all sentences same length. Finally, I used word embedding my keras model.

![alt text](https://github.com/gaetanlop/Tripadvisor_reviews_rating_NLP/blob/main/images/examples.PNG)

## Model Building

I created a simple LSTM model.

![alt text](https://github.com/gaetanlop/Tripadvisor_reviews_rating_NLP/blob/main/images/my_model.PNG)

## Model performance

![alt text](https://github.com/gaetanlop/Tripadvisor_reviews_rating_NLP/blob/main/images/classification_report.PNG)
![alt text](https://github.com/gaetanlop/Tripadvisor_reviews_rating_NLP/blob/main/images/confusion_matrix.PNG)

## Productionization and Deployment
Coming Soon!
