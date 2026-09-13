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

### 1.4 Six Heikin-Ashi patterns ("Become the King of Trends")

Six-panel reference chart (credited with an "FJ" logo, not the course's own). Each panel is one pattern:

| Panel | Pattern | What to look for | Use |
|-------|---------|------------------|-----|
| 1 | **Shift from green to red** | First red HA candle after a green run, often with a small body | Uptrend ending; exit longs, short bias begins |
| 2 | **Strong uptrend** | Consecutive green candles with **no lower shadows** | Long is valid; stay in |
| 3 | **Trend continuation** | A cluster of small-bodied candles inside a trend, then the trend resumes | Pause, not reversal; hold or re-enter with trend |
| 4 | **Shift from red to green** | First green HA candle after a red run | Downtrend ending; exit shorts, long bias begins |
| 5 | **Strong downtrend** | Consecutive red candles with **no upper shadows** | Short is valid; stay in |
| 6 | **Trend reversal** | Small-bodied candles, dojis or spinning tops at the end of a run, then colour change | Take profit, then look the other way |

Panels 3 and 6 look the same at the moment they form: a cluster of small bodies. The difference is only known afterwards, by whether the next full-bodied candle is the same colour (continuation) or the opposite colour (reversal). So a small-body cluster on its own means **wait**, which is the Skip decision at candle level. The confirming candle is the entry, which is what "enter at the right moment, not the first moment" means here.

### 1.5 Bybit setup for Heikin-Ashi

From the "Steps to setting" screenshots (TRBUSDT, USDT-Perp, 1-minute chart):

1. Derivatives → USDT-Perp → pick the coin → **Charts** tab.
2. Select timeframe. The screenshot has **1m** selected, with 15m, 1h, 4h, 1D also available on the bar.
3. Open **Chart Settings** (pencil icon) → **Others**.
4. **Candlestick** → change from Candle to **Heiken**.
5. Other settings shown: Scale = Middle, Style = Bar, Mark Price = Close, Automatic Fullscreen off.

Also visible on the chart screen and worth noting:

- The indicator bar offers MA, EMA, BOLL, MAVOL, MACD, KDJ, RSI. The "3 Main Indicators" in section 2 will almost certainly come from this list.
- Below the chart: Order Book, Trades, **OI Data**, **Contract** tabs. These are where the screener's checks 2 and 3 (open interest, funding rate) are read, and the Order Book is check 4 (depth).
- The **1m** selection confirms the entry timeframe. Direction comes from the higher timeframes (Module 2 screener); the Heikin-Ashi entry chart is 1 minute.

### 1.6 "Find Direction: which one easier?" The Diagnose comparison

Side-by-side of the same 1-minute chart (roughly 2:45 PM to 5:00 PM):

- **Without Diagnose** ("Normal, no guide"): plain candles. Labelled "confusing direction".
- **With Diagnose** ("Direction guide"): the same chart with two EMAs overlaid (blue short-term, red long-term). A green circle marks the golden cross near 3:00 PM and a green arrow the rise that followed. A red circle marks the death cross around 4:15 PM and a red arrow the fall that followed.

What the slide shows, beyond what it says:

- The Diagnose chart uses **regular candles, not Heikin-Ashi**. The EMA cross is the direction guide; Heikin-Ashi is a separate lens. They are not stacked on one chart in the course's own example.
- **The death cross fires late.** The top was near 4:00 PM at about 0.01826. The cross prints around 4:15 PM near 0.01817, after roughly half the eventual move down had already happened. The golden cross is better timed but still after the low. This is the lag cost of the EMA method, visible in the course's own example. The exit-signal rule from Module 1 ("short EMA crosses back below long EMA, exit, no questions") would have given back a meaningful part of the long's gain here.
- The EMA periods are still not stated. Two lines, blue and red, is all the slide gives.

### 1.7 The driving analogy

"Trading is like driving. Copy blindly will lead to car crash."

| Without Diagnose | With Diagnose |
|------------------|---------------|
| Follow GPS blindly. Autopilot without knowing how to drive. Ends in a crash. | Learn to drive properly. GPS is a useful guide. Reach the destination safer. |

The point is aimed at students who copy signals (the "GPS") without being able to read the chart. Indicators are the guide, not the driver. This repeats the Module 1 line "the signal is the symptom".

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

- ~~Which timeframe is the Heikin-Ashi read on for entries?~~ Answered: the Bybit setup screenshots use the 1-minute chart.
- Is the EMA in Module 1 computed on Heikin-Ashi candles or real candles? The two give different crosses.
- Are the "3 Main Indicators" the EMA, OI and funding rate from the screener, or three from the Bybit indicator bar (MA, EMA, BOLL, MAVOL, MACD, KDJ, RSI)?
- What are the two EMA periods? Still unstated after four slides showing the pair.
