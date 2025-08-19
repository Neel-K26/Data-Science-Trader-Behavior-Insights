# Trader Behavior vs Market Sentiment (Fear & Greed Index)

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1xL-CdjfxRAy37HnIJRWaCcDJ7WuOyhWq/view?usp=sharing)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📌 Overview
This project explores how trader profitability, risk, volume, and leverage align or diverge from market sentiment (Fear vs Greed).  

Completed as part of the **Web3 Trading Team – Data Science Assignment**.  

**Datasets analyzed:**  
1. **Bitcoin Market Sentiment Dataset** – daily sentiment classification (`Fear` / `Greed`) and index values.  
2. **Historical Trader Data (Hyperliquid)** – trade-level data (`execution price`, `size`, `side`, `closedPnL`, `leverage`, etc.).  

The analysis includes daily aggregation, feature engineering, visualizations, hypothesis testing, and predictive modeling using Random Forests.  

---

## 📂 Project Structure

```text
ds_Neel_Khairnar/ 🔹
├── 📓 notebook_1.ipynb          # Main analysis (Google Colab notebook)
├── 📓 notebook_2.ipynb          # Optional scratch / experiments
├── 📁 csv_files/                # Input & processed datasets
│   ├── fear_greed_index.csv     # Bitcoin market sentiment dataset
│   ├── historical_data.csv      # Hyperliquid historical trades
│   └── merged_features.csv      # Preprocessed & merged features for analysis
├── 📁 outputs/                  # Generated charts & plots
│   ├── correlation_heatmap.png
│   ├── pnl_volatility_by_sentiment.png
│   ├── trade_size_by_sentiment.png
│   ├── feature_importance.png
│   └── ...                      # Additional visualizations
├── 📝 report_outline.pdf        # Summarized report of analysis
└── README.md                    # Project documentation (this file)



---

## 🚀 How to Run
1. Open the [Google Colab Notebook](<INSERT LINK HERE>)  
   - Ensure that runtime has access to your **Google Drive**.  
   - Place datasets inside: `MyDrive/Dataset Folder/`  

2. Run all cells in order to reproduce results.  
   - Aggregates data by date  
   - Merges with sentiment  
   - Generates engineered features  
   - Produces visualizations & hypothesis tests  
   - Trains Random Forest classifier  

3. Outputs (plots, CSVs) are automatically saved in the `outputs/` folder.  

---

## 📊 Key Results
- **Hypothesis Test**: No significant difference in PnL between Fear vs Greed days.  
- **Model Performance** (RandomForest Classifier):  
  - Accuracy: ~75%  
  - ROC-AUC: ~0.69  
  - High recall for profitable days (~91%)  
- **Feature Importance**: PnL Volatility, Rolling Avg PnL, and Volume were most predictive.  

---

## 📈 Insights
- Sentiment alone is **not sufficient** for profitability prediction.  
- Combining sentiment with volatility & trading activity features improves predictive power.  
- Fear/Greed impacts **trading intensity** more than profitability.  

---

## 🔮 Future Improvements
- Add microstructure features (order book depth, intra-day volatility clusters).  
- Explore sequential models (LSTMs/Transformers) for temporal dynamics.  
- Extend dataset timeframe for more robust patterns.  

---

## 👤 Author
- **Name**: `<Neel Khairnar>`  
- **Contact**: `<neel.khairnar09@gmail.com>`  

