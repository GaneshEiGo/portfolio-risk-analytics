# portfolio-risk-analytics

# Global Portfolio Risk & Performance Analytics System

## Executive Summary

This project builds a quantitative portfolio optimization engine that analyzes a diversified basket of Indian and US equities to identify the most efficient capital allocation under risk constraints. 

Using Monte Carlo simulation (10,000 portfolio combinations), the system evaluates risk-return tradeoffs and determines the Maximum Sharpe Ratio portfolio. The final output includes a structured capital allocation strategy for a ₹10,00,000 investment and a Power BI dashboard for executive-level interpretation.

This project combines financial mathematics, statistical modeling, and business-focused visualization.

---

## Business Context

Investors constantly face a fundamental challenge:

How do we maximize expected return while controlling portfolio risk?

Diversification across markets (India + US) can reduce volatility, but optimal allocation is not intuitive. This project solves that problem using quantitative simulation rather than guesswork.

The goal is to:

- Model portfolio risk mathematically
- Simulate thousands of allocation possibilities
- Identify the most efficient portfolio
- Translate results into actionable capital distribution

---

## Methodology & Technical Approach

### 1. Data Collection
- Retrieved 5 years of historical adjusted closing prices
- Included large-cap Indian equities (NSE) and major US technology stocks
- Benchmarked against NIFTY 50 and S&P 500

### 2. Return & Risk Computation
- Calculated daily log returns
- Annualized returns using 252 trading days
- Constructed covariance matrix to model asset interdependence

### 3. Monte Carlo Simulation
- Generated 10,000 random portfolio weight combinations
- Computed:
  - Expected Annual Return
  - Annual Volatility
  - Sharpe Ratio (risk-adjusted performance)

### 4. Efficient Frontier Construction
- Mapped return vs volatility tradeoffs
- Identified Maximum Sharpe Portfolio
- Visualized optimal boundary

### 5. Capital Allocation Simulation
- Applied optimal weights to ₹10,00,000 capital
- Generated real investment allocation by asset
- Evaluated diversification benefits

---

## Key Insights

- Cross-market diversification reduced overall volatility relative to concentrated exposure.
- The Maximum Sharpe portfolio achieved superior risk-adjusted performance compared to equal-weight allocation.
- Efficient Frontier analysis visually demonstrates diminishing returns at higher risk levels.
- Quantitative allocation outperforms intuitive portfolio construction.

---

## Tools & Technologies

- Python (Pandas, NumPy)
- Statistical Modeling
- Monte Carlo Simulation
- Portfolio Optimization Logic
- Power BI (Executive Dashboard Visualization)

---

## Dashboard Overview

The Power BI dashboard presents:

- Efficient Frontier visualization
- Risk-adjusted performance metrics
- Optimal capital allocation breakdown

---

## Why This Project Matters

This is not just a visualization project.

It demonstrates:

- Quantitative financial reasoning
- Risk modeling capability
- Statistical simulation
- Optimization thinking
- Business interpretation of analytical results

The system can be extended to:
- Add transaction costs
- Include risk-free rate modeling
- Perform rolling backtests
- Integrate automated rebalancing strategies

---

## Future Enhancements

- Dynamic portfolio rebalancing simulation
- Rolling volatility and drawdown analysis
- Scenario-based stress testing
- Integration with live market APIs
