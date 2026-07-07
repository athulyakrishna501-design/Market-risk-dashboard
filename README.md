# Market Risk Dashboard — Quantitative Methods

A multi-asset market risk analytics notebook implementing core quantitative risk methods used by risk desks at investment banks and asset managers.
<img width="1328" height="490" alt="image" src="https://github.com/user-attachments/assets/21814057-9508-48c4-ac19-ff0c6c154aea" />


## Quantitative Methods Covered

| Method | Description |
|--------|-------------|
| **Historical VaR** | Non-parametric Value at Risk from empirical return distribution |
| **Parametric VaR** | Variance-covariance VaR assuming normal returns |
| **Monte Carlo VaR** | Simulated VaR using correlated multivariate normal draws |
| **Expected Shortfall (CVaR)** | Average loss beyond VaR threshold (Basel III preferred measure) |
| **EWMA Volatility** | Exponentially weighted volatility (JP Morgan RiskMetrics, λ=0.94) |
| **Correlation Analysis** | Static and rolling correlation across asset classes |
| **Stress Testing** | Hypothetical scenario analysis (equity crash, rate shock, etc.) |
| **Component VaR** | Risk decomposition by asset for risk budgeting |

## Portfolio

Multi-asset universe covering three asset classes:

- **Equities:** S&P 500 (SPY), International Developed (EFA), ASX 200 (STW.AX)
- **Fixed Income:** US Long Treasury (TLT), US Aggregate Bond (AGG)
- **Commodities:** Gold (GLD), Oil (USO)

## Setup

```bash
pip install -r requirements.txt
jupyter notebook market_risk_dashboard.ipynb
```

## Key Outputs

- VaR comparison across three methodologies at 90%, 95%, 99% confidence
- Expected Shortfall tail risk analysis
- EWMA vs rolling volatility time series
- Correlation heatmap and rolling correlation dynamics
- Stress test scenario impact analysis
- Component VaR risk decomposition with weight vs risk contribution charts
- Executive risk dashboard summary

## Tech Stack

Python · NumPy · Pandas · SciPy · yfinance · Matplotlib · Seaborn

## Author

Athu — Master of International Economics & Finance, University of Queensland
