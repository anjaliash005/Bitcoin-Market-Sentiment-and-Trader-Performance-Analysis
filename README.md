# Bitcoin Market Sentiment and Trader Performance Analysis

## Primetrade.ai Data Science Internship Assignment

### Author

Anjali Ashtankar

---

## Project Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance using historical trading data from Hyperliquid and Bitcoin Fear & Greed sentiment data.

The objective is to determine whether market sentiment influences trader profitability, win rates, and trading behavior, while uncovering patterns that may help improve trading strategies and decision-making.

---

## Business Objective

The goal of this analysis is to:

* Explore the impact of Bitcoin market sentiment on trader performance.
* Identify behavioral patterns across different sentiment conditions.
* Evaluate profitability and win rates under varying market emotions.
* Generate actionable insights that could support data-driven trading strategies.

---

## Datasets Used

### 1. Bitcoin Market Sentiment Dataset

Contains daily Bitcoin Fear & Greed Index values and sentiment classifications.

**Key Fields**

* Date
* Value
* Classification

  * Extreme Fear
  * Fear
  * Neutral
  * Greed
  * Extreme Greed

### 2. Hyperliquid Historical Trader Dataset

Contains detailed historical trading activity.

**Key Fields**

* Account
* Coin
* Execution Price
* Size Tokens
* Size USD
* Side
* Timestamp IST
* Start Position
* Direction
* Closed PnL
* Fee
* Transaction Hash
* Order ID
* Trade ID

---

## Project Workflow

### Data Cleaning

* Inspected dataset structure and column information.
* Converted timestamp fields into datetime format.
* Standardized date formats across datasets.
* Resolved datatype mismatches during merging.
* Validated merged records and sentiment assignments.

### Data Integration

* Extracted trade dates from trading records.
* Merged trading data with sentiment data using date as the common key.
* Verified successful mapping of sentiment classifications.

### Exploratory Data Analysis

The following analyses were performed:

1. Profitability by Market Sentiment
2. Win Rate Analysis
3. Buy vs Sell Activity Analysis
4. Top Performing Traders
5. Most Profitable Coins
6. Fee Analysis
7. Correlation Analysis and Heatmap

---

## Key Findings

* Extreme Greed produced the highest average profit per trade.
* Extreme Greed also generated the highest win rate.
* Fear conditions generated the highest cumulative profitability due to greater trading activity.
* Extreme Fear resulted in the lowest win rates and profitability.
* Trading activity remained relatively balanced between buying and selling.
* A small number of assets contributed the majority of overall profits.
* Market sentiment demonstrated a measurable relationship with trader performance.

---

## Visualizations

The notebook includes the following visualizations:

* Average Profit by Market Sentiment
* Win Rate by Market Sentiment
* Buy vs Sell Activity by Sentiment
* Top Performing Coins
* Correlation Heatmap

---

## Leverage Analysis Note

Leverage analysis was initially planned because leverage was referenced in the assignment description.

However, the provided trading dataset did not contain any leverage-related field.

As a result:

* Leverage analysis could not be performed.
* No leverage metrics were available for evaluation.
* Related code was removed from the final notebook.
* Only analyses supported by the available dataset were included.

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## Repository Structure

```text
├── Anjali_Ashtankar_Primetrade_Sentiment_Analysis.ipynb
├── Anjali_Ashtankar_Primetrade_Trader_Performance_Analysis.pdf
├── merged_trader_sentiment_data.csv
├── README.md
```

---

## Conclusion

This project demonstrates how market sentiment data can be integrated with historical trading activity to better understand trader behavior and performance. The findings suggest that sentiment indicators can provide valuable context for evaluating market conditions and supporting trading decisions.

The analysis highlights the importance of combining behavioral market signals with transactional trading data to generate actionable insights in cryptocurrency markets.
