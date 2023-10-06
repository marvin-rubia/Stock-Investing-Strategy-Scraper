# Scraping Function for Stock Investing Analysis and Prediction
This repository develops my Python function that scrapes key stock information from Yahoo Finance necessary for a 1-year investment strategy. The result is a dataset with 10 columns, including the target variable. The function, which utilizes the `yfinance` Python library, can be used to collect more data for analysis and prediction. 

## Plan
As a positional stock trader, I want to simulate the experience of deciding whether to buy a stock or not. My goal is to produce a dataset that can be used for analysis and prediction. This is similar to the common trading practice of __backtesting__, which is a process to decide whether a trading system is really profitable, based on its performance using historical prices. Unfortunately, almost all backtesting softwares/platforms out there are not free. Hence, I'll do it on my own in Python.

__When to invest? (i.e. signal for investing)__

A day after the annual report is published. Because I need the data from the latest annual report to decide if I will invest in the stock for _this_ year. Thus, I have to code how to get the date of publication for the stock's annual report. 


Other data I need to scrape, code, and calculate: <br>
__Features:__
1. Buy Price (it is the open price for the next candle after the day the annual report becomes available)

2. % change from 52Wk High (expecting Buy Price to be lower than 52 Wk High, so there is room for price appreciation during the investment period)

3. % change from 52Wk Low (expecting Buy Price to be at least 20% above it, because closer to it might indicate a market or stock weakness for whatever reason)

  From the annual report:

4. Revenue growth (relative to the previous year)

5. Net income growth (relative to the previous year)

6. Earnings Per Share (Basic EPS)

7. Debt Ratio (total debt over total assets)

__Target:__ The maximum profit gained within the next 260 days (52 weeks * 5 trading days) after buying the stock.

## Snippet of the dataset I produced
![image](https://github.com/marvin-rubia/Stock-Investing-Strategy-Scraper/assets/140475770/4d73b390-979a-439c-a562-922334497bf3)

## How to see my work?
Check the Notebook uploaded in this repository. 
