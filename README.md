## Single-Stock-EDA

**STILL UPLOADING AND CLEANING UP THIS REPO**

Single Stock EDA Example for Anomaly Detection and Feature Clustering

High volatilities, high kurtosises, and fat-tail distributions are the enemy of stock trading machine learning models. Let's try to analyze these problems and understand how to create features for models to recognize these black-swan events for a single stock.

I am assuming you already have the adjusted OHLCV data for a single stock. If you do not have this data, look into my other repositories for how to build a rotating stock dataset. You will also need market data for part 4 below.

This is an excerpt from one of my stock machine learning programs.

## Breakdown

**1. Standardization Vs Normalization**

Test different ways for standardizing vs normalizing your stock data.

**2. Plotting**

Histograms, QQ-plots, ACF, and PACF plots are your friends. Summarize findings and understand your cutoff to identify your fat-tail distributions.

**3. Brainstorming for Outlier Handling**

Check discretization, winsorization, or filling effects.

**4. Anomaly Detection and Clustering**

Understanding your data, let's see if we can run gaussian detection or other clustering methods to determine when these events happen. If not can we add any additional features to do so?

**5. How do we use this data beyond what we have?**

How can we apply this information to a more general idea against the stock market itself. Can we create any features from this EDA or determine when we should avoid trading if the model is not good enough. How do we go about measuring the success or practicality of these ideas?
