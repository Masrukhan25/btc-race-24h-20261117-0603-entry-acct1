# BTC Race Bot — Sniper + Dip-Buy

[![Rank](https://make.fun/badge/btc-race-24h-20261117-0603/Masrukhan25/btc-race-24h-20261117-0603-entry-acct1/rank.svg)](https://make.fun/bounty/btc-race-24h-20261117-0603)
[![Reward](https://make.fun/badge/btc-race-24h-20261117-0603/Masrukhan25/btc-race-24h-20261117-0603-entry-acct1/reward.svg)](https://make.fun/bounty/btc-race-24h-20261117-0603)
[![Entries](https://make.fun/badge/btc-race-24h-20261117-0603/Masrukhan25/btc-race-24h-20261117-0603-entry-acct1/entries.svg)](https://make.fun/bounty/btc-race-24h-20261117-0603)

A long-only cbBTC trading bot for the [Race a BTC trading bot live for 24 hours](https://make.fun/bounty/btc-race-24h-20261117-0603) bounty. It trades two setups and otherwise stays in cash: Setup B, a capitulation-bounce sniper that buys the violent bounce after a multi-hour capitulation (drop >= 550 bps from the 720-bar high, long lower wick, sharp +60 bps reversal bar, RSI turning up, R:R >= 2:1, trailing stop +80/+80); and Setup D, a loose dip-buy for calm, range-bound windows that buys a dip of >= 120 bps off the 120-bar high when RSI(14) < 50 and the bar closes up, with an 80 bps stop and a +100/+100 trailing stop, capped at one dip trade per window. At most 3 trades per window, stop after 2 consecutive bounce losses, stop entering below 98% of starting equity, no entries after bar 1320.

## License

MIT — see [LICENSE](LICENSE).
