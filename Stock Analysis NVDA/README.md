<div align="center">

# 🧠 NVIDIA Next-Day Stock Prediction System (NVDA)

**Quantitative AI-driven forecasting pipeline for NVIDIA (NVDA) using hybrid statistical, ML & DL models**

![NVIDIA Banner](Visual%20Data/nvda_banner.png)

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-FF6F00?logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-Gradient%20Boosting-007ACC?logo=xgboost)](https://xgboost.readthedocs.io/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Data%20Viz-11557c?logo=plotly&logoColor=white)](https://matplotlib.org/)
[![scikit-learn](https://img.shields.io/badge/Scikit--Learn-ML%20Toolkit-F7931E?logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![ARCH](https://img.shields.io/badge/ARCH-GARCH%20Modeling-00758F?logo=python)](https://arch.readthedocs.io/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)

</div>

---

## 📘 Overview

This project develops a **multi-model ensemble** to forecast **NVIDIA's next-day stock price**, integrating:

- **ARIMA-GARCH** for volatility modeling  
- **XGBoost** for market regime classification  
- **LSTM-GRU Attention** for time-series sequence prediction  
- **Monte Carlo Simulation** for probabilistic analysis  

Outputs include **next-day price forecasts**, **confidence intervals**, **risk metrics**, and **trading signals**.

---

## 📊 Sample Prediction Report

| Metric | Value |
|--------|--------|
| **Current Price** | \$183.16 |
| **Predicted Next-Day Price** | \$186.58 (+1.87%) |
| **95% Confidence Interval** | [\$182.07, \$184.05] |
| **Sharpe Ratio** | 6.79 |
| **Volatility Forecast** | 4.36% |
| **Recommendation** | 🟢 **BUY** |

### 📉 Trend & Mean Reversion
- Trend: 📉 Downtrend  
- Mean Reversion Level: \$156.14  
- Half-Life: 53.7 days  

### 📈 Trading Strategy
| Parameter | Value |
|------------|--------|
| Entry | \$183.16 |
| Stop Loss | \$182.07 |
| Target | \$186.58 |
| Take Profit | +1.87% |
| Risk/Reward | 3.13 |
| Kelly Size | 0.00% (risk-neutral stance) |

---

## 🧩 Model Architecture

### 🧮 1. ARIMA-GARCH
Captures temporal autocorrelation and conditional volatility using econometric principles.

### ⚡ 2. XGBoost
Ensemble gradient-boosting tree model for identifying market regime patterns.

### 🧠 3. LSTM-GRU Attention
Hybrid recurrent network for sequential financial forecasting.  
Final validation loss: **0.0001**

### 🎲 4. Monte Carlo Simulation
Simulates **10,000 stochastic paths** to generate uncertainty intervals and risk profiles.

### 🔗 5. Ensemble Layer
Weighted integration of all models:
- ARIMA-GARCH → 15%  
- XGBoost → 20%  
- LSTM-GRU → 45%  
- Monte Carlo → 20%


---

## ⚙️ Key Features

✅ Multi-Model Ensemble (ARIMA + XGBoost + LSTM-GRU + Monte Carlo)  
✅ Advanced Feature Engineering (34 indicators)  
✅ Real-Time Volatility Forecasting  
✅ Monte Carlo Risk Estimation  
✅ Confidence Intervals & Value-at-Risk (VaR)  
✅ Automated Model Saving / Reloading  
✅ Visualization Dashboards (Matplotlib + Plotly)  
✅ Trading Signal Generator (Buy/Sell Recommendations)  

---

## 🚀 How to Run

### **1️⃣ Install Dependencies**
```bash
pip install pandas numpy scikit-learn tensorflow xgboost matplotlib arch


