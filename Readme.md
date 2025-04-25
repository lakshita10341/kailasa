# 📊 NIFTY Index Trading Strategies – Comprehensive ML-Based Analysis

This repository presents a comparative analysis of three machine learning-driven trading strategies developed as part of the **Kailasa Capital Quantitative Challenge**. Each strategy targets the Indian markets, specifically the **NIFTY 50** and **NIFTY Bank** indices, across different timeframes using technical indicators and Random Forest models to predict price movements.

---

## 🧠 Strategy Summaries

### 1. NIFTY 50 Daily ML Strategy
- **Timeframe**: Daily  
- **Approach**: Medium-term trend identification using Random Forest classifier trained on multiple technical indicators  
- **Indicators**: SMA (5, 10), EMA (5, 10), RSI, Momentum, Volatility, Daily Returns  
- **Risk Management**: 10% take-profit, 5% stop-loss  
- **Results**:
  - 📈 CAGR: **65.75%**
  - 💰 Final Capital: ₹15.3 Cr (from ₹70L)
  - 🔁 Win Rate: 47.10%
  - 📉 Max Drawdown: -11.87%
  - 📊 Sharpe Ratio: **3.12**

---

### 2. RSI-Momentum 15-Minute Strategy
- **Timeframe**: 15-Minute  
- **Approach**: High-frequency intraday trades using RSI and Momentum  
- **Indicators**: RSI (14), Momentum (45)  
- **Risk Management**: 10% TP, 15% SL, 3 trades/day limit  
- **Results**:
  - 📈 Total Return: **1,478%**
  - 💰 Final Capital: ₹1.57 Cr (from ₹10L)
  - 🔁 Win Rate: **90.58%**
  - 📉 Max Drawdown: **-93.80%**
  - ⚠️ Sharpe Ratio: 1.29*

> *Despite high returns and win rate, this strategy suffers from extreme drawdowns and high time in drawdown (90%+), requiring better risk controls.

---

### 3. NIFTY Bank 60-Minute Strategy
- **Timeframe**: 60-Minute  
- **Approach**: Intraday balanced strategy with moderate frequency and signal quality  
- **Indicators**: SMA (5, 20), RSI, Bollinger Bands, Mean Reversion  
- **Risk Management**: 10% TP, 5% SL, 3 trades/day  
- **Results**:
  - 📈 CAGR: 3.44%
  - 💰 Profit: ₹4.58L (from ₹20L)
  - 🔁 Win Rate: 78.26%
  - 📉 Max Drawdown: -1.82%
  - 📊 Sharpe Ratio: -0.17

---

## 📊 Comparative Performance

| Strategy              | Timeframe     | CAGR     | Win Rate | Max Drawdown | Sharpe Ratio | Total Return |
|-----------------------|---------------|----------|----------|---------------|---------------|----------------|
| NIFTY 50 ML           | Daily         | **65.75%** | 47.10%   | -11.87%       | **3.12**       | **2085%**       |
| RSI-Momentum          | 15-Minute     | 0.00%*   | **90.58%** | **-93.80%**     | 1.29          | 1478%         |
| NIFTY Bank Strategy   | 60-Minute     | 3.44%    | 78.26%   | -1.82%        | -0.17         | 22.90%        |

---

## 🔍 Key Insights

- **Risk-adjusted returns** matter more than raw win rates. The NIFTY 50 ML strategy performs best despite a sub-50% win rate.
- **Drawdown management** is critical. RSI-Momentum shows the dangers of high-frequency trading without capital protection.
- **Timeframes** create trade-offs: shorter intervals offer more signals but higher noise and risks; daily provides more robust, reliable outcomes.
- **Machine Learning** (Random Forest) proved effective in uncovering actionable patterns, outperforming traditional rule-based systems when coupled with proper risk controls.

---

## 🧰 Technical Setup

Each strategy uses the following tools:
- 📈 Technical Indicators (SMA, EMA, RSI, Momentum, Bollinger Bands, Volatility)
- 🤖 Machine Learning (Random Forest Classifier)
- 📊 Backtesting Engine (custom Python implementation)
- 📉 Risk Controls (Take-Profit, Stop-Loss, Position Sizing)

---
