# 🧠 Trader Behavior Insights Based on Market Sentiment

## 📈 Project Overview

This project analyzes the relationship between **Bitcoin market sentiment** (Fear/Greed Index) and **trader performance** using historical trading data from Hyperliquid. The goal is to uncover patterns that reveal how emotions like fear and greed impact real trading behavior and profitability.

---

## 📊 Datasets Used

### 1. 📅 **Bitcoin Market Sentiment Dataset**
- Columns: `timestamp`, `value`, `classification`, `date`
- Shows historical sentiment: **Fear**, **Greed**, **Neutral**, etc.

### 2. 📈 **Hyperliquid Trader Data**
- Columns include: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Timestamp`, `Closed PnL`, etc.
- Logs individual trade executions over time

---

## ⚙️ Key Steps in the Project

1. **Data Cleaning & Parsing**
   - Converted UNIX timestamps (ms) into datetime
   - Extracted `date` for daily aggregation

2. **Merging Datasets**
   - Combined both datasets on `date`
   - Result: 184,263 records with sentiment labels per trade

3. **Exploratory Data Analysis (EDA)**
   - Analyzed profit/loss and trade volume by sentiment
   - Created boxplots and bar graphs for insights

---

## 📌 Key Insights

- ✅ **Average PnL** was highest on **Greed** days (`$87.89`), showing traders benefit most from positive momentum.
- 😱 **Fear** days saw **extremely high trade volumes** (`$704M+`), indicating emotional decision-making and volatility.
- 📉 **Neutral** and **Extreme Greed** days had lower activity and lower returns.
- 💡 Emotional market states like **Fear** and **Greed** drive significant shifts in trader behavior.

---

## 📁 Folder Structure
trader-sentiment-analysis/
│
├── charts/
│ ├── pnl_by_sentiment.png
│ └── volume_by_sentiment.png
│
├── trader_sentiment_analysis.ipynb
├── README.md
└── requirements.txt

---

## 🚀 How to Run

1. Clone the repo
2. Install dependencies (`pip install -r requirements.txt`)
3. Run `trader_sentiment_analysis.ipynb` in Jupyter Notebook

---

## 📬 Contact

For queries: sunayanawork6@gmail.com  
Let's build smarter trading strategies together!
