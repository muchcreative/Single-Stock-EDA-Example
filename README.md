## Stock-EDA-for-Black-Swan-Events

**STILL UPLOADING AND CLEANING UP THIS REPO**

High volatilities, high kurtosises, and fat-tail distributions are the enemy of stock trading machine learning models. Let's try to analyze these problems and understand how to create features for models to recognize these black-swan events for a stock or avoid them entirely. With these thoughts in mind we can sum up what we are looking for in 3 goals and start work from there.

**Goals and Data Prerequisites**

**Goals:**
1. How will we define and recognize black swan events?
2. Can we extract features from these events that can be translated to practical uses?
3. If (2) is not possible, can we introduce other data or add additional features/dimensions to aid in this task? 

**Data Prerequisites:**
- Adjusted OHLCV data for a variety of stocks.
- Adjusted OHLCV data for a basket of market indices.

If you do not have this data, look into my other repositories for building a stock database.

**Null Hypothesis**

After defining our goals let's create a null hypothesis to encompass what we have to reject to verify that we can create features or indicators for our strategy.

<p align="center"> <em> Black swan events are not recognizable and can not be accounted for when trading. </p> </em>
 
**Getting Started**

With the above out of the way, I will include all the modules I used in their respective sections under a module folder. Additionally, due to the changing nature of stock data, I will only be pulling around 15 years of data from my own database for the years 2008 to 2022. However, this timeframe will change depending on the task at hand, so it should not be a problem if your timeframes differ from mine. Ok, now, let's breakdown what is in this repository.

## Breakdown

**1. Initial Data Transformations**

We need to test out Log Transformations, Standarization, and Other Methods

Test different ways for standardizing vs normalizing your stock data. For plotting, histograms, QQ-plots, ACF, and PACF plots are your friends. Summarize findings and understand your cutoff to identify your fat-tail distributions using these methods. 

**2. Outlier Handling**

Check discretization, winsorization, filling effects or even if they can be applied here. There is a high chance that this type of filling reduces the volatility of the stock and therefore losing the information from the correlations between other features you may have if you have a multivariate system. This can easily lead to model drift (reducing overall model accuracy). If that is the case, outliers should not be removed, but should be accounted for in a strategy or ml system.

**3. Anomaly Detection and Clustering**

Understanding your data, let's see if we can run gaussian detection or other clustering methods to determine when these events happen. If not can we add any additional features to do so?

**4. How do we use this data beyond what we have?**

How can we apply this information to a more general idea against the stock market itself. Can we create any features from this EDA or determine when we should avoid trading if the model is not good enough. How do we go about measuring the success or practicality of these ideas?
