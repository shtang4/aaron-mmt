# 07 — Course handouts (three PDFs)

Three PDF handouts supplied alongside the slides, all copyright Dr. Aaron MMT 2026. They are image-based, designed pages; one carries a NotebookLM watermark and the "Trade Anatomy" page shows a mock exchange UI with garbled text, so they were generated from the course material rather than written from scratch. Confirmed from the session: the handouts are **supplementary**; where they and the slides differ, the slides are the taught method. They are still worth reading because they are more internally consistent and more textbook-standard than the slides, and in several places they quietly correct them.

| Handout | Pages | What it is |
|---------|-------|-----------|
| MMT Coin Trend Screener cheat sheet ("System Blueprint v1.0") | 10 | The four screener checks, one page each, plus a confluence matrix |
| MMT Risk Management Checklist ("The Signal Radar") | 14 | The same four checks with a scorecard that sets position size by score, and a two-rule bottom line |
| MMT Trade Call Execution Guide | 5 | A pre-flight checklist version of the screener and a "final rule manifesto" |

All three are the **screener**. None covers SPE, the Wick Tracker, the climax exit, hedging or SSWB. "Risk management" in the second title means the screener plus two sizing rules.

## 1. What the handouts settle

### 1.1 Minimum confluence, and size by score (closes open question A1)

Risk checklist, "Confluence Action Scorecard", and the Trade Call guide's "Decision and Risk Management Guide" agree:

| Score | Action | Stop |
|-------|--------|------|
| **4 / 4** | Full planned size. High conviction. | Standard stop |
| **3 / 4** | **50% to 75%** of planned size. | **Tighter** stop |
| 2 / 4 | Tiny pilot position, or do nothing. Waiting is advised. | |
| 1 / 4 or conflict | **Do not trade.** "You have zero edge here. Patience itself is profit." | |

Trade Call guide, under the pre-flight checklist: "If your score is not 3 or higher in ONE direction, do not trade." Note "in one direction": a coin scoring 2 long and 2 short is a conflict, not a 2. **The spoken session is looser and grades by experience** (notes/08 part 3): beginners 4/4 or a cautious 3/4, intermediates down to 2/4, advanced traders even 1/4. The handouts' flat rule is the beginner row, which is the row that applies to a new student.

This is the first time the course scales position size by evidence. It is also a Dose rule the slides never had.

### 1.2 The depth check, defined (closes A2)

Screener cheat sheet step 4 and risk checklist step 4: compare the **ask-side** and **bid-side** depth.

| Book | Signal |
|------|--------|
| Lighter ask (thin sell side) | **Long**: less resistance moving up |
| Lighter bid (thin buy side) | **Short**: less resistance moving down |
| Equal sides | Neutral. Skip; no immediate edge |

Plus a "hidden sell wall" warning: total depth can look light while one large block sits at a single price. Do not enter into it; wait for it to be digested or pulled. Source: Bybit or Binance → Perpetual → Order Book / Depth Chart. This confirms the inference in Module 2 section 5.1. **But the spoken session states the opposite pairing** (long when the bid side is lighter); see notes/08 part 3. Unresolved.

### 1.3 Funding rate, with numbers and a bull-market override (closes A3)

Risk checklist, "Funding Rate Decision Card":

| 8-hour funding | Label | Signal |
|----------------|-------|--------|
| **+0.10% and above** | Extreme heat | Strong short bias. "The crowd has lost its mind." |
| **+0.05%** | Long squeeze risk | Short bias. Longs are paying you. |
| **about 0%** | Balanced | Neutral. Follow the EMA. No fee advantage. |
| **−0.01% and below** | Short squeeze | Long bias. Shorts are trapped and paying you. |

Cost receipt on the same page: a $10,000 position at +0.05% pays $5 per 8 hours, $15 a day, $450 a month. "Never blindly hold against high funding rates."

Screener cheat sheet, "Context Override: The Bull Market Reality Check": in a strong bull market almost every coin carries positive funding. **If the trend filters say long, accept paying the funding. Do not force a counter-trend short merely to collect fees against major momentum.** The confluence matrix records this as "Negative (or accept Positive in Bull)".

So the funding check is a scored layer with an override, not a veto. That is why the SOL hockey-stick long in Module 2 section 6.3 went ahead into positive funding: it was a 3-of-4, and under this scorecard it should have been at 50% to 75% size with a tighter stop.

### 1.4 Open interest, as a 2×2 (confirms the correction in Module 2 section 5.1)

Risk checklist, "OI Diagnostic Matrix":

| | OI up | OI down |
|-|-------|---------|
| **Price up** | Real buying, fresh capital. **Long.** | Short squeeze: shorts panic-covering. **Caution**, reversal likely. |
| **Price down** | Real selling, new shorts. **Short.** | Long covering: exiting longs, not real selling. **Neutral / weak.** |

Core rule: rising OI validates the price trend; falling OI invalidates it. The slides' "vice versa for short" was loose; this is the correct form. Source given: CoinGlass → Futures → Open Interest → chart line direction (the Bybit OI Data tab shows the same thing).

### 1.5 The stop and the risk rule, in writing (closes C3 and D2)

Both the risk checklist ("The Absolute Bottom Line") and the Trade Call guide ("Final Rule Manifesto") end on the same two rules:

1. **"Always set your stop loss before the entry order fills.** A single un-stopped trade in a highly leveraged market will instantly liquidate an account."
2. **"Never risk more than 1% to 2% of total account equity on any single trade setup, regardless of confluence confidence."**

And: "A missed trade costs nothing. A trade without a stop loss can wipe your account."

Two consequences:

- The stop rule the Golden Rules omitted and the hedging section replaced is stated as the first rule of the course's own handouts. The SOP's "never" list is now the handouts' position, not only mine.
- "Risk" here is **maximum loss**, a percentage of equity. That settles the Module 5 ambiguity (margin versus loss). The $20 stake with a 20% ROI stop is a $4 loss, 0.2% of a $2,000 wallet, well inside the rule. The 1% rule slide's "1% = $1,000" is now readable as loss, which implies a $100,000 account, and the SSWB $20 stake is the practice version.

## 2. What the handouts contradict

### 2.1 A third EMA setup

| Source | EMA configuration |
|--------|------------------|
| 2023 seahorse and GMX charts | EMA 10, 25, 50 (Bybit) |
| Module 3 slides, current method | EMA 9, 25, 55, 155, 255 (Bybit) |
| **Handouts** | **One EMA, length 20**, on TradingView ("Indicators → EMA → Length: 20") |

The handouts' direction rule is "price above or below the EMA 20 on Daily, 4H and 1H". The slides' direction rule is three full-body candles on one side of EMA 155 on the entry chart. These are different tests on different charts with different lines. They will agree in a clean trend and disagree at every turn. Confirmed from the session: the slides' EMA 155 rule is the taught one. The handouts' EMA 20 on three higher timeframes is an optional filter to run before it, and that is how the SOP uses it.

### 2.2 Is the 1-minute chart the entry chart or a danger zone?

- Screener cheat sheet, step 1: Day → 4H/1H → 15m/5m/5m → **1 Min, "micro-trend execution"**. And: "Scalping counter-trend on the 1-minute chart is permissible, but you must always refer back to the Daily."
- Risk checklist, same step: 1D highest priority, 4H high, 1H medium, 15M "precision timing", **"5M & 1M: Extreme noise. Danger!"**

The two handouts disagree with each other, and the second disagrees with the whole course, whose entry chart is the 1-minute (Module 3 section 1.5, every SPE example, the SSWB SOP). Confirmed from the session: **the 1-minute chart is the execution chart.** Direction from 1D/4H/1H, timing on 15m, execution on 1m. The risk checklist's "danger" line means a 1-minute chart read on its own.

### 2.3 Counter-trend is permitted, with reduced size

The slides implied all timeframes must agree. The handouts allow disagreement and grade it:

| Condition | Signal |
|-----------|--------|
| Daily + 4H + 1H all above EMA | Strong long |
| Daily + 4H + 1H all below EMA | Strong short |
| Daily up, smaller timeframes mixed or down | **Lean long / caution: reduce size** |
| All timeframes disagree | No signal: skip the coin |

So a short on a 1-minute hockey-stick-in-reverse while the daily is up is a "caution, reduce size" trade, not a forbidden one. Combined with 1.1, size is now a function of two scores: timeframe alignment and screener confluence.

## 3. The screener, final form

Merging slides and handouts:

| # | Check | Source | Long | Short | Weight |
|---|-------|--------|------|-------|--------|
| 1 | EMA 20 on 1D, 4H, 1H (bias) then EMA 155 three-candle rule on the entry chart (direction) | TradingView, Bybit | Above / three above | Below / three below | Mandatory. Mixed = reduce size. Conflict = skip. |
| 2 | Open interest with price | CoinGlass or Bybit OI Data | Price up + OI up | Price down + OI up | Scored |
| 3 | Funding | CoinGlass or Bybit Contract tab | ≤ −0.01%, or positive accepted in a bull | ≥ +0.05% | Scored; bull override |
| 4 | Order book depth | Bybit order book | Lighter ask | Lighter bid | Scored; equal = neutral; beware single walls |

Score 4 → full size, standard stop. Score 3 → 50% to 75% size, tighter stop. Below 3 in one direction → no trade. Stop resting before the fill. Loss at the stop ≤ 1% to 2% of equity.

## 4. What the handouts do not touch

SPE, the Wick Tracker, the climax exit, the Hunting SL, hedging, SSWB, the seahorse and hockey stick. Nothing in them supports or retracts the hedging section. They simply state the stop rule as absolute, which is the same thing.
