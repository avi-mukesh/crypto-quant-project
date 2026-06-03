# Crypto Cross-Sectional Momentum

Systematic signal research and strategy development for cryptocurrency markets using hourly Binance data (2022–2026).

## Overview

Three signals are investigated as cross-sectional predictors of relative returns:

- **Tweet share momentum** — each coin's share of Twitter mentions across the universe. A 7-hour lag shows consistent cross-sectional IC of 0.012–0.016 across years, suggesting retail attention precedes price movement.
- **Taker imbalance** — net aggressive buying/selling pressure. Shows modest time-series predictability but limited value as a cross-sectional ranking signal.
- **Price momentum** — 2-week return identified as the optimal lookback via IC analysis across windows from 5 to 85 days.

The primary strategy is a long/short cross-sectional price momentum strategy holding ~50% of the universe, with a BTC regime filter that dampens short exposure during bull markets.

## Data

- **Price data**: Hourly OHLCV from Binance
- **Tweet data**: Hourly mention counts via Twitter API
- **In-sample**: 2022–2024, 8 coins (BTC, ETH, SOL, ADA, BNB, LINK, SHIB, DOGE)
- **Out-of-sample**: Jan 2025–May 2026, 17 coins

## Validation

Walk-forward validation, parameter sensitivity analysis, and out-of-sample testing on an expanded 17-coin universe drawn from the top 35 by market cap on CoinMarketCap (May 2026).

## Requirements

```bash
pip install seaborn xdk pandas numpy matplotlib python-binance
