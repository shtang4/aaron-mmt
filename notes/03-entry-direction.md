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

The three, in the order taught, with the course's Bybit settings:

| # | Indicator | Bybit path | MMT setting | Role |
|---|-----------|-----------|-------------|------|
| 1 | **EMA** | Indicators → Main Indicator → Moving Average Exponential | 9, 25, 55, 155, 255 | Direction (EMA 155) and pullback levels (the faster lines) |
| 2 | **MACD** | Indicators → Secondary Indicator → MACD | Fast 8, Slow 13, Signal 9 | Momentum confirmation on the pullback |
| 3 | **Volume** | Indicators → Secondary Indicator → Volume | VOLMA 5 and 10 (default) | Confirmation, and spike-based exhaustion at turns |

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

Exact settings from the "MMT 5 Lines EMA setting" screenshot (Bybit → Chart Settings → Indicators → Main Indicator → **Moving Average Exponential**). Tick exactly these five rows and set the periods; leave the rest unticked:

| Ticked | Period | Colour on chart | Role |
|--------|--------|----------------|------|
| ✓ | **9** | Purple | Fastest line |
| ✓ | **25** | Blue | |
| ✓ | **55** | Pink / magenta | |
| ✓ | **155** | **Green** | **Pivot of the trend** |
| ✓ | **255** | Indigo | Slowest line |

Unticked rows in the screenshot (Bybit defaults, not used): 7, 14, 28, 0, a second 25, a second 55. Press **Confirm**.

The five values agree with the earlier chart header (EMA9, EMA25, EMA155, EMA55, EMA255), so the set is now confirmed from two independent slides.

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


**Second example: ZETAUSDT, 1-minute chart.** Same chart shown twice, both with "Entry 0.8570" drawn as a horizontal line and a highlighted box at about 17:30 to 18:00, after a spike to 0.9828 and a pullback.

- 2 EMA (Basic): labelled **"No clue"**. With two lines there is nothing at 0.8570 to justify an entry.
- 5 EMA (Advance): labelled **"SPE Entry"** and "LONG". The pullback lands on one of the faster EMAs of the 5-line set, price holds it, and that touch is the entry. Price then grinds higher to about 0.90.

This is the clearest statement yet of what Sniper Price Entry (Module 4) is: **a pullback to an EMA of the 5-line set, in the direction EMA 155 confirms**. The 2-EMA chart cannot produce it because the intermediate lines do not exist.

Both ZETA screenshots also show MACD in the lower pane, which is why MACD is the next indicator taught.

### 2.4 Which pair is the "basic" 2 EMA, and what is "EMA 50"?

No slide names the basic pair. On the ZETA 2-EMA chart the lines are yellow and magenta, which match the colours of Bybit's default, unticked EMA rows (7 is yellow, 28 is pink) rather than any of the five MMT lines. So the "basic" chart may simply be Bybit's out-of-the-box EMA overlay, not a deliberate pair. That is an inference from colours only. The Module 1 stop-loss rule says "below EMA 50", and there is no EMA 50 in the 5-line set. The closest is **EMA 55**. Most consistent reading: the basic pair is two of the five, the stop rule's "EMA 50" is EMA 55, and the "long-term EMA" in the exit signal is probably EMA 55 or EMA 155. This needs confirming from the session, and it matters, because the exit and stop rules hang on it.

### 2.5 The airport analogy

"Trading is like an airport flight. Wrong timing will miss flight."

| Ride dangerously like James Bond | Ride calmly like Business Class |
|----------------------------------|--------------------------------|
| Last call, boarding close. Run after the plane. | Arrive before boarding. Wait at the premium lounge. On time, board to destination. |

Applied: do not chase a candle that has already left an EMA. Wait for price to come back to the line (the lounge) and board there. This is the behavioural rule behind the 5-EMA pullback entries.


### 2.6 MACD concept

Slide text, condensed. MACD (Moving Average Convergence Divergence) has two lines, the MACD line and the signal line, plus a histogram. Three standard readings:

| # | Reading | Bullish | Bearish |
|---|---------|---------|---------|
| 1 | **Signal line crossover** | MACD line crosses above signal line | MACD line crosses below signal line |
| 2 | **Zero line crossover** | MACD line crosses above zero: momentum turns positive | MACD line crosses below zero: momentum turns negative |
| 3 | **Divergence** | Price makes lower lows while MACD makes higher lows | Price makes higher highs while MACD makes lower highs |

Closing caution on the slide: MACD "should not be used in isolation".

**MMT MACD setting** (from the "MACD setting" screenshot): Fast Length **8**, Slow Length **13**, Signal Length **9**. This is not the default 12 / 26 / 9. The shorter fast and slow lengths make the MACD line react faster and cross more often, which suits a 1-minute chart and matches the 5-EMA philosophy of more, earlier signals. The cost is the same: more crosses means more false ones.

**Example chart** (a daily chart of PDD, Pinduoduo, August 2019 to May 2020, from ProRealTime, shown twice): every MACD cross is marked as a buy or sell signal. On the left panel, five buying signals over nine months, each at a histogram flip from red to green. On the right, the same period with both buying and selling signals marked. Of the buy signals shown, the first four preceded moves that mostly went sideways or down before the fifth caught the real advance. That is the honest picture of MACD crosses on their own, and it is why the course pairs MACD with EMA 155 for direction rather than trading the cross alone.

How it fits: EMA 155 gives direction, the faster EMAs give the pullback level, and MACD is the momentum check on the pullback. A long on an EMA touch is stronger when the histogram is contracting toward zero and turning up, and weaker when MACD has already crossed down hard. Reading 3, divergence, is the one that argues against an entry: a pullback after bearish divergence is more likely a reversal than a continuation. The slides do not say any of this; it is how the two tools are normally combined.


### 2.7 Volume concept

Slide table, transcribed:

| Volume indicator | Explanation |
|------------------|-------------|
| Confirmation of price movements | Increased trading volume confirms the price trend. Higher volume during an uptrend indicates increased buying interest; higher volume during a downtrend suggests increased selling pressure. |
| Volume breakouts | Volume surpassing a threshold or exceeding average volume can indicate the initiation or continuation of significant price moves. |
| Volume divergence | Price makes new highs or lows but volume fails to follow. Indicates weakening of the prevailing trend and potential reversal. |
| Volume patterns | Volume spikes or clusters can help identify potential turning points or areas of support and resistance. |

Closing text: volume assesses activity and liquidity; interpretation varies by market and strategy; use with other indicators.

**Example charts** (three, all reused from public sources):

- S&P 500 E-mini daily (TradingView): three volume spikes highlighted, each at a sharp low (October 2014, December 2014, August 2015) followed by a reversal up.
- eBay daily (commodity.com): two spikes labelled **"2X Avg Volume"**, one at a low labelled **buying exhaustion** (the sellers finished, then price rose) and one at a high also labelled buying exhaustion (the buyers finished, then price fell).
- A 1-hour crypto-style chart with one volume bar roughly three times its neighbours at the start of a strong up move.

The rule these examples encode: **a volume bar around twice the recent average marks exhaustion of the side that was in control, and price turns.** The same spike means "bottom" after a fall and "top" after a rise. It is a turning-point signal, not a continuation signal, despite the table's first row.

How it fits: volume is the third check on an SPE pullback entry. A pullback on **falling** volume into an EMA is healthy (sellers are thin), and a long there is confirmed. A pullback on a **2× spike** is exhaustion, meaning either the trend is over or the spike marks the low of the pullback; either way, wait for the next candle rather than buying into the spike. **MMT Volume setting** (from the "Volume setting" screenshot): Indicators → Secondary Indicator → Volume → tick **VOLMA 5** (yellow) and **VOLMA 10** (blue), leave the other nine rows unticked at 0, Confirm. This is the Bybit default, so the two volume moving averages on the ZETA screenshots are the course setup.

Note that the S&P and eBay examples are daily charts of stocks and index futures, not 1-minute crypto. The exhaustion pattern is general, but "2× average" on a 1-minute chart is hit constantly by single large orders. A stricter multiple, or the Bybit MA10 line as the baseline, will be needed to make it usable at that timeframe.

### 2.8 What the course claims Diagnose gives you

Two framing slides. The pain points quoted: "I never know exactly when to enter a trade." "I always feel like I'm too early or too late." "I have followed the same signals before and lost." Answer: "The EMA tells you. Every time. Diagnose removes the guesswork entirely."

What you will have when implementing Diagnose: why the call was made, when to enter, when to exit, when to skip, how to find better entry timing.

"Every time" and "entirely" are marketing. The course's own examples show the EMA cross firing after half a move, and the 5-EMA pullback entries clustering in the last leg. What the EMA set does give you is a **written reason** for every entry, which is the Module 1 checklist requirement. That is the defensible claim.

## 3. Add-on SMC indicator (添加SMC指标)

### 3.1 Concept

Slide text (given in English and Chinese): in futures trading, the Smart Money Concept means tracking the actions of large, well-informed institutional investors who drive significant market movements. It assumes these players have better information and analysis, so their trades are more predictive. Traders using it look for institutional buying and selling patterns, such as price accumulations, manipulations and liquidity grabs, to align with the smart money's direction.

### 3.2 Glossary, as given on the slide

| Term | Slide definition |
|------|-----------------|
| Supply zone | Area where selling pressure exceeds buying pressure, often leading to a price decrease. |
| Demand zone | Area where buying pressure exceeds selling pressure, often leading to a price increase. |
| Fair Value Gap (FVG) or imbalance | "Represents the initial significant move in a new trend, indicating a potential entry point for Smart Money traders." |
| Weak high | A peak with limited buying interest, often signalling potential resistance. |
| Weak low | A trough with limited selling interest, often signalling potential support. |
| Strong high | A peak with significant buying interest, suggesting strong upward trend continuation. |
| Strong low | A trough with significant selling interest, suggesting strong downward trend continuation. |
| CHoCH (Change of Character) | A shift in market sentiment or trend direction, often indicating a potential reversal. |
| BOS ("Breakout or Breakdown") | Price breaches a significant support or resistance level, potentially indicating a shift in trend direction. |
| Equal high / equal low | Multiple price peaks (troughs) at the same level, indicating potential resistance (support). Cut off at the bottom of the slide. |

The table contains literal `<br>` tags, so it was pasted from a web or AI-generated source without editing.

### 3.3 Where the slide's definitions differ from standard SMC usage

Several of these are loose or inverted relative to how SMC is normally taught. If you use an SMC indicator on TradingView or Bybit, it will label things by the standard definitions, not the slide's, so the differences matter:

| Term | Standard SMC meaning | Difference from slide |
|------|---------------------|----------------------|
| **FVG** | A three-candle imbalance: the gap between candle 1's high and candle 3's low (bullish) that candle 2 skipped over. Price tends to return to fill it, and that return is the entry. | The slide describes it as "the initial move in a new trend", which is the displacement that *creates* the FVG, not the gap itself. The entry is on the retrace into the gap, not on the move. |
| **BOS** | **Break of Structure**: price takes out the previous swing high in an uptrend (or swing low in a downtrend). It confirms trend *continuation*. | The slide expands it as "Breakout or Breakdown" and says it indicates a *shift* in trend. In standard usage a shift is CHoCH; BOS is continuation. |
| **Strong high / strong low** | A strong low is the low that produced a BOS to the upside, so it is protected and unlikely to be revisited. A strong high is the mirror. | The slide's "significant buying interest at a peak suggests upward continuation" is muddled: a peak with heavy buying that fails is a weak high, not a strong one. |
| **Weak high / weak low** | A high that did not produce a BOS, so it is likely to be taken out (liquidity sits above it). | The slide treats a weak high as resistance. In standard usage it is a target, not a barrier. |
| Supply / demand zone, CHoCH, equal highs and lows | Match the slide closely enough. | |

Net: the slide gets supply and demand, CHoCH and equal highs right, and gets FVG, BOS, and strong versus weak highs wrong or backwards. Use the standard definitions.

### 3.4 How SMC fits the MMT stack

- **Demand zones and FVGs are pullback targets**, the same role the faster EMAs play in the 5-line set. A pullback that lands on an EMA *and* a demand zone or FVG is a stronger SPE entry than either alone.
- **Equal highs and lows are where the stop must not be.** Liquidity rests just beyond them and gets swept. A stop placed just below an equal low is the stop most likely to be run before the move. The Module 1 rule of a structural stop below EMA 55 (or 155) generally sits further away than an equal low, which is the safer side of this.
- **CHoCH on the 1-minute chart is the early exit warning**, ahead of the EMA cross-back. It fires when price breaks the last higher low in an uptrend, which usually happens before EMA 9 crosses EMA 25.
- No SMC indicator settings are given, and the Bybit app does not have a native SMC indicator in the list shown. This add-on is presumably a TradingView indicator; confirm which one.


## 4. Advance tool: New Indicators

_Not yet captured._

## 5. Trend line, Support & Resistance, Tunnel trend line

_Not yet captured._

## 6. Seahorse pattern

_Not yet captured._

## Open questions

- ~~Which timeframe is the Heikin-Ashi read on for entries?~~ Answered: the Bybit setup screenshots use the 1-minute chart.
- Is the EMA in Module 1 computed on Heikin-Ashi candles or real candles? The two give different crosses.
- ~~Which are the 3 Main Indicators and the MACD setting?~~ Answered: EMA (9/25/55/155/255), MACD (8/13/9), Volume (default).
- What volume multiple counts as a spike on the 1-minute chart, and is the baseline VOLMA 5 or VOLMA 10?
- Which SMC indicator does the course use, and on which platform, given Bybit has none in its list?
- In the ZETA example, which of the five EMAs did price pull back to for the SPE entry?
- Which two of the five EMAs (9, 25, 55, 155, 255) are the "basic" pair, and does the Module 1 stop rule's "EMA 50" mean EMA 55?
- What counts as a "full body" candle for the three-candle EMA 155 rule, and is it read on Heikin-Ashi or regular candles?
