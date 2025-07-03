# Volatility Risk Forecasting – Visa Inc. Signal Stress Test

*Built a forward-looking volatility model to uncover tail-risk exposures, replicating SIG-style GARCH signal analysis and backtest cycles.*

---

## Project Overview

This project simulates a quantitative research process for a hedge fund client holding Visa Inc. (V) stock. It builds and validates a GARCH-based volatility forecasting model to uncover early-warning drawdown signals and quantify tail risk under market stress.

Inspired by SIG’s production-style quant research loop—idea generation, signal testing, scenario analysis, and validation—this project integrates forecasting, Monte Carlo stress testing, and robustness diagnostics into a modular Python workflow.

---

## Key Features

- **Dynamic Volatility Modelling**  
  Engineered an AR(6)-GARCH(3,7) model to forecast daily volatility, mimicking SIG’s dynamic regime modelling logic.

- **Risk Metrics**  
  Estimated Value-at-Risk (VaR) and Expected Shortfall (ES) under multiple confidence levels to assess drawdown risk in portfolio exposure.

- **Monte Carlo Stress Testing**  
  Simulated 10,000+ potential return paths using GARCH residuals to evaluate model performance under extreme uncertainty.

- **Historical Benchmarking**  
  Compared predicted VaR thresholds against real market exceedances to assess signal reliability and tune model alerts.

- **Diagnostic Testing**  
  Applied Jarque-Bera (normality), Ljung-Box (autocorrelation), and kurtosis/skewness checks to validate model assumptions and structure.

- **Fully Automated Python Pipeline**  
  Built using `arch`, `statsmodels`, `matplotlib`, and `seaborn`, emphasizing modular code and clear visualization—aligned with SIG’s emphasis on clarity, replicability, and production-readiness.

---

## Outputs

- Daily VaR and ES curves with exceedance highlighting  
- Monte Carlo drawdown distribution charts  
- Model diagnostic test summaries  
- Modular Python implementation for adaptation to other assets

---

## Skills Demonstrated

- Time series modeling (ARIMA, GARCH)  
- Risk diagnostics (VaR, Expected Shortfall)  
- Scenario-based analysis using simulation  
- Quant research thinking aligned with SIG-style production pipelines

---

## File Structure

- `Visa Inc. Risk Modelling.ipynb` – Main analysis and modelling notebook  
- `data/` – Historical price data for Visa Inc.  
- `plots/` – Output charts and simulation visualizations  

---
