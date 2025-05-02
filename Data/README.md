# Data

### Data Dictionary
| Field | Type | Description | 
| ------ | ------ | ------ |
| Ticker | Text | Stock symbol used for merging and analysis |
| Company Name | Text | Full name of the company |
| Company Sector | Text | Sector classification from _Wikipedia_ |
| Date | Date | Trading day date |
| Stock Price | Numeric | Latest available price from _TradingView_ |
| Price % Change | Text | Stock price percentage change (with +/- and % sign) |
| Price % Change (Numeric)| Numeric | Cleaned stock price % change as float |
| Open | Numeric | Opening price on that day |
| High | Numeric | Highest price on that day |
| Low | Numeric | Lowest price on that day |
| Close | Numeric | Closing price on that day |
| Volume | Numeric | Latest stock volume (converted to numeric) |
| 30 Days Avg Volulme | Numeric | 30 days average volume of each stock |
| Volume Spike Ratio | Numeric | Volume spike ratio of each stock (determine unusual volume activity) |
| Daily Movement | Numeric | Daily movement of each stock |
| Daily Volatility | Numeric | Daily volatility of each stock |

### CSV File Description
