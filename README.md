---
# 📈 Stock Market Trend Prediction Project

### **Phase 1: Data Exploration & Trend Modeling**

### **Phase 2: Final Insights, Documentation & Project Packaging**
---

## 🚀 Project Overview

This project applies machine learning to classify short-term **stock price trends** (Uptrend, Downtrend, Sideways) based on historical price data and over 40 technical indicators.

The goal is to produce a clean, professional analytical project suitable for learning, portfolio use, and preparing for more advanced MLOps work in Phase 3.

We do **not** deploy a production pipeline in this phase—focus is on high-quality analysis, modeling, documentation, and packaging.

---

## 📂 Project Structure

```text
stock-trend-analysis/
├── data/
├── notebooks/
├── models/
├── visuals/
├── docs/
├── src/
├── README.md
└── requirements.txt
```

See full folder description in the main documentation.

---

## 📊 Datasets Used

- **company_info.csv** — metadata for each stock
- **stock_prices.csv** — OHLCV price data
- **stock_prices_with_indicators.csv** — 40+ technical indicators (primary modeling dataset)
- **fundamental_data.csv** — quarterly financials (optional features)
- **market_indices.csv** — market context data

Processed modeling dataset is stored at:

```
data/processed/modeling_dataset.csv
```

---

## 🧪 Modeling Approach

Two core models are implemented:

### **1. Logistic Regression (Baseline Model)**

Used to establish a performance benchmark.

### **2. Random Forest Classifier (Improved Model)**

Used as the primary model for predictions.

Performance is evaluated using:

- Accuracy
- Precision, Recall, F1-score
- Confusion matrix

---

## 📈 Key Visualisations

The following visuals are included in the project:

### **Exploratory Analysis**

- Price trend charts
- Sector volatility comparisons
- Technical indicator patterns (RSI, MACD, Bollinger Bands)
- Correlation heatmap

### **Modeling Outputs**

- Confusion matrices
- Feature importance ranking
- Prediction vs actual trends

All visuals are saved under:

```
visuals/
```

---

## 🧠 Key Insights

### **Market Behaviour**

- Stock price movement is noisy and difficult to predict
- Technical indicators provide useful clues but have lag
- Volatility strongly influences trend direction

### **Model Performance**

- Baseline logistic regression achieved: XX% accuracy
- Random Forest achieved: XX% accuracy
- Model struggles most with “Sideways” predictions

### **Feature Importance Highlights**

Top contributors:

- Momentum indicators (RSI, momentum_10)
- Trend indicators (SMA20, SMA50)
- Volatility indicators (ATR, BB width)

---

## ⚠️ Limitations

- Short prediction horizon → very noisy labels
- Technical indicators lag behind real market movement
- Class imbalance affects trend prediction
- Model does not incorporate macroeconomic or sentiment data

---

## 🔮 Future Improvements

- Add return-based engineered features
- Introduce market regime classification
- Try advanced ML models (XGBoost, LightGBM)
- Introduce deep learning models (LSTM for time series)
- Move to full MLOps pipeline with MLflow + FastAPI + Streamlit in the next project

---

## 👥 Authors & Contributors

- **Project Lead:** Muhammad Yekini
- **Team:** Intern Group — Data Exploration, Modeling & Visualisations

---

## 📎 License
