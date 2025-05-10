# Data

### Data Dictionary
| Field | Type | Description | 
| ------ | ------ | ------ |
| Ticker | Text | Stock symbol used for merging and analysis |
| Company Name | Text | Full name of the company |
| Company Sector | Text | Sector classification from _Wikipedia_ |
| Date | Date | Trading day date |
| Stock Price | Numeric | Latest available price from _TradingView_ |
| Open | Numeric | Opening price on that day |
| High | Numeric | Highest price on that day |
| Low | Numeric | Lowest price on that day |
| Close | Numeric | Closing price on that day |
| Price % Change (Numeric)| Numeric | Cleaned stock price % change as float |
| Price Movement | Numeric | Absolute value of daily return, showing magnitude of price change regardless of direction |
| Daily Volatility | Numeric | Daily volatility of each stock |
| Volume | Numeric | Latest stock volume (converted to numeric) |
| 30 Days Avg Volulme | Numeric | 30 days average volume of each stock |
| Volume Spike Ratio | Numeric | Volume spike ratio of each stock (determine unusual volume activity) |
| Signal | Text | Classification of stock as Buy, Sell, or Hold |
| Predicted Signal | Text | Machine learning model prediction on stock movement, classified as Buy, Sell, or Hold |



### CSV/XLS File Description
**1. sp500_stocks.xls** (Final cleaned and merged dataset)
Contains one row per S&P 500 stock with enriched metrics for all research questions. Includes latest OHLC data, calculated volatility, buy/sell/hold signals, volume spike analysis, and machine learning predictions.
_**Key Fields:**_
- Ticker, Company Name, Company Sector
- Stock Price, Open, High, Low, Close
- Price % Change (Numeric), Volume, 30-Day Avg Volume, Volume Spike Ratio
- Price Movement, Daily Volatility
- Signal, Predicted Signal

**2. sp500hist_data.xls** (Raw 6-month historical OHLC data for all S&P 500 tickers)
- Downloaded from Yahoo Finance. Provides daily Open, High, Low, Close, and Volume for each ticker.
- Used to compute rolling volume averages and support ARIMA-based time series forecasting.

**3. wiki_sector.xls** (Sector classification for all S&P 500 companies)
Scraped from Wikipedia. Maps each stock ticker to its official GICS sector and sub-industry classification and used for sector-based grouping and performance comparison.
_**Key Fields:**_
- Symbol, GICS Sector

**4. tickers_only.xls** (List of all S&P 500 ticker symbols)
- Simple file containing only ticker symbols.
- Used to generate the download list and merge data across sources.
