# Trader-Behavior-Insights

🔍 Overview

This project analyzes the relationship between Bitcoin market sentiment and trader behavior/performance using historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index.

The goal is to understand:

How market emotions (Fear, Greed) affect profitability

How trader behavior changes across sentiment regimes

Which traders remain profitable regardless of market emotion

This analysis is designed to generate actionable insights for smarter trading strategies, risk management, and trader selection in Web3 markets.

📁 Datasets

The analysis uses two datasets provided as part of the assignment:

Historical Trader Data (Hyperliquid)

Key columns:
Account, Coin, Execution Price, Size USD, Side,
Closed PnL, Leverage, Timestamp IST, Trade ID, etc.

Bitcoin Fear & Greed Index

Columns:
date, value, Sentiment (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

⚠️ Note:
Raw datasets are not included in this repository due to size and data-sharing constraints.
The notebook assumes these files are available locally.

⚙️ Methodology

Data Cleaning & Preprocessing

Converted timestamps to datetime

Extracted trade date from timestamps

Merged trader data with daily sentiment data

Feature Engineering

Win/Loss flags

Risk-adjusted returns (PnL / Size USD)

Trade counts and capital deployed

Exploratory & Behavioral Analysis

PnL distribution across sentiment regimes

Buy vs Sell performance under each sentiment

Leverage and risk behavior analysis

Trader Intelligence

Trader-level performance metrics

Identification of traders profitable across multiple sentiment regimes

Detection of emotionally sensitive vs regime-robust traders

📊 Key Insights
📉 Market Sentiment & Strategy

Buying during Fear tends to outperform selling.

Selling during Greed and Extreme Greed yields significantly higher average PnL.

Emotional extremes create both opportunity and risk.

🧠 Trader Behavior

Many traders perform well in either Fear or Greed, but not both.

Extreme Greed shows the lowest win rates, suggesting overconfidence and poor risk control.

Risk-adjusted returns deteriorate when leverage increases during euphoric markets.

🏆 Elite Traders

A small subset of traders remains profitable across both Fear and Greed regimes.

These traders demonstrate emotional discipline and superior risk management.

Such traders are ideal candidates for capital allocation, copy trading, or funding strategies.

💡 Conclusion

Market sentiment is a powerful signal not only for trade timing (Buy Fear, Sell Greed) but also for trader selection and risk management.

The most valuable traders are not those who win in one emotional regime, but those who remain profitable across multiple market emotions.

This insight can directly inform Web3 trading platforms, prop desks, and hedge funds looking to optimize performance and control risk.

🛠 Tools & Libraries

Python

Pandas

NumPy

Matplotlib / Seaborn

Jupyter Notebook

📌 File Structure
Trader_Behavior_Insights.ipynb   # Main analysis notebook
README.md                       # Project overview
