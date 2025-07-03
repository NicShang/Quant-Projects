# Portfolio Signal Optimization – Multi-Asset ETF Strategy

**Built a reusable portfolio optimization engine with real-world constraints, reflecting SIG’s research-to-production workflow.**

---

## What It Does

This Python project implements a **Sharpe-maximizing portfolio optimization framework** that mirrors how SIG turns ideas into production-ready tools:

- Class-based design for optimization using annualized returns, covariance matrices, and bounded weights.
- Institutional-style capital constraints (e.g. Core ≥ 65%, Satellite ≤ 15%) embedded directly into the optimization logic.
- CPI + 6% performance benchmark used as a realistic hurdle rate to test capital efficiency.
- 5,000 Monte Carlo simulations run to validate signal robustness under uncertainty.
- Visualized efficient frontier and max-Sharpe allocation using Plotly for decision-ready communication.

---

## Why It Matters

This was **not** coursework. It was designed to simulate SIG’s full research-to-deployment loop:

> **Idea generation → signal formulation → stress testing → capital allocation → visualization**

The engine is modular, extensible, and benchmark-aligned—capable of being adapted for different ETFs, constraints, or signal overlays.

---

## Key Features (Code Snippets)

**Sharpe Ratio Objective Function**

```python
def _negative_sharpe_ratio(self, weights):
    ret = self._portfolio_return(weights)
    std = np.sqrt(self._portfolio_variance(weights))
    return -(ret - self.risk_free_rate) / std
