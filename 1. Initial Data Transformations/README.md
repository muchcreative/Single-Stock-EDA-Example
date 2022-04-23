## 1. Initial Data Transformations

Starting with data transformations first, since individual stock data and their prices all vary. You have to be able to change your prices to robust forms that can be used for machine learning or algorthmic trading. Outputs must be consistent and reproducible in the vast majority of times. Additionally, casting the data to a normal distribution has benefits for anova and other statistical methods to be applied later.

**Data Characteristics Assumptions**

- Data and stock OHLC data market is non-stationary
- Stock data does not completely follow a random walk, but there are trends within a stock price that can be determined by a random walk with a deterministic trend or drift. With the following being proved with both the advent of algorithmic trading strategies HFT (high frequency trading) and the success of momentum trading.
- Predicting a single price of stock data can not be done with a univariate model. Stock data and the market is a multivariate and complex system.

### Types of Data Transformations

**1. Basic Returns**

The easiest type of data transformation is using basic daily returns given as (P2 / P1) for your machine learning or strategy inputs.

**2. Log-Returns**

The most well known form of data transformations for the stock market. More information on this and well founded reasoning can be found on Quantivity, seen [here](https://quantivity.wordpress.com/2011/02/21/why-log-returns/). The equation is given as log(P2/P1) with the recommened log base being e, but log10 has been used before. We will check both.

**3. Moving Averages**

Looking forward, because this data will be entered into an RNN, transformer, or other model as a sequence. There may be a possbility to utilize moving averages as features. Selecting an arbitrary sequence length. You can collect the daily returns and enter the returns to a simple or exponential moving average calculation. This has the benefits of casting the sequence to a well fixed range, but also helps the machine learning algorithm leverage a momentum indicator, which is an already proven, working, and successful trading strategy.

**4. Miscellaneous**

There have been papers published using Autoencoders or PCA to convert time sequences to an embedded vector space and analyze this space with attention models or other ANNs. I will skip this section for brevity and lack of research in its applicability, but it is something to keep in mind. Alternatively, there has been research done in Fourier Transformations and decompositions into frequency domain. However, that has yet show significant results over long-term dependencies or sequence lengths. In our case, we will stick to the more basic transformations to try to capture more human trading behaviors for the model.
