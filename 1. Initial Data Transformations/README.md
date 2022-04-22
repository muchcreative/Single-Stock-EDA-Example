## 1. Initial Data Transformations

Since individual stock data and their prices all vary. You have to be able to change your prices to robust forms that can be used for machine learning

We will go over some initial data transformations that 


not completely a random walk and creatine algorithsm to help trade the stock market are multivariate models with univariate ideas being impractical in real-life. 

Data:
- Data and stock OHLC data market is non-stationary
- Stock data does not completely follow a random walk, but there are trends within a stock price that can be determined by a random walk with a deterministic trend or drift. With the following being proved with both the advent of algorithmic trading strategies but more so with HFT (high frequency trading).

Deterministic Trend 

**Standardization:**

The most indsutry wide type of feature transformation for stock trading are log returns. A good explanation of why to use log returns from Quantivity read [here] (https://quantivity.wordpress.com/2011/02/21/why-log-returns/).

Standardization is the transofrmation of features by subtracting from mean and dividng by standard deviation

Standardization can be helpful in cases where the data follows a Gaussian distribution. 
However, this does not have to be necessarily true. Geometrically speaking, it translates the data to the mean vector of original data to the origin and squishes or expands the points if std is 1 respectively. 
We can see that we are just changing mean and standard deviation to a standard normal distribution which is still normal thus the shape of the distribution is not affected.

Standardization does not get affected by outliers because there is no predefined range of transformed features.

**Normalization:**

Normalization is used to transform features to be on a similar scale.
