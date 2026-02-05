# 📊 Trader Performance vs Market Sentiment Analysis

**Primetrade.ai — Data Science Intern Assignment**

---

## 📌 Overview

This project explores how market sentiment (Fear/Greed Index) influences trader behavior and performance on Hyperliquid. By merging sentiment data with historical trade activity, the analysis identifies patterns in profitability, risk-taking, and participation across different emotional market phases.

The goal is to extract actionable insights that can inform smarter trading strategies.

---

## 🎯 Objective

To analyze the relationship between Bitcoin market sentiment and trader behavior by answering:

* Does trader performance differ during Fear vs Greed periods?
* Do traders change their behavior based on sentiment?
* Can we identify meaningful trader segments?
* What strategy ideas emerge from the observed patterns?

---

## 🗂️ Datasets Used

### 1) Bitcoin Market Sentiment Dataset

Contains:

* Timestamp
* Sentiment value
* Classification

  * Fear
  * Greed
  * Extreme Fear
  * Extreme Greed
  * Neutral

### 2) Historical Trader Data (Hyperliquid)

Contains:

* Account
* Coin
* Execution Price
* Size (USD & Tokens)
* Side (Buy/Sell)
* Closed PnL
* Fees
* Timestamp

---

## 🧹 Data Preparation

Steps performed:

* Converted timestamps to a consistent date format
* Created a daily-level alignment between datasets
* Merged trade data with sentiment classification by date
* Checked for missing values and duplicates
* Removed rows without sentiment labels

This ensured that each trade was tagged with the corresponding market sentiment for that day.

---

## ⚙️ Feature Engineering

### Performance Metrics

* Daily PnL per trader
* Average PnL per trade
* Win rate per trader
* Profit consistency

### Behavioral Metrics

* Number of trades per day
* Average trade size (USD)
* Total trading volume per account
* Long vs Short activity ratio

### Trader Segmentation

Traders were categorized into:

* High-volume vs Low-volume traders
* Frequent vs Casual traders
* Profitable (Winners) vs Unprofitable (Losers)

---

## 📈 Analysis Performed

The study compared trader behavior across sentiment regimes:

* Fear
* Greed
* Extreme Fear
* Extreme Greed
* Neutral

Key relationships examined:

* PnL vs sentiment
* Win rate vs sentiment
* Trade size vs sentiment
* Trading activity vs sentiment
* Segment-wise performance differences

Visualizations were used to highlight behavioral shifts and performance trends.

---

## 🔍 Key Insights

**1) Profitability improves during Greed phases**
Average trader performance tends to be stronger during Greed and Extreme Greed periods, suggesting favorable momentum-driven conditions.

**2) Risk appetite increases in bullish sentiment**
Traders take larger positions and trade more actively during Greed phases, indicating higher confidence and capital deployment.

**3) Volatility and losses increase during Extreme Fear**
PnL distributions show higher downside risk during fear-driven markets, with more inconsistent outcomes.

**4) High-activity traders dominate market participation**
Frequent and high-volume traders contribute significantly to total market activity and shape overall performance trends.

---

## 🧠 Strategy Recommendations (Actionable Output)

**Strategy 1 — Risk Reduction in Fear Markets**
During Fear/Extreme Fear periods:

* Reduce position size
* Avoid aggressive entries
* Focus on capital preservation

**Strategy 2 — Momentum Participation in Greed Markets**
During Greed/Extreme Greed:

* Increase trade participation cautiously
* Scale positions gradually
* Momentum-based strategies may perform better

---

## 📊 Tools & Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## ▶️ How to Run

1. Clone the repository:

   ```
   git clone <your-repo-link>
   ```

2. Open the notebook:

   ```
   primeTradeAI_Assessment.ipynb
   ```

3. Run all cells sequentially to reproduce:

   * Data preparation
   * Feature engineering
   * Analysis
   * Visualizations

---

## 📁 Project Structure

```
├── primeTradeAI_Assessment.ipynb
├── README.md
└── (datasets loaded locally)
```

---

## 📌 Conclusion

This analysis demonstrates a clear connection between market sentiment and trader behavior. Traders tend to take more risks and perform better in Greed-driven markets, while Fear periods are associated with higher volatility and more cautious participation.

Segment-level insights further highlight that trading behavior is not uniform across participants, suggesting that adaptive, sentiment-aware strategies may improve outcomes.

---

## 🚀 Future Improvements

* Build a predictive model for next-day profitability
* Cluster traders into behavioral archetypes
* Create a Streamlit dashboard for interactive exploration

---


