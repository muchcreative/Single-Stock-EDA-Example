## 1. Initial Data Transformations

Starting with data transformations first, since individual stock data and their prices all vary. You have to be able to change your prices to robust forms that can be used for machine learning or algorthmic trading. Outputs must be consistent and reproducible in the vast majority of times. Additionally, casting the data to a normal distribution has benefits for anova and other statistical methods to be applied later.

**Data Characteristics Assumptions**

- Data and stock OHLC data market is non-stationary
- Stock data does not completely follow a random walk, but there are trends within a stock price that can be determined by a random walk with a deterministic trend or drift. With the following being proved with both the advent of algorithmic trading strategies HFT (high frequency trading) and the success of momentum trading.
- Predicting a single price of stock data can not be done with a univariate model. Stock data and the market is a multivariate and complex system.

### Types of Data Transformations

**1. Basic Returns**

The easiest type of data transformation is using basic returns

**2. Log-Returns**

The most well known form of data transformations for the stock market. Quantivity read [here] (https://quantivity.wordpress.com/2011/02/21/why-log-returns/).

The most indsutry wide type of feature transformation for stock trading are log returns. A good explanation of why to use log returns from
Standardization is the transofrmation of features by subtracting from mean and dividng by standard deviation

Standardization can be helpful in cases where the data follows a Gaussian distribution. 
However, this does not have to be necessarily true. Geometrically speaking, it translates the data to the mean vector of original data to the origin and squishes or expands the points if std is 1 respectively. 
We can see that we are just changing mean and standard deviation to a standard normal distribution which is still normal thus the shape of the distribution is not affected.

Standardization does not get affected by outliers because there is no predefined range of transformed features.

**3. Moving Averages**

Looking forward, because this data will be entered into an LSTM or transformer as a sequence. There may be a possbility to utilize moving averages as features. Selecting an arbitrary sequence length.

**4. Misc **

There has been papers published using Autoencoders or PCA to convert time sequences to an embedded vector space and analyze this space with transformers. I will skip this section for brevity and lack of research in its applicability, but it is something to keep in mind.
