# Section 5: Equity Analysis with Python (Part 1)

**Course:** Algorithmic Stock Trading and Equity Investing with Python  
**Section:** 5 - Equity Analysis with Python (Part 1)  
**Status:** ✅ Completed  
**Completed on:** [Add Date]

---

## 📚 Section Overview
This section introduces **equity analysis using Python** with the `yfinance` library. You'll learn how to download, manipulate, and analyze stock market data, including handling dividends, stock splits, adjusted close prices, and multiple tickers.

### Lecture Breakdown
| # | Lecture | Duration | Status |
|---|---------|----------|--------|
| 21 | Yahoo Finance - Overview | 5min | ✅ |
| 22 | How to open and work with the Course Notebooks | 3min | ✅ |
| 23 | How to Install yfinance | 2min | ✅ |
| 24 | yfinance API - first steps | 11min | ✅ |
| 25 | IMPORTANT NOTICE | 1min | ✅ |
| 26 | Excursus: Versions and Package Updates | 3min | ✅ |
| 27 | Analysis Period | 5min | ✅ |
| 28 | Data Frequency | 6min | ✅ |
| 29 | Dividends | 9min | ✅ |
| 30 | What's the Adjusted Close Price? | 8min | ✅ |
| 31 | Stock Splits | 8min | ✅ |
| 32 | Stocks from other Countries / Exchanges | 4min | ✅ |
| 33 | Multiple Tickers | 5min | ✅ |
| 34 | Saving and Loading Data (Local Files) | 7min | ✅ |
| 35 | [Article] Saving/Loading Data with Pandas - advanced topics | 1min | ✅ |
| 36 | Coding Challenge | - | ✅ |

**Total Time:** 1hr 22min (All Completed ✅)

---

## 🎯 Key Learning Points (All Mastered ✅)

### Yahoo Finance & yfinance
- ✅ Overview of Yahoo Finance as a data source
- ✅ Installing and setting up the `yfinance` library
- ✅ Basic API usage for downloading stock data

### Data Parameters
- ✅ Setting analysis periods (start/end dates)
- ✅ Understanding and selecting data frequency (daily, weekly, monthly)
- ✅ Handling dividends data
- ✅ Understanding Adjusted Close Price vs. Close Price
- ✅ Handling stock splits data

### Multi-Stock Analysis
- ✅ Downloading data for stocks from other countries/exchanges
- ✅ Working with multiple tickers simultaneously
- ✅ Saving and loading data to/from local files
- ✅ Advanced Pandas techniques for data persistence

### Practical Application
- ✅ Completed the coding challenge
- ✅ Understanding the importance of adjusted prices for accurate backtesting

---

## 📝 Personal Notes
*Add your own notes, code snippets, or tips here:*

### Basic yfinance Usage
```python
import yfinance as yf
import pandas as pd

# Download single stock
msft = yf.Ticker("MSFT")
hist = msft.history(period="1y")

# Download multiple stocks
stocks = ["AAPL", "GOOGL", "MSFT", "AMZN"]
data = yf.download(stocks, start="2020-01-01", end="2023-12-31")

# Get dividends
dividends = msft.dividends

# Get stock splits
splits = msft.splits
```

### Key Concepts
- **Adjusted Close Price:** Accounts for dividends and splits, essential for accurate return calculations
- **Stock Splits:** Increases number of shares, decreases price proportionally
- **Data Frequency:** Choose appropriate frequency based on your analysis needs
- **Ticker Format:** Different exchanges have different formats (e.g., .SA for Brazil)

---

## 🚀 All Lectures Completed ✅

| Lecture | Status |
|---------|--------|
| 21. Yahoo Finance - Overview | ✅ |
| 22. Working with Course Notebooks | ✅ |
| 23. Installing yfinance | ✅ |
| 24. yfinance API - first steps | ✅ |
| 25. IMPORTANT NOTICE | ✅ |
| 26. Versions and Package Updates | ✅ |
| 27. Analysis Period | ✅ |
| 28. Data Frequency | ✅ |
| 29. Dividends | ✅ |
| 30. Adjusted Close Price | ✅ |
| 31. Stock Splits | ✅ |
| 32. Stocks from other Countries | ✅ |
| 33. Multiple Tickers | ✅ |
| 34. Saving and Loading Data | ✅ |
| 35. Advanced Saving/Loading | ✅ |
| 36. Coding Challenge | ✅ |

---

## 🔗 Resources
- [yfinance Documentation](https://pypi.org/project/yfinance/)
- [Yahoo Finance](https://finance.yahoo.com/)
- [Pandas Documentation](https://pandas.pydata.org/)

---

## 💡 Key Takeaways from This Section
- **yfinance** is the go-to Python library for free stock data.
- **Adjusted Close** is crucial for accurate performance analysis.
- **Data Frequency** impacts analysis - choose based on your trading horizon.
- **Multiple Tickers** can be downloaded simultaneously for portfolio analysis.
- **Data Persistence** saves time by avoiding repeated API calls.
- **Stock Splits & Dividends** significantly affect returns and must be accounted for.
