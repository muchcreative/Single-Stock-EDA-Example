## Single-Stock-EDA-for-Black-Swan-Events

**STILL UPLOADING AND CLEANING UP THIS REPO**

High volatilities, high kurtosises, and fat-tail distributions are the enemy of stock trading machine learning models. Let's try to analyze these problems and understand how to create features for models to recognize these black-swan events for a single stock.

**Goals:** 
- Create applicable machine learning or strategy algorithmic features



I am assuming you already have the adjusted OHLCV data for a single stock. If you do not have this data, look into my other repositories for how to build a rotating stock dataset. You will also need market data for part 4 below.

This is an excerpt from one of my stock machine learning programs.

**Starting Ideas**


There our Null Hypothesis Will Be:
- *Some null hypothesis*

Will be, not completely a random walk but a verison of it with some underlying trend or drift and creating algorithsm to help trade the stock market are multivariate models with univariate models being impractical in real-life. 

## Breakdown

**1. Initial Data Transformations**

We need to test out Log Transformations, Standarization, and Other Methods**

Test different ways for standardizing vs normalizing your stock data. For plotting, histograms, QQ-plots, ACF, and PACF plots are your friends. Summarize findings and understand your cutoff to identify your fat-tail distributions using these methods. 

**2. Outlier Handling**

Check discretization, winsorization, or filling effects.

**3. Anomaly Detection and Clustering**

Understanding your data, let's see if we can run gaussian detection or other clustering methods to determine when these events happen. If not can we add any additional features to do so?

**4. How do we use this data beyond what we have?**

How can we apply this information to a more general idea against the stock market itself. Can we create any features from this EDA or determine when we should avoid trading if the model is not good enough. How do we go about measuring the success or practicality of these ideas?
