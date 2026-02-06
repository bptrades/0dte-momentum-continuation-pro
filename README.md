# Momentum Continuation Pro Algo (0-DTE Momentum Continuation Pro v4)

Rule-based momentum + structure confirmation indicator for TradingView (Pine Script v6).

**This is NOT a signal service.**
It’s a decision-support tool designed to help identify **momentum continuation conditions** and avoid low-quality chop.

---

## What it’s designed for
- Momentum continuation trades (not reversals)
- Intraday trading, including 0-DTE style momentum windows
- Traders who already use rules + risk management
- Filtering low-quality trades (saying “NO” more than “YES”)

---

## What it checks (high-level)
- EMA structure alignment (fast vs slow)
- Momentum relative to EMAs
- VWAP positioning (optional)
- Volume confirmation vs volume MA
- ATR expansion vs ATR MA
- Higher timeframe bias (15m EMA alignment, optional)
- Time-of-day filter (built-in)

---

## Setup quality labels
- **A+ BUY / A+ SELL**: Strong alignment across structure + momentum + VWAP + HTF bias + candle strength  
- **B BUY / B SELL**: Momentum present, but missing strength components (requires discretion)

---

## Time filter (important)
The script includes a time filter to focus on higher-quality intraday windows and reduce noise.
This is intentional to help prevent overtrading.

---

## When NOT to use this
- Choppy / range-bound market conditions
- Low-volume drift
- As a standalone system without a risk plan
- If you’re chasing candles

No indicator replaces discipline.

---

## Risk & exit logic
The script tracks a position state and resets when:
- Momentum breaks (price crosses EMA fast against you)
- VWAP flips against you (if enabled)
- ATR-based protection threshold is hit

You still must control:
- Position sizing
- Max loss rules
- Daily trade limits

---

## How to install (TradingView)
1. Open TradingView
2. Go to **Pine Editor**
3. Copy the code from `MomentumContinuationProAlgo.pine`
4. Paste into Pine Editor
5. Click **Add to Chart**
6. Adjust settings (EMA lengths, VWAP/HTF toggles) as desired

---

## Inputs (defaults)
- EMA Fast: 9
- EMA Slow: 21
- Volume MA Length: 20
- ATR Length: 14
- ATR Premium Protection: 0.75
- Use VWAP: true
- Use 15m HTF Bias: true

---

## Disclaimer
This software is provided for educational purposes only and **is not financial advice**.
Trading options involves significant risk. Use at your own risk.
