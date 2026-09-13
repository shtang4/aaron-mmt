# 03 — How To Enter Market With The Right Direction

Source: Module 3 slides, Momentum Mastery Trading (MMT), Dr. Aaron MMT, 2026.

Module contents (from the section title slide):

- Heikin-Ashi (平均蜡烛图)
- 3 Main Indicators (三大主要指标)
- Add-on SMC indicator (添加SMC指标)
- Advance tool: New Indicators (添加新指标)
- Trend line, Support & Resistance, Tunnel trend line
- Seahorse pattern

## 1. Heikin-Ashi (平均蜡烛图)

### 1.1 Definition table

Transcribed from the slide.

| Aspect | Description |
|--------|-------------|
| Type | Candlestick charting technique |
| Purpose | Identify trends and potential reversals |
| Smoothing effect | Smooths out price data to reduce noise |
| Calculation | Based on the previous candle's data |
| Candle components | Open: average of the previous open and close. Close: average of open, high, low and close. High: highest price during the period. Low: lowest price during the period. |
| Trend identification | Bullish (green) for uptrends, bearish (red) for downtrends |
| Reversal signals | Change from bullish to bearish or vice versa |
| Gaps | Fewer gaps compared to traditional candles |
| Support / resistance | Used to identify key price levels |
| Usefulness | Helps filter out noise and emphasise trends |
| Caution | Should be used in conjunction with other tools |

Formulas, made explicit:

```
HA_Close = (Open + High + Low + Close) / 4          # of the current real candle
HA_Open  = (HA_Open_prev + HA_Close_prev) / 2       # of the previous HA candle
HA_High  = max(High, HA_Open, HA_Close)
HA_Low   = min(Low,  HA_Open, HA_Close)
```

The slide's "High: highest price during the period" is a simplification; the standard HA high and low also include the HA open and close.

### 1.2 Reading the candles

From the annotated chart (a daily WMT chart, 2013 to 2014, credited to tradingsetupsreview.com). Four readings:

| # | Candle shape | Meaning |
|---|--------------|---------|
| 1 | Green candles with **no bottom shadows** | Trending up, strong |
| 2 | Red candles with **no top shadows** | Trending down, strong |
| 3 | **Dojis** with both top and bottom shadows, after a run | Turning point |
| 4 | **Dojis** with both shadows, in a cluster | Congestion (range) |

The rule that falls out: a shadow on the *trend side* of a Heikin-Ashi candle is the first sign of weakening. A green candle growing a lower wick means buyers are no longer in full control; a doji means the trend is undecided.

### 1.3 How it fits the method

- Heikin-Ashi is a **direction** tool. Green run with flat bottoms confirms the long bias from Module 2; red run with flat tops confirms the short bias.
- Readings 3 and 4 are the **Skip** conditions at candle level: dojis mean no trade, whether they signal a turn or a range.
- **Heikin-Ashi prices are not real prices.** The HA close is an average, and the HA open is derived from the previous HA candle. Every level from Module 1's Discharge rules (nearest resistance, EMA 50, the stop) must be placed on the **real** chart, not read off HA candles. An HA "close above resistance" can occur while the real close is below it.
- **It lags by construction.** The HA open is half a candle behind. On a 1-minute scalping chart that lag is small in time but large relative to the target. This is why the slide's own caution says to combine it with other tools, and why the course's "enter at the right moment, not the first moment" is compatible with it.

## 2. 3 Main Indicators (三大主要指标)

_Not yet captured._

## 3. Add-on SMC indicator

_Not yet captured._

## 4. Advance tool: New Indicators

_Not yet captured._

## 5. Trend line, Support & Resistance, Tunnel trend line

_Not yet captured._

## 6. Seahorse pattern

_Not yet captured._

## Open questions

- Which of the six timeframes from the screener is the Heikin-Ashi read on for entries?
- Is the EMA in Module 1 computed on Heikin-Ashi candles or real candles? The two give different crosses.
- Are the "3 Main Indicators" the EMA, OI and funding rate from the screener, or a separate set?
