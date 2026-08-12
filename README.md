# Monte Carlo Investment Risk Simulator

## Overview

This project uses Monte Carlo simulation to model the uncertainty of
investment outcomes over a 10-year period.

The model simulates 10,000 possible investment scenarios and analyses
the resulting distribution of final investment values.

The project was developed as an actuarial science programming project
to apply concepts from probability, financial mathematics, statistics,
and investment risk analysis.

## Objectives

The project aims to:

- Model uncertain investment returns using Monte Carlo simulation.
- Estimate the probability of reaching a financial investment target.
- Estimate the probability of ending below the initial investment.
- Analyse the effects of expected return and volatility.
- Examine the effect of inflation on purchasing power.
- Measure downside risk using percentile-based measures and Expected
  Shortfall.

## Model Assumptions

| Parameter | Value |
|---|---:|
| Initial investment | KSh 100,000 |
| Investment period | 10 years |
| Number of simulations | 10,000 |
| Expected annual return | 8% |
| Annual volatility | 15% |
| Annual inflation | 5% |
| Target investment value | KSh 200,000 |

Annual investment returns are generated from a normal distribution
using the assumed expected return and volatility.

## Analysis

The project includes:

### Monte Carlo Simulation

10,000 possible investment paths are generated to produce a
distribution of potential final investment values.

### Summary Statistics

The simulated outcomes are analysed using:

- Mean
- Median
- Standard deviation
- Percentiles

### Risk Analysis

The model estimates:

- Probability of reaching KSh 200,000.
- Probability of ending below the initial KSh 100,000 investment.
- 5% VaR-style downside threshold.
- 5% Expected Shortfall.

### Sensitivity Analysis

The model examines how investment outcomes change when:

- Expected annual return changes from 5% to 11%.
- Annual volatility changes from 5% to 25%.

### Inflation Analysis

Nominal investment values are converted into inflation-adjusted
(real) values to demonstrate the effect of inflation on purchasing
power.

## Key Findings

Under the original model assumptions:

- The estimated probability of reaching KSh 200,000 was approximately
  49%.
- The estimated probability of ending below the initial investment
  was approximately 8%.
- Higher expected returns increased the probability of reaching the
  investment target.
- Higher volatility increased the probability of loss.
- Inflation substantially reduced the purchasing power of nominal
  investment gains.

The exact results may vary slightly depending on the random simulation
and number of simulations used.

## Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook
- GitHub

## Project Structure

```text
Monte-Carlo-Investment-Risk-Simulator/
│
├── Monte_Carlo_Investment_Simulator.ipynb
├── README.md
└── .gitattributes