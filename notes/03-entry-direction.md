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

The Bybit Indicator Settings screen (shown on the "Steps to setting" slide) groups indicators as **Main Indicator: Moving Average, Moving Average Exponential, Bollinger Bands** and **Secondary Indicator: Volume, MACD, KDJ, Relative Strength Index, WR**. The course's "3 Main Indicators" most plausibly refers to Bybit's three Main Indicator entries, with EMA as the one actually taught. Treat that as a likely reading until a slide names the three.

### 2.1 EMA concept

Definition table, transcribed:

| Term | Definition |
|------|------------|
| EMA (Exponential Moving Average) | A popular technical indicator used in financial markets to analyse price trends and identify potential entry or exit points for trades. |
| Calculation | Assigns more weight to recent price data, making it more responsive to short-term price changes. |
| Weighting | The most recent price data points are given more weight, while older data points receive less weight. |
| Formula | EMA = (Close − EMA(previous)) × Smoothing factor + EMA(previous) |
| Smoothing factor | A smoothing constant that determines the weight given to the current closing price. |
| Purpose | Identifies the direction of a price trend and potential points of support or resistance. |
| Crossovers | Crossovers between different EMA periods are often used as signals for potential buying (bullish) or selling (bearish) opportunities. |
| Timeframes | EMA can be applied to various timeframes, such as daily, weekly, or hourly charts. |
| Application | Used in technical analysis to assist in making informed trading decisions. |

The smoothing factor is not given on the slide. Standard value: 2 / (N + 1) for an N-period EMA.

### 2.2 The MMT 5-line EMA set

From the Bybit chart header on the setup slide, the five EMAs and their values at the moment of the screenshot:

| EMA | Colour on chart | Role |
|-----|----------------|------|
| EMA 9 | Purple / blue (fastest) | Fast line |
| EMA 25 | Yellow | |
| EMA 55 | Pink / magenta | |
| **EMA 155** | **Green** | **Pivot of the trend** |
| EMA 255 | Indigo (slowest) | Slow line |

Bybit setup: Chart Settings → **Indicators** → Main Indicator → **Moving Average Exponential**, then set the five periods.

Slide rules for the 5-line set, verbatim:

- Each individual line can be the support line or resistance line for entry-point consideration.
- Each line is a guidance line of SPE (Sniper Price Entry, Module 4).
- **Green line EMA 155 always acts as the pivotal point of the trend.**
  - If 3 consecutive full-body candles form **above** this line → considered uptrend, can **LONG**.
  - If 3 consecutive full-body candles form **below** this line → considered downtrend, can **SHORT**.

This is the first fully mechanical direction rule in the course. It replaces the vague "golden cross, look for a long" with a countable condition: three closed, full-bodied candles on one side of EMA 155. "Full body" is not defined; the sensible reading is a candle whose body is clear of the line, not one that wicks through it.

### 2.3 "Real example: Sniper Entry", 2 EMA versus 5 EMA

Side by side on the same 1-minute chart (a coin rising from about 0.0562 to 0.0680 between 08:22 and 09:19, then pulling back):

| | 2 EMA (Basic) | 5 EMA (Advance) |
|-|---------------|-----------------|
| Lines | Yellow (faster) and blue (slower) | All five |
| Entries marked | Two: the golden cross near 08:30 and a touch of the slower EMA near 09:12 | Six or more: every pullback that tags one of the faster EMAs on the way up |
| Slide caption | "Less entry" | "More entry opportunity" |

What this means in practice: with two lines, the only entries are the cross and the occasional pullback to the slow line. With five lines, each faster EMA becomes a pullback level, so a strong trend offers an entry on every dip to EMA 9, 25 or 55. That is the "advance method to find more entry": **buy the pullback to an EMA in the direction EMA 155 says**, rather than waiting for the next cross.

The example also shows the downside. After the spike to 0.0680 at 09:00, price fell through EMA 9, 25 and 55 in a few minutes. A pullback entry at any of those lines during the fall would have been stopped. The 5-EMA method produces more entries, and more of them are in the last leg of a move. The Discharge rules from Module 1 (take profit set first at the nearest resistance) are what make the extra entries survivable.

### 2.4 Which pair is the "basic" 2 EMA, and what is "EMA 50"?

Neither slide names the basic pair. The colours do not settle it either: on the 2-EMA chart the blue line is the slower one, while on the 5-EMA chart the blue-purple line is EMA 9, the fastest. The Module 1 stop-loss rule says "below EMA 50", and there is no EMA 50 in the 5-line set. The closest is **EMA 55**. Most consistent reading: the basic pair is two of the five, the stop rule's "EMA 50" is EMA 55, and the "long-term EMA" in the exit signal is probably EMA 55 or EMA 155. This needs confirming from the session, and it matters, because the exit and stop rules hang on it.

### 2.5 The airport analogy

"Trading is like an airport flight. Wrong timing will miss flight."

| Ride dangerously like James Bond | Ride calmly like Business Class |
|----------------------------------|--------------------------------|
| Last call, boarding close. Run after the plane. | Arrive before boarding. Wait at the premium lounge. On time, board to destination. |

Applied: do not chase a candle that has already left an EMA. Wait for price to come back to the line (the lounge) and board there. This is the behavioural rule behind the 5-EMA pullback entries.

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
- Are the "3 Main Indicators" Bybit's Main Indicator group (MA, EMA, Bollinger Bands), or a course-specific set? Only EMA has been taught so far.
- Which two of the five EMAs (9, 25, 55, 155, 255) are the "basic" pair, and does the Module 1 stop rule's "EMA 50" mean EMA 55?
- What counts as a "full body" candle for the three-candle EMA 155 rule, and is it read on Heikin-Ashi or regular candles?
