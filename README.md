# The Elements of Quantitative Investing: 7-Day Implementation Sprint

This repository contains a 7-day guided implementation of **"The Elements of Quantitative Investing"** by Giuseppe A. Paleologo. 

The goal of this project is to bridge advanced structural portfolio theory with practical, vectorized Python implementation. Rather than just summarizing the math, each day translates specific quantitative architectures—from linear factor models to covariance shrinkage and factor-mimicking portfolios—into executable code. It is designed as a tactical extraction of the text for applied quantitative research and structural portfolio engineering.

## 🛠️ Tech Stack
* **Language:** Python
* **Environment:** Jupyter Notebooks / Google Colab
* **Key Libraries:** `numpy`, `pandas`, `statsmodels`, `scikit-learn` (Covariance), `arch` (Volatility modeling), `yfinance`

## 📅 The 7-Day Architecture

Each folder contains a standalone Colab notebook with theoretical notes, mathematical translations, and a self-contained mini-project.

| Day | Topic | Key Concepts | Implementation Project |
| :--- | :--- | :--- | :--- |
| **Day 1** | Foundations & The Linear Model | Log returns, Stylized Facts, GARCH(1,1), Spanned vs. Orthogonal Alpha. | Extracting market beta and modeling idiosyncratic heavy-tail residuals using OLS and GARCH. |
| **Day 2** | Covariance Math & The Structural Shift | Failure of empirical covariance, Condition Numbers, Ledoit-Wolf Shrinkage, The Precision Matrix. | Building a multi-asset matrix and proving the mathematical stability of shrinkage estimators in high dimensions. |
| **Day 3** | Fundamental Factor Models | Cross-sectional regressions, Dummy variables, Characteristic-based factors. | Engineering a structural multi-factor model for a thematic equity basket. |
| **Day 4** | Statistical Models & Backtesting | Principal Component Analysis (PCA), Rank deficiency, Cross-validation without data snooping. | Extracting purely statistical factors via PCA and contrasting them with fundamental models. |
| **Day 5** | Portfolio Optimization | Mean-Variance Optimization (MVO), Handling estimation errors, Constraints as Bayesian priors. | Building a covariance optimization engine to balance structural risk contributions. |
| **Day 6** | The Friction of Reality | Transaction cost models (Frobenius norms), Market impact, Hedging. | Constructing Factor-Mimicking Portfolios (FMPs) to isolate pure orthogonal alpha. |
| **Day 7** | Sizing, Allocation & Attribution | The Kelly Criterion, Fractional Kelly, Ex-post PnL attribution. | Decomposing backtested returns into timing, stock selection, and factor exposure. |

## 🚀 How to Use This Repository

All code is designed to run seamlessly in Google Colab. To explore a concept:
1. Navigate to the respective Day's folder.
2. Open the `.ipynb` file.
3. Click the **"Open in Colab"** badge at the top of the notebook (if configured) or upload directly to your Colab environment.
4. Run the cells sequentially to pull live market data and visualize the matrix transformations.

## 📖 Reference
* Paleologo, Giuseppe A. *The Elements of Quantitative Investing*.
