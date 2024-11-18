Overview
This project aims to predict the likelihood of an Airbnb property being booked. The goal is to identify key features that influence booking decisions and use them to build a predictive model. This effort involves extensive feature engineering, data integration, and model development to provide insights into what makes an Airbnb more likely to be booked.

Features of the Project
Feature Engineering
The foundation of the model lies in creating new features to enhance predictive power. Key features include:

Duration of Service: Calculated by dividing the total number of reviews by reviews per month, giving insight into how long the Airbnb has been operational.
Price per Minimum Nights: Provides a rate-based metric for affordability.
Price Competitiveness: Compares an Airbnb's price against the neighborhood average, categorizing properties as "competitive," "not competitive," or "equal."
Proximity to Subway Stations: Uses NYC subway data to calculate the number of stations within 0.5 miles of an Airbnb, considering accessibility as a critical factor.
Distance to Tourist Attractions: Measures proximity to major attractions, emphasizing location desirability.
Data Challenges
An attempted integration with restaurant datasets was abandoned due to computational inefficiencies in calculating distances between large datasets.

Model Highlights
The model predicts three categories of booking likelihood:

Highly Likely to Be Booked:
Properties with high reviews and good ratings.
Affordable prices (e.g., below $200 per night).
Located near attractions and multiple subway stations.
Primarily in Manhattan.
Likely to Be Booked:
Similar criteria but located in boroughs other than Manhattan.
Unlikely to Be Booked:
Properties with low ratings, long minimum stays, or inconvenient locations.
Properties not fitting these categories are classified as "other," though this category is rare.

