# Crypto ETF Analysis

This is an empirical study of structural liquidity mismatches and Monday re-pricing effects
in spot crypto ETFs using high-frequency data. This repository contains the data and code used for the project.  

## Overview

The approval of U.S. spot Bitcoin ETFs in January 2024 integrated crypto assets into
traditional market infrastructure, but introduced a structural timing mismatch:
Bitcoin trades 24/7, while ETFs trade only during U.S. equity hours.

This project studies the market microstructure consequences of this mismatch using
5-minute high-frequency data from 2023–2025. I document a “Liquidity Vacuum” on
weekends, where institutional capital is absent and price discovery becomes fragile.
This vacuum leads to predictable volatility spikes at the Monday market open as ETFs
re-price accumulated weekend drift.

Using a Difference-in-Differences framework, I show that the weekday–weekend
volatility gap widened significantly post-ETF. I further identify a “Monday Morning
Heartbeat”: a sharp volatility surge around 9:30 AM EST that did not exist pre-ETF.
Evidence suggests that institutional flows initially *chase* weekend sentiment rather
than immediately correcting it.

## Paper

📄 **The Weekend Vacuum: Structural Liquidity Mismatches in Spot Crypto ETFs**  
Weirong Deng (2025)

The full paper, including theory, econometric methodology, figures, and robustness
checks, is available here:

- [`Crypto_ETF_Liquidity_Vacuum_Deng.pdf`](paper/Crypto_ETF_Liquidity_Vacuum_Deng.pdf)

## Notebooks

- **main.ipynb** – Analysis for Bitcoin (BTC).  
- **main copy.ipynb** – Analysis for Ethereum (ETH).  

## Structure

All supporting scripts, data, and figures are included in the repository. Run the notebooks in order to reproduce the results.  

## Notes

- Ensure all dependencies are installed (e.g., pandas, numpy, matplotlib, statsmodels).  
- Data files are assumed to be in the same folder as the notebooks.  

