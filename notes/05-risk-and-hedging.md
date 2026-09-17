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

The entry price is the same 0.8570 as the ZETA 1-minute SPE example in Module 3. It is one trade shown at two timeframes: entered on the 1-minute chart, held for about two weeks on the 4-hour chart, exited at roughly +233% of price.

**ZETA was a day-one or day-two listing when she entered.** From the walkthrough: "that time this coin just started day 1 or day 2 only ... she managed to enter at this pricing, 0.8570." The monthly chart carries three candles in total. So the trade breaks **Golden Rule 4** (new-born coins, a few days only) as well as Golden Rule 6, and the EMA 155 it was entered on had about two and a half hours of a brand-new listing behind it on the 1-minute chart. See [03 §2.3](03-entry-direction.md).

**The Jane case study names the leverage: 50×** ([06 §7.2](06-case-studies.md)). Her Bybit card carries exactly these prices, 0.8570 to 2.8530, and reads **+11,339.67% ROI**. So this slide's lesson — hold through the retrace, do not take profit too early — was taught over a **50× position held for two weeks**, on which roughly a 2% adverse move is a liquidation at any point before the gain builds. The retrace it praises (1.90 down to 1.20) was survivable only because price was already more than double the entry by then. Nothing about the argument transfers to a position taken at 50× and then retraced early, which is the position a student copying it would be in.

Slide caption: "You exited early, then watched the price pump without you." Follow-up slides:

- **"The problem wasn't the trade."** Your direction and entry (Diagnose) may be correct. The wrong position size (Dose) created too much pressure to hold.
- **"Do you know exactly how much you could lose?** Or do you decide your position size based on how confident you feel?"
- **"What is your risk level?** Can you stay calm when the position moves against you? Your position size must match your capital, experience and emotional tolerance."

### 2.4 What is right and what is wrong in the ZETA argument

**The behavioural claim is sound.** An oversized position makes a normal retrace feel unbearable, and the trader exits to relieve the pressure rather than because the chart said to. Sizing so that the retrace is tolerable is the correct fix, and it is the first time the course states *why* Dose matters rather than *that* it matters.

**The example undermines three things the course has already taught:**

1. **It is not a scalp.** A two-week hold on a 4-hour chart is a swing trade. Module 1 defined scalping as seconds to minutes. The course's showcase trade is the opposite of its definition.
2. ~~**It contradicts the Module 1 exit rule.**~~ **Resolved by the closing slide of the same case** ([06 §7.5](06-case-studies.md)). "Short-term EMA crosses back below long-term EMA, exit, no questions" would have exited in the 1.4 to 1.6 area on the retrace. The Wick Tracker at 2.8530 is what actually closed it, and that level was chosen **before the trade** — so Module 4's Wick Tracker does replace the Module 1 cross-back exit as the primary target, with the cross-back demoted to the runner's backstop. The hold was not luck presented as discipline: the exit existed in writing and it fired one and a half cents under the eventual high.
3. **It is hindsight-selected — but he shows the other side himself.** "Hold through the retrace" is still only visible because ZETA recovered, and nothing on this slide distinguishes that retrace from a seahorse at the time the circle was drawn. What has to be said in the course's favour: the closing slide of the case is the **weekly chart to April 2026, ZETA at 0.04533**, titled "Current Price (Never exit will liquidate)". He puts the cost of the opposite error on screen, on the same trade.

**The two slides are one rule, and only together.** This slide prices exiting *early*: you miss the pump. The closing slide prices *never* exiting: you are liquidated, and on this coin the decline was 98% from the high. Neither is a rule on its own. Together: **take the written level — not sooner, not never.** That is a well-built teaching pair, and it is the answer to "when do I get out" that the rest of the deck circles around.

The safe reading: size so you *could* hold, then let the written Discharge plan decide whether you *do*. Do not convert "I sized correctly" into "therefore I never take profit on a retrace", and do not convert "hold through the retrace" into "hold past the target".

**One thing the whole ZETA sequence never shows: a stop.** Entry and target, at four timeframes, across two modules, and no stop price anywhere. He says "it come back to hunt your stop losses" about a level never drawn. At the 50× the Jane card reports, a stop would have to sit inside about 1.7% of entry to be a stop rather than a liquidation notice, which on a day-two listing's 1-minute chart is inside the noise. Read honestly: **this trade had no survivable stop and the take-profit was doing the work of both.** Which is an argument for the leverage rule, not against the stop rule.

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
- **Isolate with 5× to 10× leverage**, as it can be adjusted. The smaller your leverage, the further away the liquidation price. **The spoken version is more conservative still** ([03 §7.1](03-entry-direction.md)): "reduce your leverage to probably 1 to 10× ... maybe you already more than beginner level towards the intermediate. **If not, maybe you can start from 1 to 5×.**" So the beginner figure is **1–5×** and 5–10× is the intermediate band. The SOP now carries the spoken numbers.
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


### 3.10 SSWB results slides, checked

Five slides of results. All of the trade evidence is Bybit "share" cards carrying referral codes (53G19B, AKX1BP). These cards are generated by the user for whichever position they choose to share, so they are a self-selected sample by construction. No losing trade appears on any slide.

**Headline slide.** "$150 per trade (±592 MYR) to make manager's salary (±5,000 MYR)." Before: 1,993.18 USDT available. After: 18,287.81 USDT. "Grow 1:9 RR. You don't need big capital, you need skill and knowledge."

- 1,993 to 18,288 is a 9.2× account multiple. "1:9 RR" is using RR (reward-to-risk) to mean that multiple, which is not what RR means. No dates are given, so the rate of growth is unknown.
- The arithmetic of the salary claim: 5,000 MYR is about 1,266 USD a month at the slide's own rate. On $150 stakes over about 22 trading days, that is roughly 38% ROI on the stake per day, net of losses, every day. At 25× leverage that is a 1.5% net price move captured daily. It is not impossible on volatile alts, but it is a strong claim, and nothing on the slide supports it beyond one before-and-after balance.
- The MYR rate differs across slides: 4.50 on the high-capital table, 3.95 here, 4.38 on the CARV slide. The slides were made at different times and not reconciled.

**BMT trade call, 13 March 2025.** Chat screenshots (Aaron, 18:41 and 21:19: "Who's in BMT? It's pumping!") beside the order ticket and result cards.

| Field | Value |
|-------|-------|
| Order | Open Long BMTUSDT at 0.08307 |
| Quantity | 5,332 BMT, cost 30.4705 USDT, value 442.93 USDT |
| Margin mode | **Cross, 15×** |
| Estimated liquidation | 0.05332 (35.8% below entry) |
| Result card | ROI +3,735.89%, current price 0.29324, unrealised +1,120.14 USDT |

Checks: 0.08307 to 0.29324 is +253% on price; ×15 is 3,795%, shown as 3,736% after fees and funding. 30.47 USDT × 37.4 is 1,139 USDT, shown as 1,120. The numbers are consistent.

**The problem is the margin mode.** The slide labels this "30 USDT capital", and section 3.2 of this same module says cross margin puts the whole derivatives wallet behind the position. The liquidation price confirms it: isolated 15× would liquidate about 6% below entry, and this position's liquidation was 36% below entry because the wallet was backing it. The real capital at risk was not 30 USDT. It was the wallet, down to a 36% drawdown in BMT. The course's showcase SSWB trade used the setup the course's own risk slide warns against.

**BMT chart slide.** A 1-hour BMTUSDT spot chart with two entries marked:

| Entry | Time | Price | Stop shown on chart | Exit price on card | RR label | Check |
|-------|------|-------|--------------------|-------------------|----------|-------|
| First | 13/3 18:41 | 0.0831 | 0.0744 | 0.2932 | 1:24 | (0.2932 − 0.0831) ÷ (0.0831 − 0.0744) = 24.1 |
| Second | 18/3 17:45 | 0.2045 | 0.1799 | 0.3063 | 1:4 | (0.3063 − 0.2045) ÷ (0.2045 − 0.1799) = 4.1 |

Both RR labels reproduce exactly from the chart's price levels, so they are **realised** RR: actual exit divided by planned stop, computed after the trade. That is a fine review metric and a useless planning one; nobody knew at 18:41 on 13/3 that the target was 0.2932. Note also that the first trade's stop at 0.0744 is 10.5% below entry, which at 15× is a 157% ROI loss, more than the 30 USDT margin. That stop is only fillable on cross margin.

Caption: "Late trade is a losing trade. If you don't know why, you're just copying stupidity." The second entry printed a +492.70% card at 10× before BMT fell from 0.32 to 0.15 over the following week. So the "late" trade also showed a large gain at one moment; whether it lost depends on the exit, which is not shown. The actual lesson is the one from Module 2 and the airport analogy: the trade call is the candidate, not the entry, and by the time the chat says "it's pumping" the pullback entry has usually passed.

**"A little progress every day" slide.** Seventeen share cards, mostly RAREUSDT longs at 25×, plus ORCA, REEF, APT and PENDLE:

| Row | Cards | P&L shown |
|-----|-------|-----------|
| Top | 9 cards, +101.80 to +481.90 | about 2,410 USDT |
| Bottom | 8 cards, +246.12 to +1,013.10 | about 5,024 USDT |

Several are **unrealised** P&L, which is an open position, not a result. Several RARE cards have different entry prices, so they may be adds to one position screenshotted at intervals rather than separate trades. Zero losses shown.

**CARV slide.** CARVUSDT short at 5×, entry 1.2638, current 0.7447, unrealised +5,191 USDT ("~22,740+ MYR"). A 41% price move at 5× is a 205% ROI, which implies about 2,530 USDT of margin. That is not a $150 trade. Alongside it: an "Always use a stop loss" graphic and two quotes ("Trading can't make you rich overnight but it is the best business in long term", "Behind every consistently profitable trader there is a lot of losses, mistakes and lessons learned").

### 3.11 What to take from the results section

- **The entry and sizing rules are the content; the cards are marketing.** Every number that can be checked reconciles, so the screenshots are real. What they are not is a track record: no losses, no dates, some open positions, and a referral code on every card.
- **The showcase trade contradicts the risk module.** BMT was cross 15× with a 30 USDT ticket and a wallet-backed 36% liquidation buffer. If you copy the ticket without copying the margin mode, you get liquidated at 6%. If you copy the margin mode, you are risking the wallet, which section 3.2 tells you not to do.
- **"$150 per trade" and the CARV trade are different scales.** The CARV short carried roughly 17 times the $150 stake.
- **RR in this course is computed after the exit.** For planning, use the Module 1 rule (TP at nearest resistance, set first) to fix the reward before entry, and compute RR from that.
- The one sentence on these slides that is a rule rather than a result: "Always use a stop loss." It is consistent with section 3.2 and inconsistent with the Module 3 seahorse slide, and the risk module wins.


### 3.12 The SSWB procedure (the actual SOP)

Eight steps, transcribed with light cleanup:

1. **Initiate** the capital: start with **$20** per trade.
2. **Choose the coin** by active volatility and volume percentage, usually from the Gainers list.
3. Use the **MMT Coin and Trend Screener** as the SOP to decide the trend.
4. **Enter using MMT SPE** and set the **MMT Wick Tracker to 50% = $10** (buffer to 55% to 60% to cover the closing fee). Sometimes set it lower than the previous high wick spike, and you may gain more than 50%.
5. It may take **30 minutes to 1 hour**, or more depending on volatility and volume, especially with wick candles.
6. Once the TP closes the position, **immediately transfer the profit from the Derivatives account to the Funding account** to keep it secure.
7. Repeat from step 1 for up to **10 trades** in a short scalping period. You may reach the **$100** target before 10 trades. Then **stop trading and rest**.
8. **Don't hold** for a longer time.

This is the first end-to-end procedure in the course, and it fixes the meaning of two Module 4 terms before Module 4 arrives: **SPE** is the entry, and the **Wick Tracker** is a take-profit set as an ROI percentage on the margin (50% ROI on $20 margin = $10), optionally placed at a prior wick high.

**The fee buffer is roughly right.** Bybit taker fees are about 0.055% per side. At 20× that is 2.2% ROI round trip; at 50× it is 5.5%. A TP at 55% to 60% ROI nets about 50% after fees at those leverages.

**What 50% ROI means in price terms:**

| Leverage | Price move needed for +50% ROI |
|----------|-------------------------------|
| 12.5× | 4.0% |
| 20× | 2.5% |
| 50× | 1.0% |

**The "compounding" table** ("$100 USDT profit in 30 mins?"): ten trades at $20, each +50%, each +$10, total +$100 a day, "30 days = 100 × 30 = 3,000 USDT (~RM 12,000+) per month".

- It does not compound. The stake is fixed at $20 and the profits are swept out (step 6). It is linear: 10 × $10.
- It assumes ten wins out of ten, every day, thirty days a month. No losing trade appears in the table and no stop loss appears in the eight steps. **Confirmed from the session: SSWB is traded with a stop loss and isolated margin.** The stop is the Module 5 §3.2 ROI tier; the slide simply omits it.
- With a stop, the expectancy is easy to state. At the beginner tier (20% ROI stop = $4 loss) against a $10 win, breakeven is a 29% win rate. At a 50% ROI stop ($10 loss), breakeven is 50%. The course does not say which stop the SOP uses, and step 4 names only the TP. On cross margin without a stop, the loss is whatever the wallet allows.
- The "30 mins" in the title and the "30 minutes to 1 hour or more" in step 5 do not fit ten trades into 30 minutes. Ten trades at 30 to 60 minutes each is a five to ten hour session.

**The "Execute 10 trades" screenshot contradicts the SOP.** Two Bybit position screens, same account, moments apart:

| Position | Mode | Unrealised P&L | ROI | Implied margin |
|----------|------|---------------|-----|----------------|
| LUNA2USDT long | Cross 20× | +20.79 | 105% | $19.8 |
| YFIUSDT short | Cross 20× | +70.99 | 718% | $9.9 |
| 1000BONKUSDT long | Cross 20× | +40.16 | 203% | $19.8 |
| SEIUSDT long | Cross 50× | +64.68 | 332% | $19.5 |
| GODSUSDT long | Cross 20× | +11.71 | 395% | $3.0 |
| 1000000VINUUSDT long | Cross 12.5× | +2.93 | 15% | $20.0 |

The implied margins confirm the $20 stake (step 1 is real). But:

- Six positions are open **simultaneously**, all on **cross margin**, at 12.5× to 50×. Section 3.2 of this module says cross margin liquidation takes the whole wallet. The liquidation prices shown (LUNA2 at 0.3286 against an entry of 0.7476, 56% away) confirm the wallet is backing all six.
- Five of the six are at 105% to 718% ROI. A Wick Tracker set at 50% would have closed them long before. Either it was not set, or it was set far above the SOP's number. YFI at 718% ROI on 20× is a 36% price move, which is not a 30-minute scalp. Step 8, "don't hold", is not being followed on the slide that illustrates step 7.

So the screenshot demonstrates the stake size and nothing else about the SOP. The positions shown were run as held, cross-margined, uncapped trades.

**Order by Value.** Bybit order placement preferences: Order by Qty (in coin), Order by Cost (margin plus fees, in USDT), Order by Value (notional, in USDT). The slide switches from Cost to **Value** under the heading "Practice with lower risk". With Order by Value you type the notional and the margin is notional ÷ leverage, so $20 of value at 20× is $1 of margin. That is how a beginner practises the SOP with a dollar at risk per trade. The demo account shows 4.69 USDT available.

**Closing slide.** "What will you have when implementing Dose: knowing how much money you are risking; can grow from small capital to big profits."

### 3.13 The three stake sizes the module has now given

| Slide | Stake per trade |
|-------|----------------|
| SSWB SOP and compounding table | $20 |
| "Real example: Start Small Win Big" | $150 |
| CARV short (implied by P&L and ROI) | about $2,500 |
| 1% rule slide | $1,000 (implying a $100,000 wallet) |

None of these are reconciled. The defensible reading is that $20 is the practice stake, $150 is the "graduated" stake, and the larger positions are the author's own. Whatever the stake, the rule that survives all the slides is the same: isolated margin, a stop, and sweep profits out.

## 4. Advance tool: MMT Hedging (Discharge)

Title slide: **"How to salvage your trade with horrible position?"** That framing matters. Hedging is introduced as what you do *instead of* taking the stop, once a position is already badly underwater.

### 4.1 Hedging, as defined on the slide

Generic definition, condensed: hedging reduces or offsets risk by taking opposite positions; investors can hold long and short simultaneously to protect against price fluctuations; common forms are futures, options and derivative hedging (a stock investor buying index futures against a downturn); hedging does not eliminate risk but reduces portfolio volatility and potential losses.

### 4.2 "When the trade goes wrong, you still have a plan"

Diagram, two panels:

1. You are **long** (you want price up). Price goes down. Your long is in loss.
2. You keep the long **and open a short** to hedge it.

Bottom line: **Loss (long) + Profit (short) = Break Even (0)**, drawn as a balanced scale.

### 4.3 The MMT hedging formula

Slide text, verbatim:

- When setting a trade with a Cross position, don't maximise the leverage. Set lower or moderate leverage first.
- **If you lose the trade < 50%**, hedge by opening a counter trade with **extra 50% of your initial capital amount**.
- **If you lose the trade > 50%**, hedge by opening a counter trade with **extra 100% of your initial capital amount**.
- "Remember that both of above condition followed by **increasing the leverage X level to maximal level** to counter hedging higher to compensate your loss."

"Lose the trade < 50%" is ROI on margin, consistent with the rest of the module. The "initial capital amount" is the margin on the original position.

### 4.4 What the formula actually does: the arithmetic

Take the SOP numbers. Original position: long, margin **$20**, leverage **20×**, notional **$400**. Price falls 2%: ROI −40% (loss $8). That is the "< 50%" case.

**Prescribed hedge:** extra 50% of capital = **$10** of margin, at maximum leverage. Bybit maximum on most alts is 50× to 100×. Take 50×.

| | Long (original) | Short (hedge) |
|-|-----------------|---------------|
| Margin | $20 | $10 |
| Leverage | 20× | 50× |
| Notional | $400 | **$500** |

The short is **larger than the long**. The combined book is net short $100 of notional. That is not a hedge. It is a reversal into a net short, with the losing long still open underneath it.

**A true hedge** would match notional: $400 short. At 50× that needs $8 of margin, not $10; at 100× it needs $4. The formula's "extra 50%" plus "maximal leverage" over-hedges at every realistic leverage. The "> 50%" case is worse: extra 100% of capital ($20) at 50× is a $1,000 short against a $400 long, a net short of $600, six times the size of the position being "protected".

**What happens next, for the matched case (the slide's diagram):** the book is flat. Every further move in price adds to one leg what it takes from the other. The $8 loss is now **frozen**, and you are paying two sets of fees and two funding rates to keep it frozen. "Break even (0)" on the diagram means *no further change*, not recovery. A frozen loss is exactly what a stop loss gives you, minus the extra fees and the open exposure to a liquidation on either leg.

**What happens next, for the over-hedged case (the slide's formula):** you now have a directional short bet. If price keeps falling, the short earns more than the long loses and you "compensate your loss", which is the slide's intent. If price bounces 1%, the 50× short loses 50% of its margin, and at 2% it is liquidated. On cross margin that liquidation comes out of the wallet, with the original losing long still open. The formula's instruction to add max leverage is the instruction to turn a losing trade into a second, larger, faster-losing trade in the opposite direction.

**Summary table for the $20 example, price then moves ±2% after the hedge:**

| Scenario | No hedge, stop taken at −40% | Matched hedge ($8 at 50×) | MMT formula ($10 at 50×) |
|----------|-----------------------------|--------------------------|-------------------------|
| Price falls a further 2% | −$8 (already closed) | −$8 frozen, plus fees | Long −$16 total, short +$10: net −$6, plus fees |
| Price rises 2% | −$8 (already closed) | −$8 frozen, plus fees | Long −$0 total, short −$10 (liquidated): net −$10, plus fees |

The MMT formula only beats the plain stop if price continues in the direction that was already hurting you, and even then by a small margin after double fees. If it reverses, it loses more than the stop would have. Across both branches it is worse than the stop.

### 4.5 Three further problems

- **Bybit position mode.** On a one-way (default) account, opening a short on the same contract does not create a second position; it reduces or flips the long. Hedging as drawn requires **hedge mode** to be enabled in Bybit's position settings, and the slides do not mention it. A student following the slide on a default account would close their long at the low, which is the stop they were trying to avoid, at a worse price.
- **Cross margin is required and endorsed.** The formula opens with "when setting a trade with Cross position". Section 3.2 of this same module said cross liquidation takes the whole wallet and prescribed isolated. The hedging tool is only usable on the margin mode the risk tool prohibits.
- **It answers the Module 1 question the wrong way.** Module 1 asked whether hedging replaces the stop. The title slide ("salvage your trade with horrible position") and the formula ("compensate your loss") say yes: the course's plan for a trade that has gone against you is to add exposure, not to take the structural stop from the Discharge rule. Nothing in this section says "take the stop first".

### 4.6 The car-safety analogy

"Trading is like a car safety system. Poor protection will destroy you."

| Go-kart crash without backup protection | Military tank with full protection |
|----------------------------------------|-----------------------------------|
| Seatbelt without roof. One crash ends like liquidation. | Bulletproof, multi-layer protection. Survives multiple crashes. |

The analogy casts hedging as the tank. On the arithmetic above, a matched hedge is a seatbelt that costs double fees, and the MMT over-hedge at maximum leverage on cross margin is the go-kart.

### 4.7 What to do instead

The tools already in this module cover the "horrible position" case without adding exposure:

1. The structural stop from Module 1, at the ROI tier from section 3.2, placed before entry. A horrible position is one where this was skipped.
2. If the stop was skipped and the position is underwater: close it. The loss is the loss. This is the "Discharge plan written before entry" from Module 1.
3. If you want the directional short the formula is really describing, close the long first and open the short as a new, sized trade with its own stop. That is the same net exposure with one set of fees and no wallet-backed liquidation risk on a stale leg.


### 4.8 The GMX case study, labelled "Hedging"

Four slides of the author's own trade, in the first person. Slide text, condensed: bought GMXUSDT long on 16/3/23; paper loss up to −180 USDT; "did not close it as I want to recoup my loss"; held through the volatility until the next morning; waited for the morning pump; "saved my loss and managed to close it without paying any single loss."

The screenshots:

| Time (17/3/23) | Mark price | Position P&L | Notes |
|----------------|-----------|--------------|-------|
| about 08:00 | 75.665 | −87.83 (−30.61%) | Entry 78.015, size 37.78 GMX, **Cross 15×**, liquidation 51.47. 24h low 74.55. |
| about 09:30 | 77.280 | −27.95 (−12.37%) | Two other positions open: NEO long cross 10× (+4.25), ARPA long cross 12.5× (+12.20). |
| 09:30 candle | 77.585, high 78.370 | closed near 0 | "The hair / wick touched back my entry price, then I totally saved my loss!! Phew..." |

Arithmetic: 37.78 GMX × 78.015 is about 2,950 USDT of notional. The −180 USDT maximum loss is 4.76 per GMX, so price reached about 73.25 at the worst point, 6.1% below entry. Liquidation at 51.47 is 34% below entry, which on 15× means the wallet was backing the position. The chart runs the 2023 indicator set (EMA 10, 25, 50; MACD 12, 26, 9), same as the seahorse slide.

**There is no hedge in this case study.** No short was opened at any point. The "hedging method" as actually practised in the example is: hold the losing long on cross margin, do not take the stop, and wait for a wick to touch the entry price. The trade lasted about a day.

**Why the outcome is not evidence for the method:**

- Closing at entry caps the upside of the wait at zero. The downside was uncapped down to a liquidation at −34% with the wallet behind it. That is a bet with a maximum payoff of "no loss" and a maximum cost of the account.
- The exit was on a **wick** to 78.37 on one 15-minute candle. The candle closed at 77.585, below entry. Had the order been a few cents higher, or placed a candle later, the trade would still have been open and underwater.
- GMX in March 2023 recovered. The same hold on a coin that did not recover is the seahorse slide's "painful loss", and the course's own risk section says cross margin ends in "Burst!!". One recovered trade out of an unknown number of holds is a survivor, not a rule.
- The behaviour has a name in the trading literature, the disposition effect: holding losers to avoid realising the loss and selling winners early to lock the gain. The ZETA slide in section 2.3 criticised the second half of that pattern. This slide endorses the first half.

### 4.9 "Lesson of my sharing"

Five lessons, verbatim:

1. "Please set SL (Stop Loss) even though the market is happy in your way of position."
2. "Never give up to retrieve your loss → gain. So, don't let your frustration close the position so early just to save your headache."
3. "Limit or do now new position of the day and look for the potential 'market call' to standby and retrieve your loss by closing it when reaching back your initial entry price."
4. "Hold your breath and manage your EQ and be patient to the next market come."
5. "At last, DON'T BE TOO GREEDY!! You may be a little bit greedy if you are ready in front of your screen to close up the position any time it reaches your desired closing price/profit."

Lesson 1 says set a stop. Lessons 2, 3 and 4 describe what to do after not honouring one: hold, wait for the entry price, manage the discomfort. A trade with a stop set never reaches the situation lessons 2 to 4 are for. The slide is telling students to set a stop and then not to let it work.

Lesson 3 also says to limit new positions while a loser is open, which is sound, and the screenshot shows two other cross-margin longs open at the same time as the GMX loser.

Lesson 5, read closely, says be ready to close at the desired price. Combined with lesson 3, the "desired price" for a losing trade is the entry price. That is the whole method: breakeven as the target for losers.

### 4.10 What the hedging section amounts to (before the PEOPLE example)

Two things were taught under the heading "MMT Hedging" up to this point:

| | Formula (section 4.3) | Case study (section 4.8) |
|-|----------------------|-------------------------|
| What it is | Open an over-sized counter position at maximum leverage on cross margin | Hold the loser on cross margin until price returns to entry |
| Stop loss | Not taken | Not taken |
| Downside | Liquidation of either leg from the wallet | Liquidation of the position from the wallet |
| Upside | Small net gain if the adverse move continues | Zero (close at entry) |
| Evidence | None shown | One trade that recovered |

Neither is a hedge in the sense the definition slide gives. Both are ways of not taking the stop. The PEOPLE example in section 4.11 is the one actual hedge in the module, and it is analysed there.


### 4.11 The PEOPLE example: the one real hedge, and how it ends

Framing slide first: "When the market moves against me there is nothing I can do except watch it bleed. What if the trade goes wrong?" Answer: "There is always something you can do. You just have to know it before you enter. **Discharge is not just your exit (TP/SL). It is your safety plan for every scenario, written before any of them happen.**"

Then "Real example: Hedging Losing Trade. Manage your loss with strategy to stay profitable."

| Leg | Side | Size | Entry | Mark | P&L | Mode |
|-----|------|------|-------|------|-----|------|
| Losing trade | Long | 9,600 PEOPLE | 0.04450 | 0.03106 | −128.92 (−374.87%) | Cross 12.5×, liquidation "--" |
| Hedging entry | Short | 19,205 PEOPLE | 0.03850 | 0.03106 | +142.69 (+135.42%) | Cross 12.5×, liquidation 0.08863 |
| After "Close losing trade, let the runner win" | Short only | 19,205 | 0.03850 | 0.02751 | +209.71 (+351.93%) | Liquidation now 0.06118 |

Checks: (0.03106 − 0.04450) × 9,600 = −129.0. (0.03850 − 0.03106) × 19,205 = +142.9. (0.03850 − 0.02751) × 19,205 = +211.1. All match the cards.

What the numbers say:

- **The hedge was opened late.** Entry 0.0445, hedge at 0.0385: the long was already down 13.5% on price, which at 12.5× is −169% ROI. The position had lost 1.7 times its margin before anything was done. That is only survivable on cross, where the wallet absorbs it; the "--" liquidation price confirms the wallet was large relative to the position.
- **The hedge was 2:1, not 1:1.** 19,205 short against 9,600 long. That is the formula's "> 50% loss, extra 100% of capital" case in action: a net short of 9,605 PEOPLE, with the losing long still open underneath.
- **The resolution was to close the loser.** "Close losing trade, let the runner win." The long was closed at about 0.0311 for −129. The short ran on to +210. Net about **+81 USDT** across both legs. Note the short's liquidation price moved from 0.0886 to 0.0612 once the long was gone: the long had been propping it up as offsetting exposure. After closing the loser, the short is a plain 12.5× position with 122% headroom.

**The comparison the slide does not make.** Suppose the long had a stop at −20% ROI, the beginner tier from section 3.2. It closes at about 0.0438 for a loss of roughly −7 USDT. The short is then opened at 0.0385 as a fresh trade, same size, and runs to 0.0275 for +210. Net about **+203 USDT**. The hedge path made +81 because the long bled from −7 to −129 while waiting for the hedge, and then the hedge's first 13 points of profit only paid for that bleeding.

| Path | Long result | Short result | Net |
|------|-------------|--------------|-----|
| MMT hedge as shown | −129 | +210 | +81 |
| Stop at −20% ROI, then the same short | about −7 | +210 | about +203 |
| Stop at −20% ROI, no short | about −7 | 0 | about −7 |

And if PEOPLE had bounced after the hedge instead of falling: the 2:1 short loses twice as fast as the long recovers, on cross margin, with both legs paying funding.

So the example is honest in one respect that the formula slide was not: it ends with the loser closed. The "hedge" functioned as a delayed stop plus a new short. The same outcome is available with a stop and a short, for 122 USDT more, with no period where both legs are open on cross margin.

### 4.12 "What will you have when implementing Discharge"

Four bullets: partial TP / breakeven plan; hedging when suitable; exit discipline; how to protect your trade when the market moves fast.

"Hedging when suitable" is the only qualifier the module puts on hedging. **Confirmed from the session: "suitable" means one case only, a trade accidentally opened in cross mode.** On an isolated position with a stop, hedging is never the tool. For the accidental-cross case the hedge freezes exposure while you fix the mistake; the fix is to close the position, or to switch it to isolated where Bybit allows it (no pending orders on the symbol), and then the hedge leg is closed too. It is damage control for an execution error, not a strategy.

## 5. MMT Golden Rules (Follow up)

Twelve rules across two slides, transcribed with light cleanup:

| # | Rule | Reading |
|---|------|---------|
| 1 | If the market is too volatile with a sideways trend but high volume, do not trade this kind of coin or hold too long. | The seahorse and heatmap "ranging" Skip condition, restated. |
| 2 | How to earn from a trade is not just ROI%. Consider the funding rate (FR); expected profit and actual profit at close differ slightly. | Correct. Funding is charged every 8 hours on Bybit and shows up as the gap between the TP/SL screen's "expected profit" and the realised figure. It only matters if you hold across a funding time, which rule 6 says not to do. |
| 3 | "Close and Go", then "Open and Wait" for the next potential coin. | Take the profit, leave the coin, scan again. This is the SSWB loop. |
| 4 | New-born coins: trade for a few days only, avoid keeping them long. | New listings pump then fade; there is no EMA 155 history to lean on. |
| 5 | Frequent long and short scalping earns faster, for those who can monitor. | Both directions, high frequency, screen time required. |
| 6 | **Do not hold the coin too long. We are not doing swing trades.** Observe the volume percentage. | The rule the showcase trades break: ZETA (two weeks), BMT (five days), GMX (overnight on a loser). |
| 7 | **Bigger wallet → smaller trade → lasts longer. Smaller wallet → bigger trade → will not last.** | The one sizing principle in the course stated as a rule. It is correct and it is the argument against cross margin, which makes every trade wallet-sized. |
| 8 | PTP (partial take profit) and SL to entry, versus awaiting TP; Hunting SL. | Section 3.3. Take some, move the stop to breakeven, trail the rest. |
| 9 | Know the trend of a new-born coin. | Pairs with rule 4. Not elaborated. |
| 10 | We can make money with small capital and flipping our own wallet. | SSWB restated. |
| 11 | Let's become a "Wick Player". How to be a "Wick Catcher" without a Master? | A teaser for the Module 4 Wick Tracker. |
| 12 | **10% is the strategy, 90% is the mindset.** | See below. |

### 5.1 What the Golden Rules do and do not say

- **No rule says "always set a stop loss."** Rule 8 mentions moving a stop to entry after a partial take-profit, which presumes one exists, and the GMX lessons slide said "please set SL". But the twelve rules that the course labels golden do not include it. Given that the hedging section is entirely about what to do instead of a stop, that omission is consistent with how the course actually trades, and it is the first thing to add to your own copy of the list.
- **Rules 6 and 7 are the two that matter most, and the course's own examples break both.** Do not hold, and size small relative to the wallet. Every showcase trade in this module held for days on cross margin.
- **Rule 12 is the escape hatch.** "90% is the mindset" means that when the method fails, the diagnosis is the student's psychology, not the method. It is unfalsifiable. A method that is 10% strategy should be easy to state in full, and this module has shown that the strategy part (isolated, 5× to 10×, ROI-tiered stop, TP first, sweep profits) is sound and short, while the parts labelled "advanced" (cross margin, hedging, holding to breakeven) are where the risk lives.

## 6. Module 5 summary: what to keep and what to discard

**Keep** (all stated somewhere in this module by the course itself):

1. Isolated margin, 5× to 10×.
2. Small fixed stake: $20 to practise, scale by percentage of wallet later.
3. Stop set before entry, by ROI tier converted to price, at or beyond the structural level.
4. TP set first. Partial TP, then stop to entry, then Hunting SL.
5. Sweep realised profit to the Funding account.
6. Close and go. Do not hold. Stop at the day's target and rest.
7. Bigger wallet, smaller trade.

**Discard** (also stated in this module, and contradicted by the list above):

1. Cross margin as a working mode.
2. The hedging formula (over-sized counter trade at maximum leverage).
3. Holding a losing position to breakeven (GMX).
4. Opening a hedge instead of taking the stop (PEOPLE), when the same short as a fresh trade after the stop nets more. Session: hedging is only for a position accidentally opened on cross.
5. The "90% mindset" framing as an explanation for losses.


## Open questions

- Is the "1% to 10% amount" margin per trade or maximum loss per trade? The isolated-margin framing in section 3 points to margin. Confirm.
- The demo account trades at 25× while the slide prescribes 5× to 10×. Which is the course's actual recommendation?
- Was the THETA demo position isolated or cross? Its liquidation distance (8.4%) does not match isolated 25×.
- ~~What does SSWB stand for?~~ Start Small Win Big.
- Which stake is the taught one: $20 (SOP), $150 (real example), or a percentage of wallet (1% rule)? See section 3.13.
- Does the SSWB SOP use a stop loss, and at what ROI? Step 4 names only the Wick Tracker take-profit.
- Why does the "Execute 10 trades" screenshot show six simultaneous cross-margin positions at 100% to 700% ROI when the SOP says 50% TP, one at a time, don't hold?
- Over what period did the 1,993 to 18,288 USDT growth happen, and how many losing trades were in it?
- The "IceBerg Tip" on the MACD is most likely the histogram extreme, the same signal Module 4 uses in reverse for take-profit ("mid histogram"). Is the crash-bottom entry in the RAVE example a taught setup or a one-off?
- ~~Does Module 4 replace the Module 1 exit rule?~~ Yes. Module 4 takes 75% at the volume/MACD climax and protects a 25% runner. That is a coherent answer to the ZETA "too early" slide without holding everything.
- What does "hedging when suitable" mean? "Suitable" is never defined.
- ~~Is hedging a replacement for the stop loss?~~ Answered: yes. The hedging section is framed as salvaging a position already deep in loss, and never says to take the stop. See section 4.4 for why the formula is worse than the stop in both branches.
- Does the course tell students to enable Bybit hedge mode? Without it the hedge as drawn cannot exist. The GMX case study never opened a short, so the question may be moot in practice.
- How many losing positions has the author held to breakeven that did not recover? The GMX case is one that did.
- ~~What are the Golden Rules?~~ Captured in section 5. They do not contain a stop-loss rule.
