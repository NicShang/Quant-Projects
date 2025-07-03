# Quantitative Signal Discovery – ETF Portfolio Drawdown Research

*Simulated a full-cycle quant research project to identify downside patterns in ETF portfolios and convert them into predictive signals, aligned with institutional de-risking mandates.*

## Project Overview

This project builds a signal discovery pipeline aimed at identifying precursors to significant ETF portfolio drawdowns. The workflow replicates SIG’s research methodology—generating ideas from raw return/volatility data, testing hypothesis-driven signals, validating via backtest, and structuring the final model for modular reuse.

I hypothesized that short-term return/volatility dynamics predict 20-day drawdowns >5%. A logistic regression classifier confirmed this, achieving **100% sensitivity** and **0.98 AUC**, indicating robust signal detectability under realistic institutional scenarios.

## Key Features

- **Signal Discovery via Logistic Regression**  
  Tested hypothesis-driven features (short-term returns, volatility metrics) using logistic regression. Achieved high performance metrics to validate drawdown prediction logic.

- **Portfolio Construction & Scenario Simulation**  
  Constructed a synthetic multi-ETF portfolio aligned with Super Fund allocations. Simulated different asset compositions to test the signal’s generalizability.

- **Backtesting with VaR/ES**  
  Conducted Monte Carlo, parametric, and historical VaR/ES tests to benchmark the signal’s effectiveness under diversified and concentrated exposures, reflecting SIG’s focus on tail-risk understanding.

- **Visualization & Interpretability**  
  Generated interpretable visual outputs:
  - Signal timing overlay on portfolio returns
  - ROC/AUC curves
  - Temporal drawdown maps and signal accuracy tracking
  - Tail-risk distributions pre- and post-signal

- **Modular Python Stack**  
  Fully reproducible code using `scikit-learn`, `statsmodels`, `matplotlib`. Built to support future research, feedback iteration, and production-readiness, aligned with SIG’s infrastructure-first philosophy.

## Technical Stack

| Tool          | Purpose                                        |
|---------------|------------------------------------------------|
| `scikit-learn` | Signal classification and AUC evaluation      |
| `statsmodels`  | Time series preprocessing and diagnostics      |
| `numpy`        | Feature construction and simulation controls   |
| `matplotlib`   | Visualization of signal behavior and risk maps |

## Sample Output Highlights

- Drawdown signal vs event timeline charts  
- Feature contribution and signal heatmaps  
- VaR/ES output tables (single asset vs diversified)  
- Monte Carlo simulated risk surfaces

## Relevance to SIG

This project was designed with SIG’s real-world quantitative philosophy in mind:

- From **raw data** to **actionable signal**
- From **idea generation** to **risk-adjusted validation**
- From **hypothesis** to **production-ready research loop**

It demonstrates readiness for fast-paced signal iteration, modular testing, and alignment with performance-based decision making in a trading environment.

---
