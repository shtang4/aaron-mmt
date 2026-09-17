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

**How to tell reading 3 from reading 4, spoken in the session** (notes/08 part 6): look at the candles that come *after* the cluster. Same colour as before it means **congestion** and the trend continues; a colour change means a **pivotal turn**. And the timing: "Cannot say one candle is true. You have to take another one or two candle. Wait for the second, third candle, then only you execute." **A doji or a single small body is never actionable; wait two to three candles for the colour to resolve.**

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
- **The death cross fires late, and he says so.** "This is not the perfect indicator. There are some lagging ... the EMA needs to do calculation to average it out" (notes/08 part 6). On this chart the top was near 4:00 PM at about 0.01826 and the cross prints around 4:15 PM near 0.01817, after roughly half the eventual move down had already happened. The golden cross is better timed but still after the low. This is the lag cost of the EMA method, visible in the course's own example. The exit-signal rule from Module 1 ("short EMA crosses back below long EMA, exit, no questions") would have given back a meaningful part of the long's gain here.
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
| ✓ | **255** | Indigo | Slowest line. **"Considered support. That is the last guard."** |

Unticked rows in the screenshot (Bybit defaults, not used): 7, 14, 28, 0, a second 25, a second 55. Press **Confirm**.

The five values agree with the earlier chart header (EMA9, EMA25, EMA155, EMA55, EMA255), so the set is now confirmed from two independent slides.

Slide rules for the 5-line set, verbatim:

**Four rules from the session that the slides never state** (notes/08 parts 6 and 9):

- **Fan width is trend strength.** "The wider the gap open, the better it is trend and more confirm the trend." A cross with the lines still bunched is a weak signal; a spread fan is a confirmed trend.
- **Repeated crossing means ranging.** "If it keeps repeatedly changing up and down, crossing each other, that means it's ranging." Treat a chart where the lines keep swapping as a skip, not as a run of signals.
- **Wait for the separation to hold before entering.** "Enter after opening wider and no more changing would be more promising."
- **The retracement test** (A8, [06 §6.4](06-case-studies.md)): "If let's say one line down, two line down, three line down, but not against going below EMA 155, **it is only a retracement only.** Retrace and then pump back." Price losing one, two or even three of the faster lines is a dip; the trend has changed only when three full-body candles print on the far side of EMA 155 — the same test that set the direction. This is the rule that makes the five-line set's extra entries usable: a touch of EMA 9, 25 or 55 is an entry while the pivot holds, and stops being one the moment it does not.
- **The same test in its precise form, from the SMC session — it is about the EMAs' *order*, not price:**

  > "Whatever the price remains 5 EMA lines, **3 shorter term EMA can always crossing each other**. **As long as the first three EMA lines are still above the EMA 155 line, you can consider as a retracement only.** Let's say this three lines cross below the green line, and the green line turn to be the fourth line, and subsequently the EMA 255 the last line — **all turn upside down, the 5 EMA lines all upside down, like this totally is a change of trend. You either cut loss or you exit.**"

  | Fan state | Read |
  |---|---|
  | 9, 25, 55 tangled with each other, all still **above** 155 | **Retracement.** Hold. The fast lines crossing is normal noise |
  | 9, 25, 55 cross **below** 155, so the order becomes 255 > 155 > 55 > 25 > 9 — **fully inverted** | **Change of trend.** Cut loss or exit |

  This is stricter and later than the candle test above, and both are in the deck. Read them as a sequence: **three full bodies past EMA 155 is the warning that direction has gone; full fan inversion is the confirmation and the last exit.**

Slide rules for the 5-line set:

- Each individual line can be the support line or resistance line for entry-point consideration.
- Each line is a guidance line of SPE (Sniper Price Entry, Module 4).
- **Green line EMA 155 always acts as the pivotal point of the trend.** Spoken, on the ZETA walkthrough: **"EMA 155 is the most powerful EMA I would say in this world."** His claim, recorded as his. EMA 255 below it is "the last guard": the final support before the structure is gone.
  - If 3 consecutive full-body candles form **above** this line → considered uptrend, can **LONG**.
  - If 3 consecutive full-body candles form **below** this line → considered downtrend, can **SHORT**.

**A contradiction to settle before you trade it.** The Module 1 exit rule, which is in the SOP as the runner's backstop, is "EMA 9 crossing back through EMA 25 → exit, no questions". The SMC session says the opposite in plain words: "3 shorter term EMA can always crossing each other" and that is still only a retracement. Both cannot govern the same position. The reading these notes use:

| Position | Rule |
|---|---|
| The **runner** (25% left after the climax partial, stop already at entry) | EMA 9 × EMA 25 cross-back closes it. You are protecting a gain, not managing a trade |
| The **main position**, fan still ordered above EMA 155 | Fast-line crossing is noise. The exits are the climax rule, then the pivot, then fan inversion |

If you take the Module 1 rule literally on a full position you will be stopped out of every ordinary pullback, which is exactly what the five-line set exists to let you buy.

**"EMA 155" is a role, not a number.** On the A8 case-study chart ([06 §6.3](06-case-studies.md)) he states this same rule aloud over a fan of **EMA 20 / 89 / 144 / 233 / 377** — a chart with no EMA 155 on it. The line he points at is EMA 144. So the pivot is *the middle-to-slow line of the five-line fan*, and 155 is this course's choice of length for it. That makes five EMA configurations in the material (10/25/50 on the 2023 charts, 9/25/55/155/255 taught, a single EMA 20 in the handouts, 20/89/144/233/377 on A8). Run the taught set and read every rule on it; when you meet someone else's fan, map the rule to the equivalent line.

This is the first fully mechanical direction rule in the course. It replaces the vague "golden cross, look for a long" with a countable condition: three closed, full-bodied candles on one side of EMA 155. **Confirmed from the session: the rule is read on the Heikin-Ashi chart** with the Bybit setup switched on. So "full body" is the Heikin-Ashi strong-trend candle from section 1.2: the body sits on the trade side of EMA 155 and there is no wick on the opposite side (no lower wick on a green candle for a long, no upper wick on a red candle for a short). Three of those in a row, closed, and direction is set. Two consequences: Heikin-Ashi smooths, so the rule confirms a little earlier and a little more often than it would on real candles; and every price that goes into an order (entry, stop, TP) is still read from real candles, because Heikin-Ashi prices are averages.

### 2.3 "Real example: Sniper Entry", 2 EMA versus 5 EMA

Side by side on the same 1-minute chart (a coin rising from about 0.0562 to 0.0680 between 08:22 and 09:19, then pulling back):

| | 2 EMA (Basic) | 5 EMA (Advance) |
|-|---------------|-----------------|
| Lines | Yellow (faster) and blue (slower) | All five |
| Entries marked | Two: the golden cross near 08:30 and a touch of the slower EMA near 09:12 | Six or more: every pullback that tags one of the faster EMAs on the way up |
| Slide caption | "Less entry" | "More entry opportunity" |

What this means in practice: with two lines, the only entries are the cross and the occasional pullback to the slow line. With five lines, each faster EMA becomes a pullback level, so a strong trend offers an entry on every dip to EMA 9, 25 or 55. **He counts it in the session** (notes/08 part 8): two EMAs give "1, 2 and 3 only", five give "1 2 3 4 5 6 7 8, **you get 8 attempts of opportunity to enter if you miss it**". The justification for the five-line set is therefore *more chances at the same trade*, not a better signal. That is the "advance method to find more entry": **buy the pullback to an EMA in the direction EMA 155 says**, rather than waiting for the next cross.

The example also shows the downside. After the spike to 0.0680 at 09:00, price fell through EMA 9, 25 and 55 in a few minutes. A pullback entry at any of those lines during the fall would have been stopped. The 5-EMA method produces more entries, and more of them are in the last leg of a move. The Discharge rules from Module 1 (take profit set first at the nearest resistance) are what make the extra entries survivable.


**Second example: ZETAUSDT, the same trade at three timeframes.** Entry 0.8570 and exit 2.8530 drawn as blue lines on all of them. Full trade write-up: [06 §7.2](06-case-studies.md) and [05 §2.3](05-risk-and-hedging.md).

| Chart | What it shows | His verdict |
|-------|--------------|-------------|
| **1 Month** | Three candles. Low 0.6742, high 2.8813. The entry line sits at the base of the first one | The trade, seen whole |
| **1 Day**, 2 EMA vs 5 EMA | The whole move, 01/30 to 03/15 | "Seriously by using 1 day, **you can't really see clearly with the EMA, even by using 2 EMA**. 5 EMA relatively you can peer through." |
| **1 minute**, 2 EMA vs 5 EMA | The entry itself: a spike to 0.9828, a pullback into a box at 0.8570, then the grind up | 2 EMA: **"No clue."** 5 EMA: **"SPE Entry"**, "LONG". "By using smaller 1 minute, 5 EMA you can actually precisely enter it." |

Two things follow from that table, and the second one is not flattering.

**The daily chart does not produce the entry, on either EMA set.** He says so directly. Direction comes from the higher frames; the price comes from the 1-minute chart. That is the strongest statement in the course that **the 1-minute chart is the execution chart**, and it is made while admitting the method's own indicator is unreadable on the timeframe most people would check first: "So there's some other tools that you need to use, try all of them."

**ZETA was a day-one or day-two listing.** "That time when she traded, that time this coin just started day 1 or day 2 only. Day 1 or day 2, she managed to enter at this pricing, 0.8570." The monthly chart confirms it: three candles of history in total. So the "most powerful EMA in this world" was, on that 1-minute chart, an average of about **155 minutes — two and a half hours — of a brand-new listing's price**. EMA 255 was four and a quarter hours old. The lines were computable but they were not describing a trend; they were describing a launch. This is also Golden Rule 4 ("new-born coins: trade for a few days only") being broken by the same trade that breaks Golden Rule 6, since it was then held about two and a half weeks ([05 §5](05-risk-and-hedging.md)).

**The entry count, restated and now larger.** On this chart he counts the parkable levels out loud: "How many attempts you can enter, if you miss one, by using the 5 EMA comparatively to the 2 EMA? If you want to base on this EMA 155, you got 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11 opportunity for you to enter before it pumps." Eleven here, eight on the slide in part 8 of the transcript. **The number is a property of the chart, not of the method** — it counts how many times price touched a line on a move that happened to keep going. On a move that turned, the same touches are the same number of chances to be stopped.

**Parking, and following the line.** "Whatever 3 full body candles above the EMA 155, obviously you can enter as long ... If you miss this, you can up here. If you miss this here, you park here. **Just follow along the line.**" So the resting limit order is trailed up the EMA as the trend advances, and **any** of the five lines is a legitimate place to park, not only EMA 9: on this chart he points at EMA 155 itself. Reconciling with the confirmed answer that EMA 9 is the first target — EMA 9 is the shallowest and the most frequently filled, EMA 155 is the deepest with the pivot rule behind it, and EMA 255 is the last guard. Which one you use sets how often you are filled and how far the stop has to sit.

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


### 2.6a MACD as he actually teaches it: two shapes only

The slide gives the textbook three readings. The spoken version throws almost all of it away:

> "**MACD is just about histogram only.** Histogram, there's a peak at top here, green colour, and peak at the bottom, red colour. So you just need to recognise these two peaks. Green colour, **mountain**. This red colour is called **iceberg dip**."

> "If you don't understand anything of the MACD, fine, you just remember two things: **mountain peak, the green colour, and iceberg dip, the red colour.** That's it."

So the working MACD in this course is two shapes and a zero line (he calls it the "iso line", equilibrium):

| Shape | Where | What it is |
|-------|-------|-----------|
| **Mountain peak** | Tallest green bar above zero | The **long's exit** |
| **Iceberg dip** | Deepest red bar below zero | The **long's entry** |
| Iso line / equilibrium | Zero | Halfway back. Where an untaken profit goes first |

**The rule, and the cost of not taking it.** Stated three times in the same passage:

> "You can enter from here to long, but you have to determine to exit, to set TP at **mountain peak**. Otherwise it'll come back, go back to your entry. But if you never exit, they go down further, then you're losing money — because you are long."

> "From here to here, you have to TP here. **If you don't TP here, you'll come back here, at least half of your profit gone.** Then if you don't TP, it will go all the way, same level, you go back to your entry price. If not, you still hold it, then dump all the way — you are losing it."

The ladder is worth keeping because it prices the delay: **peak → equilibrium is half the profit → entry is all of it → below entry is a loss.** Same argument as the ZETA closing slide ([06 §7.5](06-case-studies.md)), made on the indicator rather than on the price.

**Both directions.** "If you want to short, you can enter here short" — at the mountain peak — "and then all the way down here, you TP here", at the iceberg dip. The two shapes swap roles: the long's exit is the short's entry.

**The honesty test he attaches to it.** This is the most useful sentence in the passage:

> "You have to determine whether you have the power to hold. **If you don't have the power to hold, then you better enter long here, exit here.**"

Iceberg dip to mountain peak is the small, complete trade. Holding past the peak for a bigger swing is a different trade that needs the temperament to sit through the give-back. He tells you to pick honestly, and to take the peak-to-peak version if you cannot. That is the same point as the Module 5 ZETA sizing argument, arrived at from the trader's side rather than the position's.

**Confirmation is price, not the indicator alone.** "How to know whether it's peak? Look at the histogram. This is the MACD, this histogram will show you the peak. **Obviously, tally it with the candle.**"

**Where this sits against the rest of the method.** The iceberg-dip entry is a **bottom-fishing entry**: you are buying the deepest red bar, which by construction happens while price is falling. The EMA 155 rule would usually forbid that trade, and the seahorse rule warns against it explicitly. Two readings, and the notes keep the second:

1. Taken literally, MACD gives an entry the direction rule vetoes.
2. Taken as a **timing** tool inside a direction the EMA has already set — which is how every other part of the course uses MACD — the iceberg dip is *when* to take the pullback the EMA rule already permits, and the mountain peak is *when* to take the profit. That is the RAVE "IceBerg Tip" entry ([05 §3.9](05-risk-and-hedging.md)) and the Module 4 climax exit ([04 §2](04-sniper-entry-exit.md)), and it is consistent with everything else.

### 2.6b The hollow histogram bar: the course's explanation, and what it actually is

A Q&A slide, and he spends longer on this than on anything else in the indicator section.

**The question** (@Like to kern): what does a hollow bar in the MACD histogram mean?

**The answer given** (Jasper Sia, 22 Apr 2024, endorsed and repeated by Aaron at length):

> "Why the hollow bar of MACD histogram is being caused by the **counter volume** (different buying & selling = contraindication). MACD supposedly downtrend by red bar but is counter pump by strong buying volume from the market. **If the trend of MACD is equal to the volume trend, then the bar of histogram will be the same solid colour.**"

Aaron's door analogy for it: "If you are going out from the house, and the door suddenly one pushing from outside — in the end of day you are not getting out from the house, you're being pushed by the force outside. That's why it forms hollow." He also ties it to price: "It contrasts, so it forms a doji, indetermined — this one forms hollow."

**The mechanism is wrong, and it is worth knowing why.** MACD is computed entirely from price: `MACD = EMA(fast) − EMA(slow)`, signal is an EMA of that, histogram is `MACD − signal`. **Volume is not an input at any stage.** The indicator cannot see volume, so volume cannot be what fills or hollows a bar.

What the hollow actually encodes on Bybit (and on TradingView's default MACD, and most platforms): **the bar is smaller in magnitude than the one before it.** Solid = the histogram is still growing; hollow = it is shrinking back toward zero. It is a rendering of the first derivative, not of volume.

**Why their version still lands on the right trades.** A red histogram bar begins shrinking precisely when buyers start pushing back against a down move, and that push usually does show up as buying volume on the same candle. So the correlation they describe is real and the observation is a good one. Only the causal arrow is reversed: the buying does not *make* the bar hollow, the buying and the hollowing are both effects of momentum turning. And the doji connection is the same thing seen on price — a doji is a candle whose net move is small, so the EMAs barely separate, so the histogram bar barely grows.

**The correction makes the signal more useful, not less.** The Module 4 climax exit fires when "the next bar prints shorter than the tallest bar" ([04 §2.1](04-sniper-entry-exit.md)). On Bybit that bar is drawn **hollow**. So:

> **The first hollow bar after a run of solid bars is the climax-exit trigger, visible at a glance.**

No bar-height comparison needed, no volume cross-check required for the exit itself. That is the practical payoff of getting the mechanism right, and it is a better rule than the one the slide states.

*Confidence: the formula's independence from volume is certain. The "hollow = shrinking magnitude" convention is the standard platform behaviour and is consistent with every hollow bar visible on the course's own screenshots (they coincide with dojis and near-zero histogram), but it is worth confirming once on your own Bybit chart before relying on it for the exit.*

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

Note that the S&P and eBay examples are daily charts of stocks and index futures, not 1-minute crypto. The exhaustion pattern is general, but "2× average" on a 1-minute chart is hit constantly by single large orders. **The session settles it, and it is the second guess: the threshold is the two VOLMA lines, not a multiple.** See 2.7a.

### 2.7a Abnormal volume, defined: the bar crosses the two VOLMA lines

**This closes the open question these notes carried for the whole course, and it replaces the working rule I had invented in its place.** He does define a volume spike. It is not a multiple of the average:

> "Majority below this line are the normal volume. Suddenly, one spike up, about two spike up. So this is the buying exhaustion ... Above, usually the volume what you see, that's one yellow line one. So, **whichever cross above this line, one sudden pump**."

and, closing the section:

> "So volume, as I say, this one is the line. This is volume line. **Whichever volume bar pump across this two lines. These are the abnormal volume.** This one abnormal by the selling power, abnormal buying power, abnormal selling power, abnormal buying power, abnormal buying power."

**The definition: a volume bar that rises above both VOLMA lines is abnormal.** VOLMA 5 (yellow) and VOLMA 10 (blue) are already in the MMT setup; they are the threshold, and no multiple is needed. Bars under the lines are "normal volume" and carry no signal.

This is a better rule than the "2× VOLMA 10" I proposed, for a reason worth stating: the two moving averages **adapt to the coin and the session**. A fixed multiple is too loose on a quiet 1-minute chart and too strict during a pump; a cross of both lines means "louder than this coin has been over the last five and ten bars", which is the question actually being asked. My 2× rule is retired; it survives only as an optional second filter if the journal shows the exit firing too early.

### 2.7b Reading the abnormal bar: colour, then body or wick

Three things he reads off the bar once it qualifies:

**1. Colour is the side.** "Red colour means sell power." Green is buying. So an abnormal bar is not just "activity", it is directional: abnormal red is a selling event, abnormal green a buying one.

**2. A wick on the candle means it was a liquidity sweep, not a move.** This is the most useful distinction in the passage and it appears nowhere on the slides:

> "How you know? Because suddenly like this, usually **it form a wick one. It's not stable full volume. Because it's just want to sweep the liquidity, it's not a full block like this one.**"

> "The manipulator sell here causing the **long wick**, they just want to grab the liquidity. Then, they sell big volume."

| Abnormal volume bar with … | Reading |
|---|---|
| A **long wick** on the price candle | **Liquidity sweep.** Someone reached for the stops resting beyond the level and came back. The move is not real; price usually returns. |
| A **full body**, no significant wick | **Real move.** The volume and the price agree; the level has actually changed hands. |

That is the discriminator the exhaustion rule in 2.7 was missing. An abnormal green bar with a long upper wick at a high is a sweep and a sell; an abnormal green bar with a full body is a breakout and a hold.

**3. The sequence to watch for.** "The left, all ranging, nothing happens. Suddenly one selling volume pump, so subsequently manipulation here." Quiet range → one abnormal bar → wick → the real move follows. The abnormal bar is the tell that the range is about to end, and the wick tells you which way is the fake.

**How this feeds the Wick Tracker.** Directly, and it refines the level rule:

> "If let's say the last higher was around here, like wick tracker. Suddenly, **you can set somewhere higher a bit. So this one is higher than this one. Then, the next pump will trigger your wick tracker.**"

So the Wick Tracker goes **slightly above the previous wick high**, not at it. The logic is the sweep logic: stops rest above a prior high, so a sweep aiming at that liquidity overshoots it. Carried into [04 §3.1](04-sniper-entry-exit.md). Note it is the opposite framing from "set it inside the wick you expect" — both can hold at once (previous high < your level < the next sweep's extreme), but his reference point is the *previous* high and that is the one to measure from.

### 2.7c Volume as a gate, not a signal

> "Volume determines that trend ... That's why you see the top gainers, how many percentage — that's the volume. **If no volume, like a coin pricing from 0.50, after 4 hours also 0.51, that means no volume.** Like BTC, ETH, SOL, there's no volume during the weekend, today, tomorrow. That's why you cannot trade. Unless something happens, hype happens, some news triggers it and suddenly it pumps alone. Then that's a different story."

This is the weekend rule and the "+4% in two hours is too slow" rule, both already in the SOP, now with the reason attached: the percentage move on the gainers list **is** the volume. It also explains why the majors are the wrong instrument for this method on a quiet day.

A group answer on the same slide makes it a gate rather than a scored check. @eric818 asks whether the volume's two lines are the same as EMA 25/55; **Jasper Sia**, 22 Apr 2024:

> "不一样吧，没注意那两条🤔，主要看那个币有没有volume，如果不活跃，即使其他条件美，没volume你也是一直卡着上下徘徊，很费时。"
> *Not the same; I haven't paid attention to those two lines. Mainly look at whether that coin has volume. If it's not active, then even if the other conditions are beautiful, without volume you'll just be stuck drifting up and down — a big waste of time.*

Two things in that answer. First, **no volume vetoes a perfect setup**: 4/4 on a dead coin is a time sink, not a trade. Second, and worth noticing, the person answering says he does not watch the two VOLMA lines — the same lines Aaron's whole abnormal-volume definition depends on. The course's own answerers are not using the same rule. Prefer Aaron's, since it is the one that is actually defined.

**Recovering the volume pane.** @kelvin63 lost the volume chart by pressing something; Jasper's answer, with a screenshot: it is **MAVOL** in the indicator row under the chart (BOLL · MA · SAR · **MAVOL** · MACD · KDJ · RSI), and the row scrolls — "在这里，推去左边看看里面有吗" (*here, swipe to the left and see if it is inside*). Worth knowing before you rebuild the whole chart setup.

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

### 3.2a The spoken glossary, which is plainer and mostly better than the slide

He re-teaches the whole table verbally, in metaphors, and the spoken version is closer to standard SMC than the slide's pasted text.

**The framing.** "Smart money — why they call it smart money? Because all the big institutions, all the market makers, they all depend on this smart money concept. **They swipe your liquidity** because based on this smart money concept." The premise is that the levels where retail stops rest are targets, and SMC is how you see them before they are taken.

The sales claim attached to it is an overclaim and should be discounted: "basically you can achieve cut loss, you can be awake, be liquidated, you even can TP whatever you want." No structural read prevents liquidation; the stop and the leverage do.

| Term | How he says it |
|------|---------------|
| **Supply zone** | The **pink** band on top. "The selling power. Selling pressure is there." |
| **Demand zone** | The **light blue** band at the bottom. "That's the buying power." |
| Both zones | "Those are the **liquidity areas** where they usually use to wick come down, or wick back whatever liquidity there." A zone is where a wick goes to collect, not where price politely turns. |
| **FVG / imbalance** | "When it pumps too high, actually surges past the gap, **then the gap needs to be filled up**. Wherever, anything, they will come back to hunt back whatever volume over there." |
| **Low** | "Imagine it is your support, which is your **floor**." |
| **High** | "Let's say high is your **ceiling**." |
| **Weak** | "**Breakable, fragile.** You can just break through the resistance." |
| **Strong** | "Very strong floor" / "very strong resistance, can't break through." |
| **CHoCH** | "Change of character ... sometimes it can be **retracement** ... **CHoCH usually is play like retracement, is change of character only but not confirmation**." |
| **BOS** | "Break of structure. Break up or break down. Once the structure fully breaks, **it's totally change trend and break the previous entry trend**." |

**The one line to keep:** *"CHoCH you imagine CHoCH equivalent to retracement. BOS means totally change of trend."*

That is the whole of SMC as this course uses it: **CHoCH warns, BOS confirms.** And note that this spoken sequence is the *standard* one, which the slide's glossary is not — see 3.3.

**The equal-high / equal-low sequence, which is the actionable part.** This is the only place in the course where SMC produces an ordered entry trigger rather than a vocabulary:

> "Equal high, equal low. Let's say if equal high, **you have to look at CHoCH and then follow by BOS. If all these is fulfilled, this thing dump to go down very hard.** Equal low — go back, you see back the one I actually circle — let's say strong low, you see equal low, **follow by BOS. This thing will going to pump like crazy.**"

| Sequence | Read | Trade |
|----------|------|-------|
| **Equal highs → CHoCH → BOS** | Liquidity above the equal highs was taken, character changed, structure broke down | **Short.** "Dump to go down very hard" |
| **Equal lows (at a strong low) → CHoCH → BOS** | Liquidity below was taken, character changed, structure broke up | **Long.** "Pump like crazy" |

Three conditions in order, and all three must be present. This is standard liquidity-sweep-then-reversal and it is correctly stated. It also dovetails with 2.7b: the sweep is the abnormal volume bar with the long wick; the CHoCH and BOS are what tell you the sweep was the turn rather than a pause.

### 3.3 Where the slide's definitions differ from standard SMC usage

Several of these are loose or inverted relative to how SMC is normally taught. If you use an SMC indicator on TradingView or Bybit, it will label things by the standard definitions, not the slide's, so the differences matter:

| Term | Standard SMC meaning | Difference from slide |
|------|---------------------|----------------------|
| **FVG** | A three-candle imbalance: the gap between candle 1's high and candle 3's low (bullish) that candle 2 skipped over. Price tends to return to fill it, and that return is the entry. | The slide describes it as "the initial move in a new trend", which is the displacement that *creates* the FVG, not the gap itself. The entry is on the retrace into the gap, not on the move. |
| **BOS** | **Break of Structure**: price takes out the previous swing high in an uptrend (or swing low in a downtrend). Within a trend it confirms *continuation*; after a CHoCH it confirms the *new* trend. | The slide expands it as "Breakout or Breakdown", which is not the name. But **his spoken usage is the standard one** (3.2a): CHoCH warns, then BOS in the new direction confirms. Read the slide as loose wording rather than a different method. |
| **Strong high / strong low** | A strong low is the low that produced a BOS to the upside, so it is protected and unlikely to be revisited. A strong high is the mirror. | The slide's "significant buying interest at a peak suggests upward continuation" is muddled: a peak with heavy buying that fails is a weak high, not a strong one. |
| **Weak high / weak low** | A high that did not produce a BOS, so it is likely to be taken out (liquidity sits above it). | The slide treats a weak high as resistance. In standard usage it is a target, not a barrier. |
| Supply / demand zone, CHoCH, equal highs and lows | Match the slide closely enough. | |

Net: the slide gets supply and demand, CHoCH and equal highs right, and gets FVG, BOS, and strong versus weak highs wrong or backwards in writing. **The spoken version corrects BOS and FVG without saying so** — "the gap needs to be filled up, they will come back to hunt back whatever volume over there" is the retrace-into-the-gap entry, and CHoCH-then-BOS is the standard sequence. Strong versus weak highs is the one that stays muddled. Use the standard definitions, which is what the TradingView indicator labels anyway.

### 3.4 How SMC fits the MMT stack

- **Demand zones and FVGs are pullback targets**, the same role the faster EMAs play in the 5-line set. A pullback that lands on an EMA *and* a demand zone or FVG is a stronger SPE entry than either alone.
- **Equal highs and lows are where the stop must not be.** Liquidity rests just beyond them and gets swept. A stop placed just below an equal low is the stop most likely to be run before the move. The Module 1 rule of a structural stop below EMA 55 (or 155) generally sits further away than an equal low, which is the safer side of this.
- **CHoCH on the 1-minute chart is the early exit warning**, ahead of the EMA cross-back. It fires when price breaks the last higher low in an uptrend, which usually happens before EMA 9 crosses EMA 25.
- The SMC add-on runs on **TradingView**, not Bybit. Settings from the "Steps to setting" screenshot (TradingView mobile app, THETAUSDT 1-minute chart):

| Indicator | Setting | Value |
|-----------|---------|-------|
| **Market Structure - By Leviathan** | BOS Confirmation | Candle (close) |
| | Show CHoCH | On |
| | Show Swing Points | On |
| | Show 0.5 Retracement Level | Off |
| | BOS line style | Dashed, grey |

This indicator labels BOS and CHoCH by the **standard** definitions in section 3.3, so on the chart BOS means continuation and CHoCH means a shift, whatever the slide's glossary says. "BOS Confirmation: Candle" means a break counts on a candle close beyond the swing point, not on a wick. That is the stricter and better choice on a 1-minute chart, where wicks through levels are constant.


## 4. Advance tool: New Indicators (添加新指标)

Two indicators, both on TradingView.

### 4.1 Donchian Trend Ribbon (唐奇安趋势带)

Slide definition: a technical indicator that displays the trend of price movements. Based on the Donchian Channel, it shows the direction of the trend over different time periods by plotting a series of coloured ribbon-like areas on the chart, to help traders identify trends more clearly.

**Setting** (TradingView, from the screenshot): Donchian Channel Period = **20**. Nothing else is changed.

What it is, beyond the slide: the Donchian Channel is the highest high and lowest low of the last N candles. The ribbon version stacks several Donchian lookbacks and colours each strip green or red depending on whether the current close is nearer the upper or lower band of that lookback. A solid green ribbon means price is at or near its N-bar highs across all lookbacks; solid red is the mirror; a mixed ribbon means the trend is not aligned across horizons.

How it fits: it is a second, indicator-based version of the "EMA on all timeframes" check from the Module 2 screener, but done on one chart with one glance. A solid ribbon in the direction EMA 155 gives is confirmation. A mixed ribbon is a Skip.

**What the session adds, and it is the most useful thing said about this indicator: the ribbon colour is a proxy for BOS.**

> "Usually **CHoCH is still remain green colour**, but down here there's a **BOS** here, so it change over here ... It's actually to show you **whether is a retracement or not. If let's say is a retracement, just only form the CHoCH, the colour still remains the same. But if let's say CHoCH form BOS, means changing trend even though a little bit, it will show change of colour, red.** ... But the moment form the BOS — see, this thing confirmatively this will change the colour to green and is uptrend."

So the mapping is:

| On the chart | Ribbon |
|---|---|
| Pullback, CHoCH only | **Colour holds.** It is a retracement; stay in |
| CHoCH **followed by BOS** | **Colour flips.** The structure broke; the trend has changed |

That makes the ribbon a **one-glance read of the SMC structure** on a chart where the BOS and CHoCH labels are small and constant. You do not have to find and judge the labels: the colour has already done it, and it only flips on the confirmation, not on the warning. Used this way it is not a duplicate of the EMA check at all; it is the SMC layer rendered as a colour bar.

Two caveats he states himself. "Donchian Trend Ribbon is **quite sensitive**" — on a 1-minute chart it will flip on small breaks, so read it with the timeframe you are actually trading. And "sometimes it may turn red colour if let's say confirmative", i.e. the flip can lag or arrive on a marginal break; it is confirmation, not prediction.

**Where it sits on the chart.** On the assembled CKBUSDT 1-minute chart it is the **solid colour bar along the bottom**, under the volume pane — not an overlay on price. The same bar is visible under the A8USDT 5-minute charts in the trade-call case ([06 §6](06-case-studies.md)), where it runs green through the pump and flips red around midday, which is when that trend actually ended.

### 4.2 Liquidation Heatmap (清算热力图)

Slide definition: a visual tool, particularly in futures, showing price areas where a high number of liquidations (forced selling or buying from insufficient margin) have occurred or are likely to occur. Three features listed:

| Feature | Slide text |
|---------|-----------|
| Colour coding | Warmer colours (red, orange) mark high-liquidation areas; cooler colours (blue, green) mark low. |
| Clusters | Clusters at specific price levels show where many traders are trapped, which can lead to rapid moves. |
| Support and resistance | Liquidation clusters frequently align with support and resistance zones, giving possible reversal points. |

Closing text: anticipate where liquidations might create volatility, and use that to plan entries and exits or to avoid high-risk areas.

No source or setting is given on this slide. The RAVE example in Module 5 shows the **Coinglass** Liquidation Heatmap (1-week view, liquidity threshold 0.26), so that is the source — but **the session gives his actual default as the 12-hour view** (4.2a), and the slide's "warm red and orange" colour description does not match the tool, which is yellow-hot on a blue-black field. The slide text also contains literal markdown bold markers (`**Liquidation Heatmap**`), so it was pasted from an AI-generated answer.

How it fits: a liquidation cluster is a **liquidity target**, the same thing SMC calls an equal high or equal low. Price is drawn toward it and often reverses after sweeping it. Two uses that follow from that:

- A cluster just beyond your stop is a reason to move the stop, because the sweep will take it before the move you want.
- A cluster ahead of your entry in the trade direction is a natural take-profit level, and often a better one than "nearest resistance" from the Module 1 Discharge rules, because it is where the opposing side gets forced out.

### 4.2a The heatmap in practice: the app, the timeframe, and reading a band

Eleven screenshots of the **Coinglass mobile app** walking the whole tool, on Binance BTC/USDT dated 9 November 2024 with BTC around 76,400.

**The colour scale, in his words:**

> "Basically you just want to recognise what? Colour, cluster, support, resistance level. How you determine it? **The hottest colour is yellow, the cooler colour is the darker blue, marine blue, or even nearly to black. Black is no liquidity.** The hotter the colour it is, the higher the liquidity is there ... Yellow are the heat, are the liquidity. Green relatively not that much of liquidity, and the marine blue is even worse — not much money there."

| Colour | Liquidity resting there |
|--------|------------------------|
| **Yellow** | Hottest. The cluster |
| Green | Moderate |
| Marine / dark blue | Little |
| Black | **None** |

Note this is Coinglass's **viridis** scale, not the "warm red / orange" the slide's pasted text describes. The slide is wrong about the colours of the tool it is describing; go by yellow-hot.

**The timeframe, and it corrects the SOP.**

> "**Usually, I use 12 hours model. 24 hours is for longer period.**"

His default is **12h**, not the 1-week view the RAVE screenshot happened to use. Both are in the material; the spoken default wins, and 1 week is for context rather than for a trade. The dropdown offers 12h · 24h · 3 day · 1w · 1mo · 3 month · 6mo · 1y.

**Where it is, on the app.** Coinglass → **Liquidation Map** tab → **Liquidation Heatmap** sub-tab → two toggles (**Pair | Symbol**, and **Model 1 | Model 2**) → the exchange-pair selector → the timeframe dropdown. The pair selector lists BTCUSDT Perpetual on Binance, OKX, Bybit, Bitget, HTX, BingX and Deribit separately, so you can read the book you are actually trading — **use the Bybit row**, since Bybit is where the order goes.

**Reading a single band.** Tap a band and a tooltip gives the timestamp, the **price**, and the **"Liquidation Leverage"** — the size of the cluster in dollars. From the screenshots: 77,643.44 → **84.08M**; 75,949.64 → **66.77M**; 78,490.34 → **28.53M**; 74,989.82 → **26.79M**. So the tool gives you a number, not just a colour, and clusters can be ranked. That is what makes a heatmap level usable as a Wick Tracker target: you can say "the nearest 80M band above me is at 77,643" rather than "it looks bright up there".

**Model 1 versus Model 2, unexplained.** He never says what the toggle does or which he uses. From the screenshots the two render differently on the same 12h window: one produces **sharp discrete bands** with a scale maximum of 84.08M over a 72,901–80,015 range; the other a **smoothed field** topping out at 29.73M over a wider 69,747–83,730 range. So the two models disagree about both where the liquidity is and how much of it there is, which is worth knowing before you place a target on one of them. Open question: what the two models assume, and which one the course uses.

### 4.2b "Support and resistance" is the wrong word, and it matters

Both the slide and the spoken version call the clusters support and resistance. A liquidation cluster is **not a barrier. It is a magnet.**

A bright band below price is where **longs** get force-closed. Price is drawn down to it; when it is reached the forced selling accelerates the move *through* it. A band above price is where **shorts** get force-closed, and price is drawn up into it. In both cases the cluster is a **destination**, and the reversal — if it comes — happens *after* the liquidity has been consumed, not at the edge of the band.

Treating a cluster as support means buying into the level where the forced selling starts. That is the single most expensive way to misread this tool.

The consequences, which are the same two already in 4.2 and are worth restating as rules:

| Cluster position | Correct use |
|---|---|
| Ahead of you, in your direction | **Take-profit target.** The wick that reaches it is the Wick Tracker's wick |
| Just beyond your stop | **Move the stop**, or lower the leverage. The sweep will take you out before the move you want |
| Below, after a crash has already hit it | **Entry**, once the sweep is done — the RAVE "heel" trade ([05 §3.9](05-risk-and-hedging.md)) |
| Between you and your target | Expect a violent candle there, not a pause |

This is the same error as the SMC glossary's "weak high = resistance" ([03 §3.3](03-entry-direction.md)): liquidity resting beyond a level is a target, not a wall. **His own practice is right in both places** — the Wick Tracker aims at clusters, and the RAVE entry buys after one is swept — it is only the vocabulary on the slides that is backwards.

### 4.3 The full chart stack, assembled

| Platform | Indicator | Setting | Job |
|----------|-----------|---------|-----|
| Bybit | Heikin-Ashi candles | on | Trend strength and exhaustion by candle shape |
| Bybit | EMA ×5 | 9, 25, 55, 155, 255 | Direction (155) and pullback levels |
| Bybit | MACD | 8, 13, 9 | Momentum on the pullback |
| Bybit | Volume | VOLMA 5, 10 | Confirmation, 2× spike = exhaustion |
| TradingView | Market Structure (Leviathan) | BOS on close, CHoCH on | Structure: continuation vs shift |
| TradingView | Donchian Trend Ribbon | 20 | Multi-horizon trend alignment |
| Coinglass | Liquidation heatmap | 1w view, threshold 0.26 | Liquidity targets for stops and TP |

Seven tools on a 1-minute chart. The course has not said how they are prioritised when they disagree. The only ordering stated so far is EMA 155 first (direction), then the others. Treat the rest as confirmations, and treat any two in conflict as a Skip until a slide says otherwise.

## 5. Trend line, Support & Resistance, Tunnel trend line

Title slide only: "How to draw: trend line, support and resistant line, tunnel trend line" (如何画出：趋势线、支撑线和阻力线、通道趋势线). Confirmed from the session: the course teaches the **standard market construction** with no MMT-specific variation. Nothing to reconcile with other modules.

Standard construction, for reference:

- **Trend line**: in an uptrend, a line under at least two higher lows; in a downtrend, over at least two lower highs. A third touch validates it.
- **Support and resistance**: horizontal lines at prior swing lows (support) and swing highs (resistance). The Module 1 take-profit rule, "nearest resistance", is read off these.
- **Tunnel (channel) trend line**: the trend line plus a parallel line through the opposite swing points. Price oscillates between the two; the far line is the take-profit target and the near line is the pullback entry.


## 6. Seahorse pattern (海马图案)

### 6.1 What it is

Three slides. The first is four photographs of seahorses. The second and third carry the actual content, with an ETHUSDT 15-minute Bybit chart as the example.

Slide text, verbatim: "I noticed whenever this kind of 'Animal Head with long beak' is definitely sideway trend with fluctuating trend, so just stay and observe, don't go in, otherwise you may end up chasing the ups and downs later on. Please BEWARE of this, to avoid PAINFUL LOSS!!!"

The shape, read off the ETH chart:

| Seahorse part | Chart feature |
|---------------|---------------|
| Tail and body (vertical) | A sharp, near-vertical rise: ETH from 1,571 to 1,698 in about 90 minutes |
| Head with long beak (horizontal) | The flat chop that follows: price oscillates in a narrow band around 1,660 to 1,680 for six or more hours, with the EMAs converging and flattening underneath |

**Rule: when the vertical move has ended and the "beak" is forming, do not enter. Watch.** It is the Module 2 "ranging" condition and the Heikin-Ashi doji-cluster condition, described by shape instead of by indicator. The trap it names is chasing: buying the small green candles in the beak because the big move is still fresh in memory, then selling the small red ones.

This is the clearest Skip rule in the course, and the only one described as a pattern to avoid rather than one to trade. Its mirror image, a slow decline ending in a vertical rise, is the hockey stick in Module 2 section 6.

### 6.2 The chart's indicator set is not the MMT set

The ETH chart shows **EMA 10, EMA 25, EMA 50**, plus WR (14, 20) and RSI (6, 12, 24) panels. That is a different, older setup from the 5-line 9/25/55/155/255 set taught earlier in this module. It answers the Module 1 puzzle: the stop rule "below EMA 50" comes from this older three-line setup, not from the current five. On the current set the nearest equivalent is EMA 55.

### 6.3 The third slide: a lifted personal post, and a contradiction of the course's own rules

The third seahorse slide is not course material in the same sense as the rest. It reads as a personal chat or Telegram post pasted onto a slide ("Both such above indicators cause me a profit gain for today market...", "HP mobile App" meaning handphone). Its four bullets, verbatim:

1. "Both such above indicators cause me a profit gain for today market."
2. "Sometimes, you should look out from the box (I mean the view of the market trend)."
3. "This method only suitable to those no enough time to stare at the PC screen (only using HP mobile app) and **no need TA at all** to trade, to look at the market and predict the trend."
4. "I created my own way of observation towards current market flow in order to help others especially the newbies to join as new traders and dare to gain more experience in trading too. **I do not set any SL, but increase all my leverage with cross margin.**"

Bullet 4 contradicts the Discharge rule from Module 1 ("stop loss: below EMA 50, structural, not emotional", "a doctor never admits a patient without a discharge plan"), the Dose rule ("your Dose is your position size and stop loss"), and the screener's own warning about manipulation, pump and dump and black swans. No stop, maximum leverage, cross margin means the entire account is collateral for every position, and one adverse move of a few percent liquidates all of it. It also contradicts the "aggressive" row of the very next slide, which says to set a stop loss.

Bullet 3, "no need TA at all", contradicts the whole of Modules 1 to 3.

Treat this slide as a historical artefact of how the author traded before the 3D method was formalised, not as a rule. If it was presented in the session as current advice, that is the single most important thing to raise with Dr. Aaron.

## 7. "My tips of scalping strategy"

Delivered at the end of Module 3 but it is Dose and Discharge content; it will be cross-referenced from Module 5. Four rows, verbatim:

| Tip | Text |
|-----|------|
| Amount | Set the amount 1% to 10% (appetite dependent) |
| Conservative | Isolated margin, less leverage, 1× to 10×, set TP and SL |
| Aggressive / risk taker | Cross margin, maximise leverage, **no TP / set SL** |
| Entry | Setting entry price with prediction |

Reading:

- **"Amount 1% to 10%"** is the first number the course gives for Dose. It is ambiguous whether this is *margin* per trade as a share of account, or *risk* per trade (the amount lost if the stop hits). The two differ by the leverage factor. At 10% margin and 50× leverage, the notional is 5× the account and a 2% adverse move wipes the margin. Ask which one is meant. If it is margin, then at high leverage the real risk per trade is far above the usual 1% to 2% of account that scalping textbooks use.
- **Conservative row** is the Module 1 Discharge rule applied: isolated margin caps the loss at the margin posted, TP is set first, SL is structural.
- **Aggressive row**, "no TP, set SL": lets winners run past the nearest resistance, with the stop as the only exit. Combined with cross margin and maximum leverage, the stop is doing all the work, and slippage on a fast 1-minute move can make the fill materially worse than the stop level. This row at least keeps a stop; the seahorse slide above drops it.
- **"Setting entry price with prediction"** means placing a limit order at the level you expect the pullback to reach (an EMA, a demand zone), rather than a market order. That is the Sniper Price Entry mechanic, and Module 4 should make it precise.


## Open questions

- Is the "1% to 10% amount" margin per trade or risk per trade? The answer changes real risk by the leverage factor.
- Was the "no SL, max leverage, cross margin" bullet presented as current advice or as a past habit?

- ~~Which timeframe is the Heikin-Ashi read on for entries?~~ Answered: the Bybit setup screenshots use the 1-minute chart.
- Is the EMA in Module 1 computed on Heikin-Ashi candles or real candles? The two give different crosses.
- ~~Which are the 3 Main Indicators and the MACD setting?~~ Answered: EMA (9/25/55/155/255), MACD (8/13/9), Volume (default).
- What volume multiple counts as a spike on the 1-minute chart, and is the baseline VOLMA 5 or VOLMA 10?
- ~~Which SMC indicator and platform?~~ Answered: TradingView, Market Structure by Leviathan.
- ~~Which site supplies the liquidation heatmap?~~ Coinglass, per the RAVE example screenshot in Module 5.
- When two of the seven chart tools disagree, which wins? Only EMA 155 has stated priority.
- ~~In the ZETA example, which of the five EMAs did price pull back to for the SPE entry?~~ Answered: any of them. He walks the chart parking at successive lines and points at **EMA 155** as the one to base the count on. EMA 9 is the first and shallowest target; EMA 255 is "the last guard".
- Which two of the five EMAs (9, 25, 55, 155, 255) are the "basic" pair, and does the Module 1 stop rule's "EMA 50" mean EMA 55?
