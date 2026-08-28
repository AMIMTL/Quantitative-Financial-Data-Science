# Section 14: How to build and analyze a Stock Index

**Course:** Algorithmic Stock Trading and Equity Investing with Python  
**Section:** 14 - How to build and analyze a Stock Index  
**Status:** ✅ Completed  

---

## 📚 Section Overview
This section teaches you how to **build and analyze stock indices** using Python. You'll learn the three main weighting methods (price-weighted, equal-weighted, and market value-weighted) and compare their performance.

### Lecture Breakdown
| # | Lecture | Duration | Status |
|---|---------|----------|--------|
| 138 | Financial Indices - an Overview | 9min | ✅ |
| 139 | Getting started | 2min | ✅ |
| 140 | Price-Weighted Index - Theory | 8min | ✅ |
| 141 | Building the Dow Jones Industrial Average Index from scratch | 5min | ✅ |
| 142 | Equal-Weighted Index - Theory | 6min | ✅ |
| 143 | Creating an Equal-Weighted Stock Index with Python | 2min | ✅ |
| 144 | Market Value-Weighted Index - Theory | 9min | ✅ |
| 145 | ***Update*** December 2023 | 1min | ✅ |
| 146 | Creating a Market Value-Weighted Stock Index with Python (Part 1) | 5min | ✅ |
| 147 | Creating a Market Value-Weighted Stock Index with Python (Part 2) | 4min | ✅ |
| 148 | Comparison of weighting methods (Part 1) | 2min | ✅ |
| 149 | Comparison of weighting methods (Part 2) | 4min | ✅ |
| 150 | Price Index vs. Performance/Total Return Index | 4min | ✅ |

**Quizzes:**  
- ✅ Quiz 1: Stock Indices  
- ✅ Quiz 2: Price-Weighted Index (PWI)  
- ✅ Quiz 3: Equal-Weighted Index (EWI)  
- ✅ Quiz 4: Market Value-Weighted Index (VWI)

**Total Time:** 59min (All Completed ✅)

---

## 🎯 Key Learning Points (All Mastered ✅)

### Financial Indices Overview
- ✅ What stock indices are and their purpose
- ✅ How indices track market performance
- ✅ Real-world examples

### Price-Weighted Index (PWI)
- ✅ Theory behind price-weighted indices
- ✅ Building the Dow Jones Industrial Average from scratch
- ✅ **Quiz 1: Stock Indices** completed
- ✅ **Quiz 2: PWI** completed

### Equal-Weighted Index (EWI)
- ✅ Theory behind equal-weighted indices
- ✅ Creating an Equal-Weighted Stock Index with Python
- ✅ **Quiz 3: EWI** completed

### Market Value-Weighted Index (VWI)
- ✅ Theory behind market value-weighted indices
- ✅ Creating a Market Value-Weighted Stock Index with Python (2 parts)
- ✅ **Quiz 4: VWI** completed

### Comparison & Analysis
- ✅ Comparison of weighting methods (2 parts)
- ✅ Price Index vs. Performance/Total Return Index

---

## 📝 Personal Notes
*Add your own notes, code snippets, or tips here:*

### Index Weighting Methods Comparison

| Method | Calculation | Example | Characteristics |
|--------|-------------|---------|-----------------|
| **Price-Weighted** | Sum of prices / divisor | DJIA | High-price stocks have more influence |
| **Equal-Weighted** | Equal allocation to each stock | SPW | All stocks have equal influence |
| **Value-Weighted** | Market cap / total market cap | S&P 500 | Larger companies have more influence |

### Python Implementation Snippets

```python
import pandas as pd
import yfinance as yf

# Price-Weighted Index (Dow Jones Style)
def price_weighted_index(prices):
    """Calculate price-weighted index."""
    return prices.sum(axis=1) / divisor

# Equal-Weighted Index
def equal_weighted_index(returns):
    """Calculate equal-weighted index returns."""
    return returns.mean(axis=1)

# Value-Weighted Index (S&P 500 Style)
def value_weighted_index(prices, shares_outstanding):
    """Calculate value-weighted index returns."""
    market_caps = prices * shares_outstanding
    total_market_cap = market_caps.sum(axis=1)
    weights = market_caps.div(total_market_cap, axis=0)
    returns = prices.pct_change()
    return (returns * weights).sum(axis=1)
```

### Key Concepts
- **Price-Weighted:** High-priced stocks dominate (e.g., Dow Jones)
- **Equal-Weighted:** Each stock has equal impact
- **Value-Weighted:** Larger companies dominate (e.g., S&P 500)
- **Price Index vs. Total Return Index:** Total return includes dividends

---

## 🚀 All Lectures Completed ✅

| Lecture | Status |
|---------|--------|
| 138. Financial Indices Overview | ✅ |
| 139. Getting started | ✅ |
| 140. Price-Weighted Index Theory | ✅ |
| 141. Building DJIA from scratch | ✅ |
| 142. Equal-Weighted Index Theory | ✅ |
| 143. Creating EWI with Python | ✅ |
| 144. Market Value-Weighted Theory | ✅ |
| 145. December 2023 Update | ✅ |
| 146. Creating VWI (Part 1) | ✅ |
| 147. Creating VWI (Part 2) | ✅ |
| 148. Comparison (Part 1) | ✅ |
| 149. Comparison (Part 2) | ✅ |
| 150. Price Index vs. Total Return | ✅ |

### Quizzes Completed ✅
| Quiz | Topic | Status |
|------|-------|--------|
| Quiz 1 | Stock Indices | ✅ |
| Quiz 2 | Price-Weighted Index | ✅ |
| Quiz 3 | Equal-Weighted Index | ✅ |
| Quiz 4 | Value-Weighted Index | ✅ |

---

## 🔗 Resources
- [S&P 500 Index](https://www.spglobal.com/spdji/en/indices/equity/sp-500/)
- [Dow Jones Industrial Average](https://www.spglobal.com/spdji/en/indices/equity/dow-jones-industrial-average/)
- [Investopedia: Price-Weighted Index](https://www.investopedia.com/terms/p/priceweightedindex.asp)

---

## 💡 Key Takeaways from This Section
- **Price-Weighted:** The Dow Jones uses this method - expensive stocks dominate.
- **Equal-Weighted:** Gives smaller companies equal influence.
- **Value-Weighted:** S&P 500 uses this - market cap determines influence.
- **Price Index vs. Total Return:** Total return includes dividends, which matters for long-term performance.
- **Python makes it easy** to build and compare different index types.
- The **4 quizzes** solidified understanding of each weighting method.
- This section is **foundational** for understanding ETFs and portfolio construction.
