# 📊Rupiah-to-USD-Exchange-Rate-Analysis---Data-Mining-Project
This project is a Data Mining and Machine Learning study that aims to predict the Indonesian Rupiah (IDR) exchange rate against the US Dollar (USD) using Linear Regression. The work was conducted as part of the Data Mining course.

**📌 Project Overview**
Fluctuations in exchange rates play a critical role in Indonesia’s economy, influencing imports, exports, foreign debt, inflation, and investments.
This project leverages data mining techniques and a Linear Regression model to predict the Rupiah–USD exchange rate by analyzing key economic indicators such as:
-Kurs Transaksi USD
-Inflasi
-BI Rate
-Neraca
-Cadangan Devisa

**⚙️ Methodology**
**Data Collection**: Data obtained from Bank Indonesia
 and BPS

**Preprocessing**:
-Data cleaning & missing value handling
-Feature engineering (e.g., Kurs Ratio, Trade Balance)
-Encoding categorical features
-Scaling numerical features with RobustScaler
-Dimensionality reduction using PCA (95% variance retained)

**Modeling**: Linear Regression

**Evaluation**:
-*Metrics*: MAE, R², RMSE
-Cross Validation to ensure model generalization

**📈 Results**

**Accuracy (R²)**: 94.04%
**Cross Validation**: 0.94 (mean 94.35%)
**RMSE**: ~477 IDR

**Residual analysis confirmed no overfitting/underfitting.**

**🔮 Implications**
-Helps exporters/importers plan financial strategies against currency fluctuations.
-Supports investors in anticipating risks related to Rupiah depreciation/appreciation.
-Provides policymakers with predictive insights for monetary and fiscal decision-making.

**🛠️ Tech Stack**
-Python
-Pandas, NumPy, Scikit-learn
-Matplotlib, Seaborn for visualization
