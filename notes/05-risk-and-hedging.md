# 05 — Risk Management + Hedge Your Position

Source: Module 5 slides, Momentum Mastery Trading (MMT), Dr. Aaron MMT, 2026.

Module contents (from the Module 5 section title slide, which maps each item to the 3D method):

| Item | 3D role |
|------|---------|
| Basic tool: risk management strategy by trading style and risk level | **Basic Dose** |
| SSWB | **Advance Dose** |
| Advance tool: MMT Hedging | **Discharge** |
| MMT Golden Rules | Follow up |

SSWB is new: it is not in the course outline from the opening slides. The acronym is not expanded on the title slide.

The last three slides of this batch carry a different copyright line, "Future Trends FZCO", instead of "Dr. Aaron MMT". They may be shared with another product of the same company.

## 1. Scalping tips (delivered at the end of Module 3)

Captured in [03-entry-direction.md, section 7](03-entry-direction.md#7-my-tips-of-scalping-strategy). Summary:

| Tip | Text |
|-----|------|
| Amount | 1% to 10%, appetite dependent (margin or risk per trade: unresolved) |
| Conservative | Isolated margin, 1× to 10× leverage, set TP and SL |
| Aggressive | Cross margin, maximise leverage, no TP, set SL |
| Entry | Set the entry price with prediction (limit order at the expected pullback level) |

## 2. Basic tool: Trading Style & Risk Level

Three slides, one table split across them. Transcribed in full.

| Aspect | Low Risk Trader | Medium Risk Trader | High Risk Trader |
|--------|-----------------|--------------------|------------------|
| Market conditions | Low to moderate volatility and high liquidity | Moderate to high volatility and liquidity | High volatility and liquidity |
| Timeframe | Medium to long-term (e.g. daily) | Short to medium-term (e.g. hourly) | Short-term (e.g. 1-minute) |
| Entry criteria | Strong confirmation signals, focus on long-term trends | Balanced approach with a mix of technical indicators | Quick entry based on short-term signals |
| Exit criteria | Conservative profit targets and tight stop-loss levels | Moderate profit targets and wider stop-loss levels | Aggressive profit targets and looser stop-loss levels |
| Risk management | Strict risk management, limited exposure per trade | Balanced risk management, adjust exposure based on volatility | Higher risk tolerance, larger position sizes |
| Trade execution | Patient and deliberate execution, avoid impulsive decisions | Timely execution with attention to market conditions | Quick execution to capitalise on short-term opportunities |
| Monitor trades | Regular monitoring with emphasis on long-term trends | Active monitoring with adjustments based on short-term indicators | Constant monitoring with quick adjustments |
| Psychological discipline | Emotionally disciplined, focus on long-term goals | Balanced emotions with a focus on managing short-term risks | High tolerance for volatility, able to handle rapid changes |
| Open interest (OI) | May consider for confirmation, but not primary focus | Consider changes in OI for insight into market sentiment | Monitor OI for quick insights into market direction |
| Technical indicators | Relies on fundamental analysis and long-term indicators | Utilises a mix of technical indicators for medium-term analysis | Focuses on short-term indicators for quick decision-making |
| Trading style | Conservative and methodical, with a focus on capital preservation | Balanced approach with a mix of caution and opportunity | Aggressive and opportunistic, aiming for high returns |

### 2.1 What the table implies about the MMT method itself

Read the table against the course as taught so far:

- **Every MMT student is in the "High Risk Trader" column by the table's own definitions.** The method uses the 1-minute chart, quick entries on short-term signals, constant monitoring, and OI as a direction input. Those are the high-risk column, row for row. The table is not offering a choice of style so much as describing what scalping is.
- **The high-risk column pairs "looser stop-loss levels" with "larger position sizes".** On a 1-minute chart, that is the combination that ends accounts: a wider stop with more size means a larger loss per stop-out, and stop-outs are frequent at that timeframe. The Module 1 Discharge rule (structural stop below the EMA) fixes the stop by the chart, not by appetite, and that is the better rule. Do not loosen the stop because you have decided you are a high-risk trader.
- **The "Low Risk Trader" column describes a different activity.** Daily timeframe, fundamental analysis, long-term trends. That is swing or position trading, and nothing in Modules 1 to 4 applies to it. It is not a lower-risk way to do MMT; it is not MMT.
- **The table does not connect to the course's own numbers.** The "1% to 10% amount" and the isolated-versus-cross split from the tips slide are the operational risk choices, and the table does not reference them. The only defensible mapping: conservative tips row = isolated, 1× to 10×, 1% to 2% amount, TP and SL set; aggressive tips row = the high-risk column. Whether the medium column corresponds to anything the course teaches is unclear.

### 2.2 The one usable instruction

Pick a column and stay in it. The failure mode the table is guarding against is mixing columns within a session: a high-risk entry (1-minute, quick) with a low-risk exit (tight stop, conservative target) gets stopped out constantly; a low-risk entry with high-risk sizing blows up on the one loss. The style, the stop width, the position size and the monitoring cadence have to come from the same row.


### 2.3 The ZETA case: "Right trade, but take profit too early?"

TradingView, ZETAUSDT perpetual (Bybit), **4-hour** chart, with a Multi EMA overlay. Trade markers on the chart:

| Event | Chart marker | Price | Date on chart |
|-------|-------------|-------|---------------|
| Entry | "SPE Entry" line, "Buy 1000" | 0.8570 | around day 2 |
| Retrace | Orange circle labelled "Take Profit?" | from about 1.90 down to about 1.20, over roughly a week | days 4 to 10 |
| Exit | "Wick tracker, Exit" and "Sell 1000" | 2.8530 | around day 16 |

The entry price is the same 0.8570 as the ZETA 1-minute SPE example in Module 3. It is one trade shown at two timeframes: entered on the 1-minute chart, held for about two weeks on the 4-hour chart, exited at roughly +233%.

Slide caption: "You exited early, then watched the price pump without you." Follow-up slides:

- **"The problem wasn't the trade."** Your direction and entry (Diagnose) may be correct. The wrong position size (Dose) created too much pressure to hold.
- **"Do you know exactly how much you could lose?** Or do you decide your position size based on how confident you feel?"
- **"What is your risk level?** Can you stay calm when the position moves against you? Your position size must match your capital, experience and emotional tolerance."

### 2.4 What is right and what is wrong in the ZETA argument

**The behavioural claim is sound.** An oversized position makes a normal retrace feel unbearable, and the trader exits to relieve the pressure rather than because the chart said to. Sizing so that the retrace is tolerable is the correct fix, and it is the first time the course states *why* Dose matters rather than *that* it matters.

**The example undermines three things the course has already taught:**

1. **It is not a scalp.** A two-week hold on a 4-hour chart is a swing trade. Module 1 defined scalping as seconds to minutes. The course's showcase trade is the opposite of its definition.
2. **It contradicts the Module 1 exit rule.** "Short-term EMA crosses back below long-term EMA, exit, no questions." On the chart, the retrace from 1.90 to 1.20 gave back more than half the open gain and the fast EMAs crossed down during it. The Discharge rule as written would have exited in the 1.4 to 1.6 area. The slide says the correct behaviour was to hold. Both cannot be the rule. Either Module 4's "New TP" and Wick Tracker replace the EMA cross-back exit, or the ZETA hold was luck presented as discipline.
3. **It is hindsight-selected.** The lesson "hold through the retrace" is only visible because ZETA then tripled. The same retrace on a coin that did not recover would be the seahorse pattern from Module 3, with the instruction "don't go in". Nothing on the slide distinguishes the two at the time the circle was drawn.

The safe reading: size so you *could* hold, then let the written Discharge plan decide whether you *do*. Do not convert "I sized correctly" into "therefore I never take profit on a retrace".

## 3. Advance Dose: Enhancement of Risks Management, and SSWB (Start Small Win Big)

Five slides titled "Enhancement of Risks Management", a "1% Risk Rule" slide, and then the SSWB slides. SSWB is expanded on its own slide as **Start Small Win Big**.

### 3.1 Basic trading concepts

Transcribed:

| Concept | Slide explanation |
|---------|------------------|
| Isolate mode | Allocate a specific amount of funds to each trade individually. Protects your other trades from affecting each other. |
| Cross mode | Uses your entire account balance as margin for all trades. Flexible sizing, higher liquidation risk. |
| Leverage × | How much your position size is amplified compared to your margin. 10× means trading with ten times your margin. |
| Liquidation | Account balance falls below a level and trades are closed automatically. Manage risk and set stop-loss orders to avoid it. |
| Derivative account | Used for futures contracts; speculate on price without owning the asset. |
| Funding account | Stores funds; deposit and withdraw here to fund trades. |

### 3.2 Isolated versus cross, leverage, and stop-loss tiers

Slide text:

- Take care of the trade by adjusting: isolated with leverage and SL, or cross with leverage and SL.
- **Isolate**: if liquidated, you only lose the capital you put in. The derivative wallet USDT is preserved.
- **Cross**: if liquidated, you lose not only the capital you put in; the total amount in the derivative wallet is liquidated ("Burst!!").
- **Isolate with 5× to 10× leverage**, as it can be adjusted. The smaller your leverage, the further away the liquidation price.
- **SL (stop loss) by risk level:**

| Level | SL |
|-------|----|
| Beginner (low risk taker) | 5% to 20% |
| Intermediate (moderate risk taker) | 20% to 50% |
| Advance (high risk taker) | above 50%, "on the amount that comfortable" |

**These percentages are ROI on margin, not price.** The Bybit TP/SL screen sets the stop as "Trigger by ROI (%)", and the screenshots in section 3.4 confirm it. Converting to price distance:

```
price distance = entry × (ROI% ÷ leverage)
```

So a beginner's 20% stop at 10× leverage is a 2% price move; at 25× it is 0.8%. An "advanced" 50% stop at 25× is still only a 2% price move. On a 1-minute crypto chart, 0.8% is inside normal noise, which is why the next slide is about giving the stop room.

This also resolves the "cross margin, no SL" bullet from the Module 3 seahorse slide: the course's own risk module says cross margin liquidation takes the whole wallet, and prescribes isolated at 5× to 10× with a stop. Treat the seahorse bullet as superseded.

### 3.3 Partial take-profit, breakeven stop, and the "Hunting SL"

Slide text:

- **SL to entry once partial TP (PTP)**: after taking part of the profit, move the stop to the entry price. The remainder can no longer lose.
- **Moving SL / Hunting SL**: a trailing stop that locks in a chosen fraction of the open profit. Set a percentage "in order for it to have more space for the wick to hit without triggering your SL easily."

**Formula, worked on the slide** (a short on THETAUSDT, entry 2.814, 25× leverage):

| Lock in | Calculation | SL trigger price |
|---------|-------------|-----------------|
| 20% ROI ("left 80% for the wick") | 2.814 × 20% = 0.5628; ÷ 25 = 0.022512; 2.814 − 0.022512 | **2.791488** |
| 60% ROI ("left 40% for the wick") | 2.814 × 60% = 1.6884; ÷ 25 = 0.067536; 2.814 − 0.067536 | **2.746464** |

The arithmetic is correct. In general form:

```
SL price (short) = entry − entry × (locked ROI ÷ leverage)
SL price (long)  = entry + entry × (locked ROI ÷ leverage)
```

The slide labels each line "Entry Price", which is a labelling slip; the first line computes the price distance and the second the trigger price.

"Left 80% for the wick" is loose. Locking 20% ROI does not leave 80% of anything; it leaves whatever open ROI exists above 20% exposed to a wick. In the screenshot the open ROI was about 55%, so the 20% lock left about 35 ROI points of room, and the 60% lock would have been *above* the current open profit and unsettable without price moving further first.

### 3.4 The Bybit screenshots, checked

THETAUSDT 1-minute, a short. Position: qty 43.2, entry 2.814, mark 2.7515, liquidation 3.0493. TP set at 2.4765 (ROI 299.84%). Two SL screens, both labelled "Hunting SL":

| SL trigger (Mark) | ROI shown | Expected profit shown |
|-------------------|-----------|----------------------|
| 2.7914 | 20.07% | 0.9763 USDT |
| 2.7464 | 60.05% | 2.9203 USDT |

Cross-checks:

- Notional = 43.2 × 2.814 = 121.6 USDT; at 25× the margin is 4.86 USDT.
- Profit at 2.7914 = (2.814 − 2.7914) × 43.2 = 0.976 USDT. Matches. ROI 0.976 ÷ 4.86 = 20.1%. Matches.
- Profit at TP 2.4765 = 0.3375 × 43.2 = 14.58 USDT. Matches the 14.5799 shown. ROI 300%. Matches.

So the formula, the screenshots and the Bybit ROI display all agree. One observation: the liquidation price 3.0493 is 8.4% above entry. Pure isolated 25× would liquidate at roughly 3.5% to 4%. Either extra margin was added to the isolated position or the account is on cross. The slide does not say. Given section 3.2's own advice, check which mode the demo account was in.

Also on the chart: the EMA header reads EMA 9, 25, 55, 155, 255 and the MACD reads (8, 13, 9). The demo chart is running the exact Module 3 settings.

### 3.5 The 1% risk rule

Slide, verbatim: Total Wallet = Risk Amount ÷ Risk Percentage. Given risk amount 1,000 USDT and risk percentage 1%, total wallet = 1,000 ÷ 0.01 = **100,000 USDT**. "If 1% risk equals 1,000 USDT, the wallet should be 100,000 USDT."

The arithmetic is trivial and correct. The framing is backwards from normal practice: a risk rule is applied *from* the wallet (risk = wallet × 1%), not used to derive the wallet you would need. Read as written, the slide says: if you are putting 1,000 USDT into a trade, you should have 100,000 USDT behind it. The ZETA case study bought 1,000 units, which at 0.857 was about 857 USDT of notional, in that ballpark.

**What "risk amount" means here is still not pinned down.** Two readings:

1. Risk = maximum loss at the stop. Then 1,000 USDT risk with a 20% ROI stop means 5,000 USDT of margin per trade.
2. Risk = margin posted on an isolated position, on the logic of section 3.2 that "if liquidated you only lose the capital you put in". Then 1,000 USDT is the margin, and at 25× the notional is 25,000 USDT.

The course's isolated-margin framing points to reading 2. If so, "1%" is 1% of the wallet as **margin**, and the loss at a 20% ROI stop is 0.2% of the wallet, which is conservative. Without a stop, the loss on liquidation is the full 1%. This is consistent with the "1% to 10% amount" tip from Module 3, and it makes the tip a margin rule, not a risk rule.

### 3.6 The Dose procedure, assembled

Putting sections 3.2 to 3.5 together into the order you would do it:

1. Isolated margin. Leverage 5× to 10× for a beginner; the demo uses 25×.
2. Margin per trade = 1% to 10% of wallet, by appetite. Start at 1%.
3. Initial stop by ROI tier: 5% to 20% for a beginner. Convert to price with entry × ROI ÷ leverage and check it sits beyond the structural level (EMA 55 or 155, an equal low). If it does not, either widen the ROI or reduce leverage until it does; do not move the structural level.
4. Take profit set first, at the nearest resistance or a liquidation cluster.
5. On a partial take-profit, move the stop to entry.
6. Thereafter, trail with the Hunting SL formula, locking a rising fraction of the open ROI.


### 3.7 High-capital trading risk

A table of ten trades at increasing capital, with the loss at 5%, 10% and 30% per trade, in USD and MYR (at RM 4.50 per USD):

| Trades | Capital per trade | 5% loss | 10% loss | 30% loss |
|--------|------------------|---------|----------|----------|
| 1 to 2 | $1,000 | $50 | $100 | $300 |
| 3 to 7 | $2,500 | $125 | $250 | $750 |
| 8 to 10 | $3,000 | $150 | $300 | $900 |
| **Total** | **$23,500 (RM 105,750)** | **$1,175 (RM 5,287.50)** | **$2,350 (RM 10,575)** | **$7,050 (RM 31,725)** |

The totals add up. The point of the slide is the bottom-right cell: at this scale, a bad run of 30% losses costs RM 31,725, which for the course's Malaysian audience is a serious sum. It is the setup for the "start small" argument.

Followed by the disclaimer slide: "There is no always 100% guaranteed method in future trading, especially during the news, FOMC, or unexpected market events."

### 3.8 SSWB: Start Small Win Big

Framing slide. Three student objections quoted: "How much money am I risking each trade?", "Small capital can start?", "Small capital cannot make meaningful returns from trading." Verdict: **"Wrong. Capital size does not determine your result. The correct Dose does: how much you are putting in for a trade. The percentage is identical."**

Comparison slide:

| Common people | Our students |
|---------------|--------------|
| Feel capital too small | Start small |
| Overleverage to grow fast | Trade with structure |
| One loss hurts badly | Scale with discipline |
| | **$150 trade capital method** |
| | Risk control first |
| | Grow through execution, not gambling |

**The $150 number.** This is the concrete Dose for students: $150 of margin per trade. Against the 1% rule slide (1% = $1,000 implies a $100,000 wallet), $150 at 1% implies a $15,000 wallet, and at 10% a $1,500 wallet. The course does not say which; "start small" suggests $150 is simply the fixed starting stake regardless of wallet, and the percentage rule applies once the wallet grows. The two slides are not reconciled.

"The percentage is identical" is true and also the weak point of the argument. Returns scale with capital, so a $150 stake at the RAVE example's +277% is about $415 of profit. The claim that small capital *can* start is correct; the implied claim that it makes meaningful money is only true after compounding, and compounding a 1-minute scalping method assumes a positive expectancy the course has not yet demonstrated on a sample of trades.

### 3.9 Real example: RAVE, "$150 per trade that changed everything"

Three screenshots, captioned "Advance method: how to enter and exit."

| Screen | Platform | What it shows |
|--------|----------|--------------|
| Left | **Coinglass** Liquidation Heatmap, Binance RAVE/USDT, 1-week view, liquidity threshold 0.26 | Liquidation clusters as horizontal bands; the densest sit below price after the pump |
| Middle | TradingView, RAVEUSDT perpetual, 1-minute, with the Leviathan Market Structure indicator | BOS, CHoCH, EQL (equal lows) and "Strong Low" labels, plus horizontal liquidity levels at 19.19, 20.02, 21.65, and a low at 15.80 |
| Right | **Bitunix** app, RAVEUSDT, 5-minute | A spike to 1.86, a crash to 0.53, then an "Entry" arrow at about 0.507 on 04/02 17:45, followed by a recovery to 0.709. Position shows +277.33%. The MACD (8, 13, 9) panel has an annotation "IceBerg Tip" at the deepest point of the histogram trough |

Observations:

- **Three exchanges now appear in the course**: Bybit (main), BTCC (SOMI card, Module 2), Bitunix (this). The scanning and indicator setup is Bybit and TradingView; the result screenshots come from wherever the trade happened to be.
- **The entry is a crash-bottom buy.** RAVE pumped from about 0.5 to 1.86 and collapsed back to 0.53 within hours. The entry at 0.507 is a bid into the collapse, at the level where the Coinglass map shows liquidations clustered. That is a liquidity-sweep reversal, and it is the opposite of the trend-following entries in Modules 1 to 3 (EMA 155 direction, pullback to an EMA). The "advance method" is a different trade type.
- **"IceBerg Tip"** appears to name the extreme of the MACD histogram trough as the reversal cue: the deepest red bar, with the next bar shorter. Read alongside the volume spike at the same candle, it is the exhaustion signal from the Module 3 volume section. This is an inference from the annotation; the slide gives no definition.
- **The arithmetic**: 0.507 to 0.709 is +40% on price. +277% ROI implies roughly 7× leverage on $150, so about $415 of profit. Consistent with the "start small" numbers.
- **The heatmap dates (04-12 to 04-19) do not match the trade date (04/02).** The heatmap screenshot is illustrative, not the one used for this entry.

## 4. Advance tool: MMT Hedging (Discharge)

_Not yet captured._

## 5. MMT Golden Rules (Follow up)

_Not yet captured._

## Open questions

- Is the "1% to 10% amount" margin per trade or maximum loss per trade? The isolated-margin framing in section 3 points to margin. Confirm.
- The demo account trades at 25× while the slide prescribes 5× to 10×. Which is the course's actual recommendation?
- Was the THETA demo position isolated or cross? Its liquidation distance (8.4%) does not match isolated 25×.
- ~~What does SSWB stand for?~~ Start Small Win Big.
- Is the $150 per trade a fixed starting stake, or 1% to 10% of some assumed wallet? The 1% rule slide and the $150 slide are not reconciled.
- What exactly is the "IceBerg Tip" on the MACD, and is the crash-bottom entry in the RAVE example a taught setup or a one-off?
- Does Module 4's New TP or Wick Tracker replace the Module 1 "EMA cross-back, exit, no questions" rule? The ZETA case says hold through a cross-back; Module 1 says exit on it.
- Is hedging (section 4) a replacement for the stop loss or a tool used alongside it? This is the question that decides whether the Discharge rule survives contact with Module 5.
- What are the Golden Rules, and do they resolve the "no SL, cross margin" contradiction in the Module 3 seahorse slide?
