# All-Weather Portfolio Construction via Macro-Informed Optimization

## Overview
This project analyzes 50+ years of monthly return data across 11 asset classes including US and International Stocks, Bonds, Commodities, and Corporate Credit.  
Using a global macro framework, the research uncovers key market regimes and provides actionable insights for building durable, risk-adjusted portfolios that can perform across economic cycles.

The study integrates:
- Portfolio optimization
- Macroeconomic analysis
- Historical backtesting

to guide the construction of resilient investment strategies.

---

## Key Contributions
- **50-Year Historical Analysis**: Optimized portfolios across major asset classes from 1970–2024 using a variety of time-frames and assets. 
- **Global Macro Lens**: Evaluation of asset returns in different macroeconomic environments (growth/inflation regimes) with special attention to asset correlations through time.
- **Custom All-Weather Portfolio**: Diversified mix that consistently outperforms the traditional 60/40 portfolio, especially in crises.

---

## Methodology
- Collected macroeconomic (GDP, CPI from FRED) and financial asset data from 1970–2024.
- Built Python classes for portfolio optimization (`scipy.minimize`) and return analysis.
- Rolling-window Sharpe-maximizing optimizations with unlevered, long-only portfolios.
- Take lessons from portfolio optimization study to develop All-Weather Portfolio.
- Statistical validation of Sharpe outperformance via bootstrapping (100k samples) following Ledoit & Wolf (2008).

---

## Key Insights
- **Diversification Wins**: Blending equities, rates, credit, and commodities improves long-term risk-adjusted performance.
- **Gold as Crisis Hedge**: Optimal portfolios heavily allocate to gold in inflation/recessionary periods.
- **More Allocation to Fixed Income**: Optimizing for risk-adjusted returns, portfolios consistently put more than 40% exposure in bond to maximize Sharpe Ratio.
- **Corporate Credit Alpha**: Investment Grade and High Yield credit provide strong diversification benefits due to unique correlation properties with stocks (S&P 500) and bonds (UST 10Y)
- **International Assets Lag**: Optimizations generally avoid FTSE, Nikkei, Gilts, and JGBs when USD-adjusted
- **Declining Bond Hedge**: Treasuries’ hedging power has weakened in recent years after rates hit the zero lower bound

---

## Custom All-Weather Portfolio
Based on historical insights, we propose a resilient allocation:

| Asset Class | Weight |
|-------------|--------|
| Gold        | 20%    |
| S&P 500     | 35%    |
| US 10Y      | 30%    |
| US IG Credit| 10%    |
| US HY Credit| 5%     |

Performance vs. 60/40 (1997–2024):

| Portfolio | Ann. Return | Ann. Volatility | Sharpe | Max Drawdown |
|-----------|-------------|-----------------|--------|--------------|
| 60/40     | 6.46%       | 7.63%           | 0.85   | -28.2%       |
| Custom    | 6.63%       | 5.65%           | 1.17   | -16.7%       |

---

## Getting Started
1. Review the [PDF summary](./Macro_Project_Summary.pdf) for a deep dive into findings.
2. Explore the Jupyter Notebook in this repo to:
   - Run the optimizer
   - Build your own custom portfolios
   - Analyze historical returns under different assumptions

---

## Next Steps
- Incorporate additional assets (EM, REITs, TIPs, Bitcoin, etc.).
- Explore tactical/ML-driven models for regime forecasting.
- Publish modular Python package for portfolio construction and stress testing.

---

## Contact
For questions or collaboration opportunities:  
📧 gguentherny@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/gus-guenther/) | [GitHub](https://github.com/guenther-QR)

---

*For research/discussion only. Not investment advice.*
