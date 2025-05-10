# Jupyter Notebook Description

**ntantawichian_project.ipynb**  
_**Main Jupyter Noterbook for S&P500 Stock Analysis Project**_  
This notebook contains the full end-to-end workflow for analyzing S&P 500 stock data. It integrates data wrangling, exploratory analysis, machine learning, and forecasting to answer four research questions.

#### Key Features:
**1. Data Collection & Cleaning**
- Web scraped current stock performance from TradingView
- Web scraped industry sector and ticker from Wikipedia
- Historical OHLC data pulled from Yahoo Finance

**2. Merged Dataset Creation**
- Combined daily snapshot, sector labels, and 6-month history into sp500_stocks
- Calculated new fields such as:
    - Price Movement
    - Volume Spike Ratio
    - Buy/Hold/Sell SignalPredicted Signal from Machine Learning
 
**3. Research Questions Addressed**
1. Which stocks are good buy/sell/hold based on short-term price behavior?
2. Which industry sectors perform best/worst in terms of average return and price movement?
3. Which stocks exhibit the highest/lowest volatility based on daily price range?
4. Which stocks have unusual trading volume activity today relative to their normal average volume?

**4. Statistical Analysis**
- Descriptive statistics and visualizations
- Hypothesis testing using t-tests

**5. Machine Learning Models**
- Classification models to predict trading signals using:
  - Logistic Regression
  - Decision Tree
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
- Evaluated using accuracy and F1-score

**6. Time Series Forecasting**
- ARIMA-based 30-day price forecasts for top-volume stocks

**7. Final Export**
- Saves completed sp500_stocks DataFrame to CSV for further use
