# Mamba-inspired 1-Minute Deriv Scalper

A mobile-first, DEMO-only Deriv Rise/Fall scalper based on a public-rule reconstruction of the MambaFx one-minute setup.

## Strategy reconstruction
- M5 EMA(50) directional filter.
- M1 breakout above/below the previous 10 completed one-minute candles.
- 1-minute Deriv contract expiry only. If Deriv rejects that duration, the bot skips the trade rather than silently extending expiry.
- Automatic stake sizing, one open contract maximum, no martingale.

## Important limitations
This is not an official MambaFx bot and is not an exact copy of the original spot-FX strategy. Deriv Rise/Fall contracts do not provide the same swing stop-loss and 1:3 take-profit structure. The app defaults to DEMO and blocks non-virtual accounts.

## Run
GitHub Pages serves `index.html` from the repository root. Enter a Deriv DEMO API token and App ID in the app; the token is held in memory and is not saved.

The strategy is a research reconstruction and is not verified profitable. Forward-test in DEMO before considering any real-money use.
