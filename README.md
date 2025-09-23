## Rupiah–USD Exchange Rate Analysis (Data Mining Project)

Predicting the Indonesian Rupiah (IDR) exchange rate against the US Dollar (USD) using Data Mining and Machine Learning (Linear Regression).

### 📌 Project Overview

Fluctuations in exchange rates play a critical role in Indonesia’s economy, influencing imports, exports, foreign debt, inflation, and investments. This project leverages data mining techniques and a Linear Regression model to predict the Rupiah–USD exchange rate by analyzing key economic indicators:

- **Kurs Transaksi USD**
- **Inflasi** (Inflation)
- **BI Rate** (Policy Rate)
- **Neraca** (Trade Balance)
- **Cadangan Devisa** (Foreign Exchange Reserves)

Data sources: Bank Indonesia and BPS.

### 🗂️ Repository Contents

- `Main.ipynb`: End-to-end notebook (data prep → modeling → evaluation)
- `Dataset.xlsx`: Source dataset used for analysis
- `Final Report.pdf`: Formal write-up of the study
- `Project presentation.pdf`: Slide deck summarizing the work

### ⚙️ Methodology

1. **Data Collection**
   - Gathered from official sources: Bank Indonesia and BPS.

2. **Preprocessing**
   - Data cleaning and handling of missing values
   - Feature engineering (e.g., Kurs Ratio, Trade Balance)
   - Encoding categorical features
   - Scaling numerical features with `RobustScaler`
   - Dimensionality reduction using `PCA` (retaining ~95% variance)

3. **Modeling**
   - Algorithm: **Linear Regression**

4. **Evaluation**
   - Metrics: **MAE**, **R²**, **RMSE**
   - **Cross-Validation** to assess generalization
   - Residual analysis to check model assumptions and fit

### 🧪 Results

- **R² (Accuracy)**: 0.9404 (~94.04%)
- **Cross-Validation (Mean R²)**: ~0.9435 (~94.35%)
- **RMSE**: ~477 IDR
- Residual analysis indicated no overfitting/underfitting.

### 🔮 Implications

- **Exporters/Importers**: Plan hedging and pricing strategies against currency fluctuations
- **Investors**: Anticipate risks related to Rupiah depreciation/appreciation
- **Policymakers**: Gain predictive insights for monetary and fiscal decision-making

### 🛠️ Tech Stack

- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

### ▶️ How to Run

1. Ensure you have Python 3.9+ installed.
2. Install dependencies (create a virtual environment if desired).

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

3. Launch Jupyter and open the notebook:

```bash
jupyter notebook Main.ipynb
```

4. Run all cells in order.

### 📈 What You’ll See in the Notebook

- Exploratory data analysis and visualizations
- Preprocessing: cleaning, encoding, scaling, PCA
- Model training: Linear Regression
- Evaluation with MAE, R², RMSE, and Cross-Validation
- Residual plots and diagnostics

### 📊 Notes on Features

- Engineered features include ratios and balances relevant to currency movement
- Scaling with `RobustScaler` provides robustness to outliers
- `PCA` reduces dimensionality while retaining ~95% of variance

### 🔁 Reproducibility

- Results may vary slightly due to randomness in cross-validation splits
- Set a random seed in the notebook if strict repeatability is required

### ⚠️ Limitations & Future Work

- Linear Regression provides a strong baseline but assumes linear relationships
- Future work: experiment with regularized models (Ridge/Lasso), tree-based models (Random Forest, XGBoost), and time-series models (ARIMA, Prophet, LSTM)
- Incorporate additional macroeconomic indicators and external shocks (e.g., commodity prices, Fed rate changes)

### 📚 References

- Bank Indonesia (BI) — Exchange Rates, Policy Rate, and Statistics: [`https://www.bi.go.id/`](https://www.bi.go.id/)
- Badan Pusat Statistik (BPS) — Inflation and Macroeconomic Indicators: [`https://www.bps.go.id/`](https://www.bps.go.id/)

### 📄 Citation

If you use this repository or build upon it, please cite the course project and authors appropriately.

---

For questions or collaboration, feel free to open an issue or reach out.


