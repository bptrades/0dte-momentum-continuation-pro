# Momentum Continuation Pro Algo (0-DTE Friendly)

Rule-based momentum continuation indicator for TradingView, written in Pine Script v6.

This is a **confirmation and context tool**, not a signal generator.

---

## 📈 About

Momentum Continuation Pro Algo is designed to help traders identify continuation-style setups by evaluating structure, momentum, volume, and volatility.
The focus is *confirmation over prediction* — you trade only when conditions align, not when you hope they do.

This tool is released for **free use**.

---

## 🧠 Key Features

- EMA trend structure (fast vs slow)
- Optional VWAP filter
- Higher timeframe bias (15m) confirmation
- Volume and ATR-based strength filters
- Built-in time filter to reduce noise
- A+ and B setup scoring for trade quality

---

## 📊 How It Works

The script examines multiple confirmation inputs (EMAs, momentum, VWAP, volume, ATR, and HTF bias).  
When conditions align with high confidence, it marks:

- **A+ BUY / A+ SELL**  
- **B BUY / B SELL**

These labels are intended as *context confirmations*, not signals.

---

## ⏱️ Best Used When

- Market direction is clear
- Volume supports momentum
- You already have a bias / plan
- You use rules and risk controls

Avoid relying on this tool in:
- Low-volume drift
- Choppy range markets
- Random, late-session moves

---

## 📥 Installation (TradingView)

1. Open TradingView
2. Go to **Pine Editor**
3. Copy contents of `MomentumContinuationProAlgo.pine`
4. Paste into Pine Editor
5. Save and **Add to Chart**
6. Adjust inputs as needed

---

## 🛠️ Inputs (Defaults)

| Setting | Default |
|--------|---------|
| EMA Fast | 9 |
| EMA Slow | 21 |
| Volume MA Length | 20 |
| ATR Length | 14 |
| ATR Premium Protection | 0.75 |
| Use VWAP | true |
| Use 15m HTF Bias | true |

---

## ⚠️ Disclaimer

This script is provided for educational purposes and **is not financial advice**.
Trading involves risk. Use at your own risk.

Rules > indicators.  
Structure > emotion.

---

## 📄 License

This project is licensed under the MIT License — see `LICENSE` for details.
