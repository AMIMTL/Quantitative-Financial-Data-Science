# Section 7: Equity Analysis with Python (Part 2)

**Course:** Algorithmic Stock Trading and Equity Investing with Python  
**Section:** 7 - Equity Analysis with Python (Part 2)  
**Status:** ✅ Completed  
**Completed on:** [Add Date]

---

## 📚 Section Overview
This section continues the equity analysis journey, diving deeper into **stock valuation concepts** including market capitalization, enterprise value, book value, and financial statements. You'll learn to distinguish between price and value, and understand key financial metrics.

### Lecture Breakdown
| # | Lecture | Duration | Status |
|---|---------|----------|--------|
| 52 | ***Update*** December 2023 | 8min | ✅ |
| 53 | IMPORTANT NOTICE | 1min | ✅ |
| 54 | Getting more Information on Stocks - the Ticker Object | 4min | ✅ |
| 55 | Price, Shares Outstanding & Market Capitalization | 5min | ✅ |
| 56 | Price vs. Value and Market Efficiency | 10min | ✅ |
| 57 | Equity Value, Firm Value and Financial Distress | 4min | ✅ |
| 58 | Market Value vs. Book Value (Part 1) | 13min | ✅ |
| 59 | Market Value vs. Book Value (Part 2) | 8min | ✅ |
| 60 | Liquidation Value | 5min | ✅ |
| 61 | Market Value vs. Book Value (Part 3) | 7min | ✅ |
| 62 | How to load Financial Statements | 4min | ✅ |

**Total Time:** 1hr 8min (All Completed ✅)

---

## 🎯 Key Learning Points (All Mastered ✅)

### Stock Information & Ticker Objects
- ✅ Using the `yfinance` Ticker object to get comprehensive stock info
- ✅ Understanding price, shares outstanding, and market capitalization
- ✅ Accessing additional stock metadata

### Valuation Concepts
- ✅ Price vs. Value and Market Efficiency
- ✅ Equity Value vs. Firm Value
- ✅ Understanding Financial Distress
- ✅ Market Value vs. Book Value (3 parts)
- ✅ Liquidation Value

### Financial Statements
- ✅ How to load financial statements with Python
- ✅ Accessing income statements, balance sheets, and cash flow data

### Key Resources
- ✅ Additional resources provided for valuation concepts

---

## 📝 Personal Notes
*Add your own notes, code snippets, or tips here:*

### Getting Stock Information with yfinance
```python
import yfinance as yf

# Create ticker object
ticker = yf.Ticker("AAPL")

# Get stock info
info = ticker.info
print(f"Market Cap: {info['marketCap']:,}")
print(f"Shares Outstanding: {info['sharesOutstanding']:,}")
print(f"Price: ${info['currentPrice']}")
print(f"Book Value: {info['bookValue']}")
print(f"P/E Ratio: {info['trailingPE']}")

# Get financial statements
balance_sheet = ticker.balance_sheet
income_stmt = ticker.income_stmt
cash_flow = ticker.cashflow
```

### Key Valuation Metrics
```python
# Market Capitalization
market_cap = price * shares_outstanding

# Enterprise Value (EV)
# EV = Market Cap + Total Debt - Cash & Equivalents

# Book Value per Share
book_value_per_share = total_equity / shares_outstanding

# Price to Book (P/B) Ratio
pb_ratio = price / book_value_per_share

# Price to Earnings (P/E) Ratio
pe_ratio = price / earnings_per_share
```

### Market Value vs. Book Value - Key Differences
| Aspect | Market Value | Book Value |
|--------|-------------|------------|
| **Based on** | Current stock price | Accounting records |
| **Reflects** | Future expectations | Historical cost |
| **Volatility** | High | Low |
| **Intangibles** | Includes (brand, IP) | Excludes (or limited) |
| **Calculation** | Price × Shares Outstanding | Total Assets - Total Liabilities |

---

## 🚀 All Lectures Completed ✅

| Lecture | Status |
|---------|--------|
| 52. December 2023 Update | ✅ |
| 53. IMPORTANT NOTICE | ✅ |
| 54. Getting Ticker Object Information | ✅ |
| 55. Price, Shares & Market Cap | ✅ |
| 56. Price vs. Value & Market Efficiency | ✅ |
| 57. Equity Value, Firm Value & Distress | ✅ |
| 58. Market Value vs. Book Value (Part 1) | ✅ |
| 59. Market Value vs. Book Value (Part 2) | ✅ |
| 60. Liquidation Value | ✅ |
| 61. Market Value vs. Book Value (Part 3) | ✅ |
| 62. Loading Financial Statements | ✅ |

---

## 🔗 Resources
- [yfinance Ticker Documentation](https://pypi.org/project/yfinance/)
- [Investopedia: Market Capitalization](https://www.investopedia.com/terms/m/marketcapitalization.asp)
- [Investopedia: Book Value](https://www.investopedia.com/terms/b/bookvalue.asp)
- [Investopedia: Enterprise Value](https://www.investopedia.com/terms/e/enterprisevalue.asp)

---

## 💡 Key Takeaways from This Section
- **Price ≠ Value**: Price is what you pay, value is what you get.
- **Market Cap** = Price × Shares Outstanding - the total value of a company's equity.
- **Book Value** is based on accounting records; **Market Value** is based on market expectations.
- **Market Value > Book Value** suggests growth expectations; **Market Value < Book Value** might indicate undervaluation or distress.
- **Enterprise Value** includes debt and cash - it's the true cost of acquiring a company.
- **Liquidation Value** is the value if assets are sold off - a worst-case floor valuation.
- **Financial Statements** (Income Statement, Balance Sheet, Cash Flow) are essential for fundamental analysis.
- The **Ticker Object** in yfinance provides easy access to all this data.
- This section bridges the gap between **Python programming and fundamental analysis**.
