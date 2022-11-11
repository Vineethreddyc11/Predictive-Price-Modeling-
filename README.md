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
