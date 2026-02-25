# Trader Performance vs Market Sentiment Analysis
Primetrade.ai – Data Science Intern Round 0 Assignment

## 📌 Objective

This project analyzes how Bitcoin market sentiment (Extreme Fear, Fear, Greed, Extreme Greed, Neutral) influences trader behavior and performance on Hyperliquid.

The goal is to uncover behavioral patterns and derive actionable trading strategies.

---

## 📂 Datasets

1. Bitcoin Fear/Greed Index  
   - Columns: Date, Classification  

2. Hyperliquid Historical Trader Data  
   - Columns include: account, execution price, size_usd, side, timestamp, closed_pnl, etc.

Both datasets were aligned at daily level.

---

## 🔧 Methodology

### 1️⃣ Data Preparation
- Cleaned column names
- Checked missing values and duplicates
- Converted timestamps to daily format
- Merged trader data with sentiment data

### 2️⃣ Feature Engineering
Created key metrics:
- Daily PnL per trader
- Win rate
- Average trade size
- Trade frequency
- Long/Short ratio
- Volatility (PnL standard deviation)

### 3️⃣ Sentiment-Based Analysis
Compared performance across:
- Extreme Fear
- Fear
- Greed
- Extreme Greed
- Neutral

### 4️⃣ Trader Segmentation
Traders were segmented into:
- Frequent vs Infrequent
- Consistent vs Inconsistent
- High Profit vs Low Profit

### 5️⃣ Strategy Recommendations
Developed sentiment-aware trading rules based on findings.

### 6️⃣ Bonus: Predictive Modeling
Built a Random Forest model to predict daily profitability using:
- Trade count
- Average trade size
- Win rate
- Sentiment

---

## 📊 Key Insights

- Profitability varies significantly across sentiment regimes.
- Trade frequency increases during Extreme Fear.
- Infrequent traders outperform frequent traders in Greed regimes.
- Inconsistent traders generate higher returns but with higher volatility.
- High-profit traders maintain performance even during extreme sentiment conditions.
- Behavioral metrics combined with sentiment contain predictive signals for profitability.

---

## 💡 Strategy Recommendations

1. Reduce trade size during Extreme Fear due to higher volatility.
2. Encourage selective trading during Greed periods instead of overtrading.
3. Apply sentiment-aware risk management filters for high-volatility regimes.

---

## 🤖 Machine Learning Results

- Random Forest model predicts daily profitability.
- Behavioral features such as trade count and win rate are strong predictors.
- Sentiment contributes additional predictive signal.

---

## ▶ How to Run

1. Clone the repository
2. Install required libraries:
   pip install pandas numpy matplotlib seaborn scikit-learn
3. Open the notebook:
   Trader_Performance_vs_Sentiment.ipynb


---

##  Conclusion

Market sentiment significantly influences trader behavior and performance.

Sentiment-aware trading adjustments can improve risk management and strategic decision-making.
   
