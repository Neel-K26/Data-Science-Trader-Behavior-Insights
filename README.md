
# Trader Behavior vs Market Sentiment (Fear & Greed Index)

## 📌 Overview
This project analyzes how trader profitability, risk, volume, and leverage align or diverge from market sentiment (Fear vs Greed).  
It was completed as part of the **Web3 Trading Team – Data Science Assignment**.  

Two datasets were analyzed:
1. **Bitcoin Market Sentiment Dataset** – containing daily sentiment classification (`Fear` / `Greed`) and index values.  
2. **Historical Trader Data (Hyperliquid)** – containing trade-level data (`execution price`, `size`, `side`, `closedPnL`, `leverage`, etc.).  

---

## 📂 Project Structure
ds_<Neel Khairnar>
├── notebook_1.ipynb # Main analysis (Google Colab notebook)
├── notebook_2.ipynb # (Optional) experiments / scratch work
├── csv_files/ # Input & processed datasets
│ ├── fear_greed_index.csv
│ ├── historical_data.csv
│ └── merged_features.csv
├── outputs/ # Saved charts & plots
│ ├── correlation_heatmap.png
│ ├── pnl_volatility_by_sentiment.png
│ ├── trade_size_by_sentiment.png
│ ├── feature_importance.png
│ └── ...
├── report outline.pdf # Final summarized report



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


