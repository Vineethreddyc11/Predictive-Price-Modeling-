# Predictive-Price-Modeling-


The project aimed at predicting the price of an Airbnb listing given a number of features. The project involved exploratory data analysis, data pre-processing, feature selection, Model Fitting, Model Comparison and deploying the containerised Webapp on AWS using CI/CD Pipeline.

## Project Goals and Objectives

**Problem:** Currently there is no convenient way for a new Airbnb host to decide the price of his or her listing. New hosts must often rely on the price of neighbouring listings when deciding on the price of their own listing.

**Solution:** A Predictive Price Modelling tool whereby a new host can enter all the relevant details such as location of the listing, listing properties, available amenities etc and the Machine Learning Model will suggest the Price for the listing. The Model would have previously been trained on similar data from already existing Airbnb listings.

## Project Overview

- **Exploratory Data Analysis:** Explore the various features, their distributions using Histograms and Box-plots

- **Pre-processing and Data Cleaning:** Normalisation, filling missing values, encoding categorical values.

- **Feature Selection:** Study the correlation with response variable (Listing Price) and determine which features are most useful in predicting the price.

- **Model Fitting and Selection:** Training different models, tuning hyper-parameters and studying Model performance using Learning Curve.

- **Model Serving:** Using FLASK to deploy and serve Model predictions using REST API.

- **Container:** Using Docker to containerise the Web Application.

- **Production:** Using AWS CI/CD Pipeline for continuous integration and deployment.

## About Dataset

The Dataset used in this project was obtained from public.opendatasoft.com. There are a total of 494,954 records each of which contains details of one Airbnb listing. The total size of dataset is 1.89 GB.

The dataset has a large number of features which can be categorised into following types,

- **Location related:** Country, City, Neighbourhood

- **Property related:** Property Type, Room Type, Accommodates, Bedrooms, Beds, Bed Type, Cancellation Policy, Minimum Nights
 
- **Booking Availability:** Availability 30, Availability 60, Availability 90, Availability 365

- **Reviews related:** Number of Reviews, Reviews per Month, Review Scores Rating, Review Scores Accuracy, Review Scores Cleanliness, Review Scores Checkin, Review Scores Communication, Review Scores Location, Review Scores Value

- **Host related:** Host Since, Host Response Time, Host Response Rate, Calculated host listings count, Host Since Days, Host Has Profile Pic, Host Identity Verified, Is Location Exact, Instant Bookable, Host Is Superhost, Require Guest Phone Verification, Require Guest Profile Picture, Requires License

- **Amenities:** TV, Wireless Internet, Kitchen, Heating, Family/kid friendly, Washer, Smoke detector, Fire extinguisher, Essentials, Cable TV, Internet, Dryer, First aid kit, Safety card, Shampoo, Hangers, Laptop friendly workspace, Air conditioning, Breakfast, Free parking on premises, Elevator in building, Buzzer/wireless intercom, Hair dryer, Private living room, Iron, Wheelchair accessible, Hot tub, Carbon monoxide detector, 24-hour check-in, Pets live on this property, Dog(s), Gym, Lock on bedroom door, Private entrance, Indoor fireplace, Smoking allowed, Pets allowed, Cat(s), Self Check-In, Doorman Entry, Suitable for events, Pool, Lockbox, Bathtub, Room-darkening shades, Game console, Doorman, High chair, Pack ’n Play/travel crib, Keypad, Other pet(s), Smartlock

The price of the listing will serve as labels for the regression task. The goal of this project would be to predict these price of the listings.

## Exploratory Data Analysis

To get a better insight into where the listings are located, the number of listings in various cities and countries are plotted in the figure below. In the given dataset, United States has the most number of listings followed by European countries and Australia. In terms of cities, Paris, London, New York, Berlin, Los Angeles are some of the cities with most number of listings.

Airbnb offers three types of listings,

- **Entire home/apartment**
- **Private Room**
- **Shared Room**

Entire home is by far the most popular type of listing offered followed by Private Rooms and then a small share of the total listings are shared rooms.
