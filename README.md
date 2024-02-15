# Project-Multivariate-data-analysis-and-hypothesis-testing

## Description:
This repository contains a project report and code, where I analyze Airbnb data to test hypotheses related to property size, pricing, and their impact on the number of reviews received. The report includes data preprocessing steps, hypothesis testing using linear regression, exploratory data analysis, and comparison of prediction models. The goal is to provide insights into factors that influence the number of reviews for Airbnb listings.

## Overview
This project analyzes Airbnb data to test hypotheses related to property size, pricing, and their impact on the number of reviews received. The report provides insights into factors that influence the number of reviews for Airbnb listings.

## Data Set
The data set used for this analysis is called "clean listing" and is a pandas DataFrame object. Columns with more than 50% missing values are removed, and missing values in review-related fields are filled with zeros. The data is then transformed and converted to floating-point numbers for analysis.

## Hypotheses Testing
1. Larger properties should receive more reviews.
   - Method: Linear regression was used to model the connection between the number of bedrooms, accommodations, and reviews per month. The results did not support the assumption that larger properties receive more reviews.

2. Higher-priced listings will receive fewer reviews.
   - Method: Properties were grouped based on location and size, and the mean reviews per month were compared for underpriced and overpriced listings. The results contradicted the hypothesis when considering location and size together but supported it when considering them individually.

## Predictive Model Comparison
- Linear Regression: R square value of 0.35, MSE of 0.74.
- Lasso Regression: R square value of 0.23, MSE of 0.84.
- Random Forest Regression: R square value of 0.52, MSE of 0.61.

## OLS Regression Findings
Factors significant for predicting monthly reviews:
- host_response_time[T.3]
- host_is_superhost[T.1]
- host_identity_verified[T.1]
- property_type[T.13]
- property_type[T.16]
- instant_bookable[T.1]
- bedrooms
- host_acceptance_rate
- host_total_listings_count
- accommodates
- price
- review_scores_checkin
- review_scores_communication
- review_scores_location
- review_scores_value

## Conclusion
The analysis provides valuable insights into the factors influencing the number of reviews for Airbnb listings, highlighting the importance of pricing, property size, and location. Further research could explore additional variables and refine prediction models for more accurate results.
