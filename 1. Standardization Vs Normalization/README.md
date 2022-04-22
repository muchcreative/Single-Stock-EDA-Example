## Normalization Vs Standardization

**Let's Start with the Difference Between the Two**

Taken from [GeeksForGeeks: Normalization Vs Standardization](https://www.geeksforgeeks.org/normalization-vs-standardization]). Stock data is non-stationary time series data meaning their "means, variances, and covariances that change over time. Non-stationary behaviors can be trends, cycles, random walks, or combinations of the three." Further explanation of non-stationarity can be found [here](https://www.investopedia.com/articles/trading/07/stationary.asp#:~:text=Non%2DStationary%20Processes-,Non%2DStationary%20Time%20Series%20Data,or%20combinations%20of%20the%20three).

Assumptions will be , not completely a random walk and creatine algorithsm to help trade the stock market are multivariate models with univariate ideas being impractical in real-life. 

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
