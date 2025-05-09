# 📈 VN Listed Company's Stock Price Prediction

This project predicts stock prices of Vietnamese listed companies using both machine learning (ML) and deep learning (DL) models.  
It supports training multiple models across multiple stocks with full automation and evaluation.

---

## 🔍 Project Overview

The pipeline includes:

- ✅ Loading preprocessed historical stock data (`data/processed/`)
- 🧠 Training ML models: Linear Regression, KNN, Decision Tree, Random Forest, SVR
- 🔁 Training DL models: LSTM, GRU, BiLSTM, CNN, LSTM-CNN Hybrid
- 📊 Evaluating models using MAPE, RMSE, R², MAE, CVRMSE
- 📝 Generating a markdown report with table and chart

---

## 📁 Repository Structure

```
vn-stock-prediction/
├── data/
│   └── processed/                # Final cleaned data
├── reports/
│   ├── dl/, ml/                  # JSON results for each model
│   ├── model_summary.csv         # Combined results table
│   └── mape_top10.png            # Chart for top models
├── src/                          # Python modules
│   ├── features.py
│   ├── model.py
│   ├── preparation.py
│   └── utils.py
├── notebooks/
│   └── pipeline_demo.ipynb       # Interactive notebook to run full pipeline
├── main_multi_model.py           # Main training pipeline
├── summary_results.py            # Combine model scores into CSV
├── generate_report.py            # Create markdown report
├── plot_mape_top10.py            # Draw MAPE chart from summary
├── requirements.txt
└── README.md
```

---

## ▶️ How to Run

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Make sure you have `.csv` files in `data/processed/`

3. Run full pipeline:

```bash
python main_multi_model.py
python summary_results.py
python generate_report.py
python plot_mape_top10.py
```

---

## 📊 Libraries Used

- `pandas`, `numpy`, `matplotlib`
- `scikit-learn`, `tensorflow`
- `json`, `os`, `glob`

---

## 📈 Example Output

- 📄 Report: `report.md`
- 📊 Chart: `reports/mape_top10.png`
- 📋 Table: `reports/model_summary.csv`

---

## 📬 Contact

For questions or collaborations:

- 📧 Email: buudiem284@gmail.com
- 📞 Phone/Zalo: (+84) 812698938
