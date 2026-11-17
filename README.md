# WideTrail

[![make.fun](https://make.fun/badge/btc-race-24h-20261117-0603.svg)](https://make.fun/competitions/btc-race-24h-20261117-0603)
[![rank](https://make.fun/badge/btc-race-24h-20261117-0603/Masrukhan25/btc-race-24h-20261117-0603-entry-acct1/rank.svg)](https://make.fun/competitions/btc-race-24h-20261117-0603)
[![reward](https://make.fun/badge/btc-race-24h-20261117-0603/Masrukhan25/btc-race-24h-20261117-0603-entry-acct1/reward.svg)](https://make.fun/competitions/btc-race-24h-20261117-0603)

A BTC trading bot for the make.fun race "Race a BTC trading bot live for 24 hours" (btc-race-24h-20261117-0603).

WideTrail trades Coinbase Wrapped BTC (cbBTC) against USDC, minute by minute, long only, starting from $1,000 paper money. Two setups:

- **Setup B (capitulation-bounce sniper):** a deep fall from the 720-bar high (≥ 550 bps) plus a long lower-wick bar, a reversal bar that closes up ≥ 60 bps above the previous bar's high, RSI(14) turning up, and room back to the high at least twice the risk. The stop sits below the capitulation low, clamped to 50–100 bps under the entry.
- **Setup D (sharp-drop dip-buy):** the close fell ≥ 120 bps from the 120-bar high but is not a capitulation (720-bar fall under 550 bps), RSI(14) sits under 50, the close also fell ≥ 150 bps over the last 60 bars (a fast fall, close-to-close), and this bar closes up. Max 1 dip trade.

WideTrail exits with a wider trailing stop (arm/trail 90/90) and holds the dip up to 400 bars. Stops are set at decision time from the decision bar's close, never from the fill price.

Backtests (faithful harness replica): dev +$16.76, race (14–15 Nov) +$25.71, held-out (11 Binance windows) +$15.89.
