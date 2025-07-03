# Latent Factor Decomposition – Yield Curve PCA on Bond ETFs

_Explored market structure signals using PCA on Australian government bond ETFs, aligning with SIG’s interest in dimensionality reduction and market regime modelling._

## Project Objective
To simulate trader-style yield curve signal decomposition by applying PCA to real bond ETF data, identifying latent macro factors (level, slope, curvature) and stress-testing their predictive value under regime shifts.

---

## Key Features & Methodology

- **Applied PCA decomposition** to yield curve movements using ASX-listed bond ETFs (`GOVT.AX`, `VGB.AX`, `IBL.AX`), extracting latent structure through eigenvalue analysis to mimic trader-style interpretation of macro shifts.
- **Preprocessed real-world ETF data**, implementing log return transformation and missing data imputation to prepare noisy time series for signal extraction under production-style constraints.
- **Visualized PCA time series** to highlight curve regime shifts, volatility clustering, and structural changes, mirroring SIG’s interest in regime-sensitive signal generation.
- **Engineered a reusable PCA pipeline** using `sklearn` and `plotly`, allowing modular experimentation and clear signal visual diagnostics for feedback-driven iteration.
- **Highlighted live signal use cases**, including flattening/steepening detection and volatility stress overlays—demonstrating how latent factor models support real-time signal monitoring and risk overlays in quant trading.

---

## Tech Stack
- **Python**, `scikit-learn`, `pandas`, `plotly`, `numpy`, `yfinance`
- Jupyter Notebook format (reusable and extensible)
- Designed to simulate production-style PCA signal testing and visualization cycles

---

## Sample Outputs
- Eigenvalue scree plots and cumulative variance
- Level, Slope, Curvature component evolution
- Interactive trend breakdowns and drawdown overlays

---

## SIG-Relevant Skills Demonstrated
- Dimensionality reduction in financial time series  
- Trader-style interpretation of rate regimes using macro data  
- Modular pipeline construction aligned with signal discovery and iteration  
- Visualization tailored for real-time monitoring and post-deployment diagnostics  

---

## Future Work
- Integration with macroeconomic indicators (e.g., CPI, GDP prints)  
- Cross-validation using forward walk and rolling-window PCA  
- Stress-testing factors under monetary policy shift scenarios

---
