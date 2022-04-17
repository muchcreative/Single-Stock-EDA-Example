## Single-Stock-EDA
Single Stock EDA Example for Anomaly Detection and Feature Clustering

High volatilities, high kurtosises, and fat-tail distributions are the enemy of stock trading machine learning models. Let's try to analyze these problems and understand how to create features for models to recognize these black-swan like events for a single stock.

I am assuming you already have the OHLCV data for a single stock. If you do not have this data, look into my other repositories for how to build a rotating stock dataset. You will also need market data for part 4 below.

This is an excerpt from a stock machine learning program.

## Breakdown

**1. Standardization Vs Normalization**

Test different ways to standardize vs normalize you stock data

**2. Plotting**

Histograms, QQ-plots, ACF, and PACF plots are your friends. Summarize findings and understand your cutoff for your fat tail distributions

**3. Anomaly Detection and Clustering**

Understanding your data, let's see if we can run gaussian detection or other clustering methods to determine when these events happen. If not can we add any additional features to do so?

**4. How do we use this data beyond what we have?**

How can we apply this information to a more general idea against the stock market itself. Can we create any features from this EDA or at least determine when we should avoid trading if the model is not good enough. How do we go about measuring the success or practicality of these ideas?
