# Pricing-Vanilla-Options-with-Cash-Dividends
This repository contains a replication and practical implementation of the paper:
“Pricing Vanilla Options with Cash Dividends” by Timothy R. Klassen (2015) 

The paper addresses one of the most debated topics in option pricing: how to extend the Black–Scholes framework to underlyings that pay discrete cash dividends.

# Paper Summary

In markets with dividend-paying underliers (stocks, ETFs, indices), pricing vanilla options becomes non-trivial. The paper explores different approaches:

## Spot Model (piecewise GBM) – assumes the stock price follows GBM between ex-dividend dates with jumps at dividend times.

## Hybrid Models (shifted GBM) – forward-adjusted models that incorporate dividends into a shifted stochastic process.

## Full Hybrid Model (FHM)

## Partial Hybrid Model (PHM, aka Escrowed Dividend Model)

## Spot-Strike Adjustment Model (SKA)

## Comparison of Models – in terms of arbitrage properties, calibration ease, volatility surfaces, and computational efficiency.

The paper further develops tree-based methods for accurate and fast pricing of American and European vanilla options under dividend assumptions.

# Implementation

This repo replicates and extends the paper by:

Implementing European and American option pricing with discrete cash dividends.

Comparing Spot vs Hybrid models on consistency, arbitrage conditions, and computational speed.

Using binomial/trinomial tree methods (Leisen-Reimer tree implementation for efficiency).

Providing calibration routines for implied volatilities and borrow rates.

Visualizing differences in implied vol surfaces across models.

## References

Klassen, T. R. (2015). Pricing Vanilla Options with Cash Dividends. SSRN: http://ssrn.com/abstract=2634051
