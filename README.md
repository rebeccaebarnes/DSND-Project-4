# Predict Availability for Seattle Airbnb
This project was completed as part of the course requirements of Udacity's [Data Scientist Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025) certification.

## Overview
The project used a [Kaggle dataset](https://www.kaggle.com/airbnb/seattle) containing data about listings Seattle Airbnb listings during 2016.

The project followed the CRISP-DM method of data exploration's six steps of:
1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Deployment

The goal of the project was to predict and determine the important features in predicting availability based on the following business cases:

_You stayed at a great airbnb location for your last vacation. You are thinking of going away in a few months, what is the likelihood that the host will have listed the place as available?_

OR

_You are scrolling through the airbnb site looking at different sites without having selected a date. Is there information that you use from this front page that may indicate that it is more likely that the host has listed the site as available for the dates you have in mind?_

To walk-thru the full project, check out the [notebook](https://github.com/rebeccaebarnes/DSND-Project-4/blob/master/seattle_airbnb_exploration.ipynb).

To read the blog post associated with the article, you can go [here](https://medium.com/@rebeccaebarnes/this-will-make-you-think-like-a-supercomputer-39898ab9eaf8).

## Technologies Used
- Python
- Libraries: sklearn, pandas, numpy, matplotlib, seaborn, nltk
- Jupyter Notebook

## Key Findings
Using a Random Forest Classifier, it was possible to predict whether a host made a listing available with approximately 90% accuracy using only information that is available when browsing the listings and the day of the week for which to predict.

!['Enter Message'](airbnb_listing.PNG)

The most important features in the classifier were price, number of reviews, the day of the week, number of bedrooms and whether the host is a superhost. Whether the listing name contained the words _heart_ and _bright_ were the next two most important features.
