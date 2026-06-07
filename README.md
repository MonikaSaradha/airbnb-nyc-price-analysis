# Airbnb NYC Price Analysis & Regression

## Overview

This project analyzes Airbnb listings in New York City to understand the key factors influencing listing prices and availability.

Using data cleaning, exploratory data analysis (EDA), and regression techniques, the project identifies patterns in pricing and provides actionable insights for hosts and platform strategy.

---

## Dataset

* Source: Inside Airbnb (Kaggle)
* Size: ~49,000 listings, 16 features
* Domain: Short-term rental marketplace

Key variables include:

* price
* neighbourhood_group
* room_type
* minimum_nights
* number_of_reviews
* availability_365
* latitude & longitude

---

## Problem Statement

Airbnb hosts face challenges in:

* setting competitive prices
* improving occupancy
* understanding demand across locations

This project aims to identify the factors that influence pricing and listing performance.

---

## Objectives

* Identify key factors affecting Airbnb prices
* Analyze listing distribution across neighborhoods
* Understand demand patterns across room types
* Evaluate relationships between features using statistical methods

---

## Data Preprocessing

* Removed duplicates to avoid bias
* Handled missing values:

  * Filled missing names with "Unknown"
  * Imputed numerical values using median
* Dropped irrelevant columns (`id`, `host_id`, `last_review`)
* Converted date columns for analysis

---

## Exploratory Data Analysis

### Key Observations

* Most listings are concentrated in Manhattan and Brooklyn
* Price distribution is highly skewed with significant outliers
* Majority of listings are priced below $1000
* High availability listings dominate the dataset

### Visual Analysis

* Heatmap for correlation analysis
* Histogram for price distribution
* Scatter plots for location-based patterns
* Boxplots to detect outliers
* Bar charts for neighborhood comparison

---

## Statistical Analysis

### Correlation

* Weak positive correlation between price and availability (~0.08)
* Negative correlation observed between price and number of reviews

### Regression Analysis

* Linear regression performed between location (latitude) and price
* Results indicate weak but noticeable relationships
* Model highlights that pricing is influenced by multiple interacting factors rather than a single variable

---

## Key Insights

* Manhattan listings have the highest prices and demand
* Entire homes/apartments are priced higher than private/shared rooms
* Listings with fewer minimum nights tend to attract more users
* Location is a strong driver of pricing

---

## Business Recommendations

* Focus on high-demand areas like Manhattan and Brooklyn
* Offer entire homes for higher pricing potential
* Keep minimum stay requirements low to increase bookings
* Maintain competitive pricing based on neighborhood trends
* Improve listing quality and reviews to increase visibility

---

## Limitations

* Dataset limited to NYC
* Weak linear relationships between variables
* Does not include external factors (seasonality, events, etc.)

---

## Future Work

* Build advanced pricing prediction models
* Include more features (amenities, reviews text)
* Apply machine learning models for better accuracy

---

## Tech Stack

* Python (Pandas, NumPy)
* Matplotlib / Seaborn
* Scikit-learn
* Statistical analysis (correlation, regression)

---

## Project Structure

* notebook.ipynb – full analysis and modeling
* data/ – dataset
* README.md – project overview
