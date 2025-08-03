# Option Pricing Engine – Python-Based Black-Scholes Risk Simulator

*Built a fully encapsulated Black-Scholes class in Python to simulate options pricing and Greeks behaviours under changing macro conditions.*

## Overview

This project implements a reusable and modular Black-Scholes pricing engine to compute analytical values and sensitivities (Greeks) for European call and put options. 

## Key Features

- **Modular Black-Scholes Class**  
  Constructed an object-oriented pricing engine that supports:
  - European call and put options
  - Dynamic user inputs (spot price, strike, rate, volatility, time)
  - Full Greek calculations: Delta, Gamma, Vega, Theta, Rho

- **Market Sensitivity Analysis**  
  Encoded option pricing sensitivity to market factors (spot, rate, volatility, time)

- **Surface Simulation**  
  Generated multi-dimensional pricing surfaces and Greek response maps to visualize convex risk behaviors and non-linear exposure patterns—crucial for identifying signal curvature and macro sensitivity.

- **Risk Dashboard Integration**  
  Visualized outputs using `matplotlib` and `tabulate`, simulating production-ready diagnostics for:
  - Stress testing
  - Hedge analysis
  - Trading overlays and signal interpretation

## Example Outputs

- Option price and Greeks at time of trade
- Cross-surface plots of Vega and Gamma vs. moneyness and time
- Tabular risk dashboards showing behavior under parameter shocks

## Why This Project Matters

This engine simulates how derivative exposures evolve under changing inputs, offering insight into:
- Convex risk behavior
- Signal resilience to macro volatility
- Real-time stress diagnostics
---
