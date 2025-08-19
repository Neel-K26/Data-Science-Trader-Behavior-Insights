# Trader Behavior vs Market Sentiment (Fear & Greed Index)

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_NOTEBOOK_LINK)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Dataset](https://img.shields.io/badge/Dataset-Available-orange)](YOUR_DATASET_LINK)

## 📌 Overview
This project explores how trader profitability, risk, volume, and leverage align or diverge from market sentiment (Fear vs Greed).  

Completed as part of the **Web3 Trading Team – Data Science Assignment**.  

**Datasets analyzed:**  
1. **Bitcoin Market Sentiment Dataset** – daily sentiment classification (`Fear` / `Greed`) and index values.  
2. **Historical Trader Data (Hyperliquid)** – trade-level data (`execution price`, `size`, `side`, `closedPnL`, `leverage`, etc.).  

The analysis includes daily aggregation, feature engineering, visualizations, hypothesis testing, and predictive modeling using Random Forests.  

---

## 📂 Project Structure
ds_Neel_Khairnar/
├── notebook_1.ipynb # Main analysis (Google Colab notebook)
├── csv_files/ # Input & processed datasets
│ ├── fear_greed_index.csv
│ ├── historical_data.csv
│ └── merged_features.csv
├── outputs/ # Generated charts & plots
│ ├── correlation_heatmap.png
│ ├── pnl_volatility_by_sentiment.png
│ ├── trade_size_by_sentiment.png
│ ├── feature_importance.png
│ └── ...
├── report_outline.pdf # Summarized report of analysis


---

## 🚀 How to Run
1. Open the [Google Colab Notebook](YOUR_COLAB_NOTEBOOK_LINK)  
   - Ensure the runtime has access to your **Google Drive**.  
   - Place datasets inside: `MyDrive/Dataset Folder/`  

2. Run all notebook cells sequentially to reproduce results:  
   - Aggregate data by date  
   - Merge with sentiment index  
   - Generate engineered features  
   - Produce visualizations & perform hypothesis testing  
   - Train a Random Forest classifier  

3. All outputs (plots, CSVs) are saved automatically in the `outputs/` folder.  

---

## 📊 Key Results
- **Hypothesis Testing**: No significant difference in PnL between Fear vs Greed days.  
- **Random Forest Model Performance**:  
  - Accuracy: ~75%  
  - ROC-AUC: ~0.69  
  - High recall for profitable days (~91%)  
- **Feature Importance**: PnL Volatility, Rolling Avg PnL, and Trading Volume were most predictive.  

---

## 📈 Insights
- Sentiment alone is **not sufficient** for predicting profitability.  
- Combining sentiment with volatility & trading activity metrics improves predictive power.  
- Fear/Greed influences **trading intensity** more than profitability.  

---

## 🔮 Future Improvements
- Incorporate microstructure features (order book depth, intra-day volatility clusters).  
- Explore sequential models (LSTMs, Transformers) for temporal patterns.  
- Extend dataset timeframe to identify more robust trends.  

---

## 👤 Author
- **Name**: Neel Khairnar  
- **Email**: neel.khairnar09@gmail.com  
 
