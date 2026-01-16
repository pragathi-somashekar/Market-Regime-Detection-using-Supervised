📌 **Overview**

This project builds supervised machine learning models to classify **bull** and **bear** market regimes using **pre-market financial and macroeconomic indicators**.
The goal is to evaluate whether ML models can detect downturns early and help support **risk-aware investment decision-making**.

The study uses **5,822 daily observations (2002–2025)** and incorporates equity, volatility, fixed-income, and macroeconomic features.


📂 **Data Sources**

* **Yahoo Finance** – SPY, VIX, TLT
* **FRED (Federal Reserve Economic Data)** – Yield curve (10Y–3M spread), credit spread
* Features include: SPY returns (lagged), VIX, yield curve, credit spread, TLT/SPY ratio, and macro indicators.


🔍 **Key Steps**

* **Data cleaning & preparation**
* **Handling class imbalance** (SMOTE–Tomek on training set)
* **Time-based train/validation/test split**
* **Feature scaling to prevent leakage**
* **Extensive Exploratory Data Analysis (EDA)**
* Rolling means, regime-wise distributions, outlier analysis, correlations


🤖 **Models Implemented**

* Logistic Regression
* LASSO Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

All models are evaluated using:

* **ROC-AUC**
* **Confusion matrices**
* **Regime-specific recall** (with special focus on bear markets)


📈 **Results**

* VIX, TLT/SPY ratio, and yield curve were the most influential predictors.
* Tree-based models (Random Forest & XGBoost) performed best at identifying **bear markets**, despite overall class imbalance.
* ML models showed strong potential in **regime-aware investment strategies** and **downside risk management**.


📌 **Conclusion**

The project demonstrates that supervised machine learning models can effectively classify market regimes and identify market downturns using only **pre-market data**.
This highlights the potential for ML-driven decision support in portfolio risk management.


📁 **Repository Includes**

* Data preprocessing scripts
* EDA notebooks
* Model training and evaluation code
* Visualizations for each modeling step
* Full PDF report


✨ **Tech Stack**

* Python
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib, Seaborn
* Jupyter Notebook
