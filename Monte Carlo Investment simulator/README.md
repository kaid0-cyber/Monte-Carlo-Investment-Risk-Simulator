# Monte Carlo Investment Risk Simulator

## Overview

This project uses Monte Carlo simulation to model possible investment
outcomes over a 10-year period.

The model simulates 10,000 possible investment paths using assumptions
for expected annual return and volatility. The resulting outcomes are
analysed using statistical and risk measures.

## Objectives

- Estimate the probability of reaching a KSh 200,000 investment target.
- Estimate the probability of ending below the initial investment.
- Analyse the distribution of possible final investment values.
- Investigate the effect of expected return and volatility.
- Analyse the effect of inflation on purchasing power.
- Calculate percentile-based risk measures, including VaR and
  Expected Shortfall.

## Model Assumptions

- Initial investment: KSh 100,000
- Investment period: 10 years
- Number of simulations: 10,000
- Expected annual return: 8%
- Annual volatility: 15%
- Inflation rate: 5%
- Annual returns are assumed to be normally distributed.
- Annual returns are assumed to be independent.
- Investment fees, taxes and withdrawals are excluded.

## Key Results

The model estimated:

- Probability of reaching KSh 200,000: 49.21%
- Probability of ending below KSh 100,000: 7.91%
- Mean final investment value: KSh 216,997
- Median final investment value: KSh 197,944
- 5th percentile: KSh 89,639
- 95th percentile: KSh 408,818
- 5% VaR-style threshold: KSh 89,639
- 5% Expected Shortfall: KSh 75,123

## Sensitivity Analysis

The project examines how changes in:

1. Expected annual return
2. Annual volatility

affect the probability of reaching the investment target and the
probability of experiencing a loss.

## Inflation Analysis

The model also converts nominal investment values into
inflation-adjusted values to demonstrate the effect of inflation on
purchasing power.

## Tools

- Python
- NumPy
- Matplotlib
- JupyterLab
- Anaconda

## Limitations

The model is a simplified representation of investment behaviour.
Actual financial returns may not be normally distributed and may
exhibit changing volatility, dependence between periods, skewness
and extreme events.

Inflation is also assumed to be constant rather than stochastic.

## Conclusion

The project demonstrates how Monte Carlo simulation can be used to
model uncertainty and quantify investment risk. It combines
probability, financial mathematics, statistics and programming to
analyse a range of possible investment outcomes.