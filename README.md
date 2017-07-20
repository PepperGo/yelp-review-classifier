# Yelp Review Classification

This is the code for a classifier that predicts ratings based on text from Yelp reviews.

## Overview

I built a multinomial naive bayes classifier that rates reviews, using the [Scikit-learn](http://scikit-learn.org/stable/) library. Text processing was done with the help of the [NLTK](http://www.nltk.org/) library. The input is text, and the output is a numeric value of either 5 (high rating) or a 1 (low rating).

The model was able to classify text with a **92.3%** accuracy.

## Dependencies

- numpy
- pandas
- scikit-learn
- nltk

Install dependencies using [pip](https://pip.pypa.io/en/stable/).

## Dataset

The dataset was taken from the [Kaggle Yelp Business Rating Prediction competition](https://www.kaggle.com/c/yelp-recsys-2013). The particular subset I used (input/yelp.csv) contains 10,000 observations (reviews) and 10 attributes.


| Column  | Definition |
| ------------- | ------------- |
| business_id  | ID of the business being reviewed  |
| date  | The date on which the review was posted  |
| review_id  | ID of the review  |
| stars  | Rating given for the busines  |
| text  | Review text  |
| type  | Type of text (all are "review" in this dataset)  |
| user_id  | ID of the user  |
| cool/useful/funny  | Comments given by other users on the review  |

## Text pre-processing

List of techniques used for text pre-processing:

- stopword removal
- vectorisation

## Usage

Run the Jupter notebook on a localhost server by typing `jupyter notebook`.
