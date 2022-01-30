# projects.github.io

# StockMLRN

StockMLRN is react-native app implementing forecasting top 18 stocks on SGX
Singapore Stock Exchange using 5 various Time-Series forecasting models.

Important to note, there is **no tool or model that can predict the
future**, but more probability scenario given past historical prices.

There are many models and business in the industry forecasting stock
prices.  This is purely for experimental.

## Models

### ARIMA

ARIMA is text book standard Time-Series forecasting.  It stands for
**Autoregressive integrated moving average**.  Clearly Stock generally
does not follow any cycle pattern.  Meaning it does not have seasonality.

The model is conservative, will score well with low volatility. As seen
for the SGX stocks it does score the highest in forecasting accuracy.

### mSSA

mSSA **multivariate Singular Spectrum Analysis** model was used from
the repository is the implementation of the [paper: On Multivariate Singular Spectrum Analysis](https://arxiv.org/abs/2006.13448). Refer to the paper for more information about the theory and the algorithm of mSSA.  MIT.

It is does well with more multi variables, just besides the single stock.
You could bring in Stock Market daily averages and volatility to produce
better forecasting model.  But for simplicity I just used the stock price.

### Facebook Prophet

This is now available for public use and produced by Facebook.
The model performs the lowest score, this is due to the fact
that model is more geared to predict the new trends.
Trend is your friend.

### LSTM

LSTM Long short-term memory is a model using neural networks deep learning techniques e.g. nearest neighbour and is uses technical of graph theorems.

This is the most complex model.



## About the Developer

Justin Woodhead is Integration Specialist in the Finance sector.  
Can be reached on in Linked-In  https://www.linkedin.com/in/justin-woodhead/
