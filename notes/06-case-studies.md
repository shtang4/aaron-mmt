# 06 — Case Studies & Q&A

Dr. Aaron teaches by worked example throughout the two days, not only in the module labelled Case Study. This file is the index of **every** case study in the course, wherever it was taught, plus the Q&A. Module 6's own slides are sections 5 to 10; the examples he ran live while teaching coin selection and the screener are sections 2 to 4.

Several Module 6 slides carry the "Future Trends FZCO" copyright line rather than "Dr. Aaron MMT".

## 1. Index of every case study in the course

| Coin | Taught in | What it demonstrates | Outcome shown | Full write-up |
|------|-----------|---------------------|---------------|---------------|
| **SOMI** | Module 2, the Bybit scan | How to pick the candidate: top of the heatmap, top of the 24h gainers | None. Candidate only | §2 below |
| **BTCUSDT** | Module 2, the screener | The four checks walked end to end; majority-vote timeframes | None. Screen reading only | §3 below |
| **10000LADYSUSDT** | Module 2, the screener | A complete 4/4 long, with the depth rule stated aloud | None. Setup only | §4 below |
| **MAVIAUSDT** | Trade-call case study | The same call taken 34 hours apart; both directions traded on the chop | Cards from +74% to +2,814% ROI | §5 below |
| **RADUSDT** | Module 6 slides | Multi-timeframe EMA alignment, all five lines, four frames | None. Screen reading only | §5 below |
| ZETAUSDT | Modules 3 and 5 | SPE entry at an EMA; then "took profit too early" | Entry 0.8570, exit 2.8530, about +233% | [03 §2.3](03-entry-direction.md), [05 §2.3](05-risk-and-hedging.md) |
| RAVEUSDT | Module 5 | Heel / crash-bottom entry on a liquidation cluster | +277% ROI on a $150-style stake | [05 §3.9](05-risk-and-hedging.md) |
| BMTUSDT | Module 5 | A chat trade call; "late trade is a losing trade" | +3,736% ROI at cross 15× | [05 §3.10](05-risk-and-hedging.md) |
| GMXUSDT | Module 5 | Held a loser to breakeven, taught as "hedging" | Closed at entry on a wick, zero | [05 §4.8](05-risk-and-hedging.md) |
| PEOPLEUSDT | Module 5 | An actual hedge, resolved by closing the loser | Net about +81 USDT | [05 §4.11](05-risk-and-hedging.md) |
| CARVUSDT, RARE, REEF and others | Module 5 SSWB | Result cards, no method shown | Various, wins only | [05 §3.10](05-risk-and-hedging.md) |
| AERGOUSDT ("Kpnd") | Module 6 | Uncorrelated pump during a BTC crash | Entry 0.078, +657% ROI at 10× | §9 below |
| Skipped-D triptych | Module 6 | Schematic failures, one per D | Schematic | §7 below |

**What every one of them has in common:** not one shows a stop loss placed before entry, a partial take-profit, or a losing trade. The three live screener walks (SOMI, BTC, 10000LADYS) stop at "setup", and the result cards start at "outcome". The middle, which is execution and the part he says decides everything, is never shown end to end. That gap is what the trade journal is for.

## 2. SOMI: how the candidate is chosen

Taught inside the Bybit scan (see [02 §4.4](02-coin-selection.md) for the screen-by-screen mechanics).

| Screen | What SOMI showed |
|--------|-----------------|
| Heatmap | **+46.56%**, the largest tile by a wide margin |
| Top Movers → View all → 24h gainers | **+47.39%**, top of the list; next best were CORN +16.29% and DRIFT +20.76% |

His rule, spoken: **"Choose the highest one. If you have no idea, choose the highest one; if not, then the second, the third accordingly."**

What this case actually teaches:

- The scan is a **ranking**, not a shortlist. You take the top of the ranking and then qualify it.
- A top gainer is "a potential coin to further analyse", never a trade. Nothing about the scan tells you direction, entry or size.
- The danger it creates is obvious and unaddressed on the slide: you are being pointed at a coin that has already moved 47% today. Every protection against buying that top is downstream, in the EMA 155 rule, the SPE pullback and the stop.

The slide then shows a BTCC share card for SOMI, Open Long Perp 50×, **+554.50%**, average open 0.9901, latest 1.0999. The price move is +11.1%; the rest is leverage. It is a different exchange's promotional card with a referral code on it, not a demonstration of the method.

## 3. BTCUSDT: the screener walked end to end

The first full run of the four checks, spoken (see [08 part 4](08-transcript.md)).

| Check | Reading | Score |
|-------|---------|-------|
| EMA, six timeframes | 1D up · **4H down** · 1H up · 15m up · 5m up · 1m up | **Up** |
| OI | Line tilting up at the right-hand end of the 5m chart | Up |
| Funding | **−0.0021% in 8 hours**, negative, counter to a long | Long |
| Depth | Bids 323,220 against asks 364,732; green lower than red | **Up** |

Two rules come out of this one case and nothing else in the course states them as clearly:

1. **The EMA check is a majority vote.** The 4-hour dissented and the check still scored Up. Unanimity is not required.
2. **Funding scores on the sign, not the size.** −0.0021% is well inside the handouts' "balanced" band, and he counted it as negative and therefore long.

It is also the screenshot that settles the depth direction for the whole course: green lower than red is the long condition, which is the reverse of the handout. See [02 §5.1](02-coin-selection.md).

Context on the screens: Bitcoin at 26,324, +3.19% on the day, initial margin 1.0% and maintenance margin 0.5%. Note those margin figures; they are the Bitcoin ones, and section 4 shows what an alt looks like instead.

## 4. 10000LADYSUSDT: a complete 4/4 long

The second full run, on a meme coin at +25.86% with 228M USDT of 24-hour turnover. That profile is "volatility and volume are the must" in practice.

| Check | Reading | Score |
|-------|---------|-------|
| EMA, six timeframes | 1D up · 4H up · 1H up · 15m up · **5m down** · **1m down** | **Up**, "but majority timeframe showing you up" |
| OI | 5m open interest climbing hard at the right end. "Wow. This one pointing up." | Up |
| Funding | **−0.0214%** in 8 hours (−0.0257% a minute later), negative | Long |
| Depth | "Green lower than red" | Long |

**Verdict, his words: "4 out of 4. Long setup."**

Three things worth carrying away:

- **The majority rule is stated outright here**, and this time two frames dissent, not one. The two that dissent are the 5m and the 1m, the frames he himself calls the noisiest.
- **A 4/4 long can coexist with a falling 1-minute chart.** That is not a contradiction; it is the exact situation SPE exists for. You rest a limit at EMA 9 and let the short-term dip come to you. Market-buying a 4/4 means buying into the dip the screener just told you to ignore.
- **Its Contract tab reads initial margin 4.0%, maintenance margin 2.0%**, against Bitcoin's 1.0% and 0.5%. Maintenance margin sets the liquidation price, so liquidation on this coin sits much closer to entry than on BTC at the same leverage, and the 4% initial margin caps leverage at 25×. The course never mentions this, and the pre-trade checklist had it hard-coded at 0.5% until this case exposed it.

## 5. MAVIA: the same call, 34 hours apart

Three slides, titled "Trade Call - Case Study", with three subheadings that are the lesson: **"If you don't know the setup, don't take the shot"**, **"Timing and reason matter, without them it's not trading, it's guessing"**, and **"Late trade is a lost trade, don't chase if you don't understand."**

### 5.1 The timeline

| When | What |
|------|------|
| **17/03/2025 13:22** | Aaron posts the MAVIA chart in `#mmt-announcement`. Price around 0.28 to 0.30. |
| 17/03 15:00 | A member posts a MEXC card, long 20×, **+1,033.15%**, entry 0.2865 |
| 18/03 13:30 | Second post: "I told u $MAVIA will PUMP!!" Price 0.5709 |
| 18/03 19:34 | A member: "short crazy pump" |
| **18/03/2025 23:13** | The contrast the slide draws. By now price has run to the 0.6 area. |

The slide puts the two timestamps side by side: **17/3 13:22 versus 18/3 23:13.** Same coin, same call, thirty-four hours apart, and the slide's point is that they are not the same trade at all.

### 5.2 The member who got caught

> **Joyce Ng, 18/03 23:12:** "Omg mavia very hard to handle. It was going down nicely but suddenly gap up to 0.6xxx level."
>
> **Yuki, 18/03 23:13, replying:** "Yes it's super manipulative so I always set higher price. Can refer to previous high or set even higher."

Yuki's reply is a **take-profit placement rule from a member, endorsed by being put on a slide**: on a manipulative coin, set the target at or above the previous high rather than at a modest level. That is the Wick Tracker idea arriving from the community side, and it is the same level the Module 4 notes list first ("a prior swing high's wick"). Read it with care, though: "set even higher" is also how a target stops being reached at all, and nothing here caps how far above.

A third member, Nica9, adds "I think Dr recently no lost streak, correct me if I'm wrong." Unverified social proof, and worth naming as such.

### 5.3 What he says about it

- He drew the structure first: **"Actually ranging, then break out. And then ranging, ranging, ranging, and break out."** The setup was a range break, twice.
- **On shorting the pump:** "You can short, but prematurely you will always get liquidated or get stop loss. **No one can tell where the pump will get.**"
- **On why:** "You can't really differentiate nicely whether it's a retracement or pivotal change. Very super duper manipulative."
- **On timing:** "You enter from here, sniper price entry, pump, start earning, came down, pump. Some of our elites started here, because she managed to interpret a decent retracement and pump, so earn higher and better. **Timing and the reason matter. Without them, it's not trading, it's just wild guessing.**"
- **On chasing:** "Late trade is a loss trade sometimes. Don't chase, but it's really for beginners. Unless you are intermediate or advanced, don't chase if you don't understand."

### 5.4 The four-leg sequence

The last slide is a **15-minute Heikin-Ashi** chart with four numbered legs, all traded by one member he calls Jane:

| Leg | Direction | Card shown |
|-----|-----------|-----------|
| 1 | Long | +414.89% at 25×, entry 0.4050 → 0.4720 |
| 2 | Short | +325.27% at 25×, entry 0.4107 → 0.3569 |
| 3 | Long | +74.19% at 25×, entry 0.4323 → 0.4448 |
| 4 | Short | +193.94% at 25×, entry 0.4181 → 0.3855 |

His comment: "Earning both sides. Up, down, up, down. **Even the ranging one, by doing scalping, you can earn very nice amount. The matter is just you know the trick.**"

Other cards on these slides: +2,814.38% (entry 0.2978 → 0.6374, 25×), Wendy at +698.68% (0.2963 → 0.3998, a realised exit), +300.26% (0.5379 → 0.6208).

### 5.5 What to take, and what to discount

**Take:**

- This is the clearest demonstration in the course of the opening claim that the difference is execution, not the signal. One call, two entry times, opposite experiences, and the slide shows both.
- **Do not short a running pump.** "No one can tell where the pump will get" is the correct instinct and it is the same reason the seahorse rule exists.
- **The range-then-breakout read** is the structure he actually traded, and it is more concrete than anything in the trend-line section.
- Yuki's target rule, with a cap of your own: prior high as the Wick Tracker level on a manipulative coin.

**Discount:**

- Every card is a win, including all four of Jane's legs. A member who traded four legs across a chop and won all four is either very good or is showing you four of more than four. The deck has now shown well over twenty result cards and not one loss.
- The four legs are read on a **15-minute** chart, not the 1-minute execution chart, and each leg spans hours. That is inside the "minutes to hours, under 24 hours" rule, but it is not the 1-minute scalp the method describes.
- 25× on MAVIA, and the MEXC card at 20× on a third exchange. The risk module prescribes 5× to 10× isolated.
- The chart's full arc: MAVIA ran from about 0.11 to 0.75 and then fell all the way back to 0.21 over the following week. Everyone whose card is on these slides was trading the left half. Nothing shows what the right half did to anyone.

## 6. RAD: the multi-timeframe check, done on the Bybit app

Four Bybit screenshots of RADUSDT side by side (+22% on the day, last price about 2.10, 24h range 1.705 to 2.115), one per timeframe, each with the five EMAs, MACD (8, 13, 9) and Volume (MA5, MA10) visible. Two of the four have the **OI Data** tab selected and one the **Contract** (funding) tab. This is Module 2's Coin Trend Screener, check 1 (EMA on every timeframe) with checks 2 and 3 (open interest, funding) being read on the same screen.

EMA values read off the four headers:

| Timeframe | EMA 9 | EMA 25 | EMA 55 | EMA 155 | EMA 255 | Price vs EMAs |
|-----------|-------|--------|--------|---------|---------|---------------|
| 1D | 1.796 | 1.762 | 1.697 | 1.568 | 1.732 | Above all five |
| 4h | 1.812 | 1.753 | 1.737 | 1.736 | 1.706 | Above all five, fully fanned |
| 1h | 1.878 | 1.801 | 1.766 | 1.729 | 1.732 | Above all five |
| 15m | 2.009 | 1.897 | 1.827 | 1.776 | 1.756 | Above all five, fully fanned |

Price is above every EMA on every timeframe, and on 4h and 15m the lines are stacked in the bullish order (9 over 25 over 55 over 155 over 255). Check 1 passes for a long. This is the cleanest worked example of the screener in the deck.

What the same screenshots also show:

- The 15-minute chart has a near-vertical spike from about 1.49 to 2.115 in a few candles, at roughly 11:30, and the screenshot is taken at 04:43 the next day with price flat at 2.11. The alignment is perfect *because* the spike just happened. A long taken here is a long after a +40% move, into what the seahorse slide (Module 3 section 6) calls the beak. The screener says the trend is up; the seahorse rule says wait for the pullback. Both are right, and SPE (Module 4) is how they are reconciled: the entry is a limit order at an EMA below current price, not a market buy at 2.11.
- The four screenshots have different timestamps (20:20, 04:43, 19:55, 19:49). They were assembled, not taken at one moment.

## 7. "What happens if you skipped one D?"

Three slides, one per D. Each has a schematic chart with **EMA 50 and EMA 5** (the generic pair from the shared deck, not the MMT five) and a medical one-liner.

### 7.1 Skip Diagnose: "What the chart was saying"

"The signal came in. You entered. No chart check."

- EMA 50 was pointing down. The chart was in decline before you entered.
- The death cross had already formed. The diagnostic line said stay out.
- You blamed the signal. **The signal was not wrong. The timing was.**

"A doctor who prescribes without diagnosing does not blame the medicine when the patient gets worse."

The chart: a downtrend, death cross marked, entry marked several candles *after* the cross, price continuing down. The failure is entering long on a "signal" (a trade call, a chat message) without reading direction from the chart. The fix is Module 3: EMA 155 three-candle rule, Heikin-Ashi run, Donchian alignment, all before any entry.

### 7.2 Skip Dose: "Right trade. Wrong size. Could not hold."

"EMA confirmed. Entry valid. But you went in too heavy."

- The trade dipped 3%, a normal pullback. But it felt like a disaster. You panicked and cut.
- After you exited, the trade ran exactly where you thought it would. Without you.

"A doctor who prescribes 10× the correct dose does not get 10× the result."

The chart: uptrend above EMA 50, valid entry, a three-candle red dip, "panic cut" at the dip low, then the run resumes. This is the ZETA slide from Module 5 section 2.3 in schematic form. The fix is Module 5 section 3.6: stake small enough that a 3% pullback at your leverage is a tolerable ROI swing. At 20× a 3% dip is −60% ROI; at 5× it is −15%. The "felt like a disaster" is a leverage choice, not a personality flaw.

### 7.3 Skip Discharge: "Won the trade. No exit plan. Gave it all back."

"Perfect entry. Correct dose. No exit plan."

- The trade went green. RM200. RM400. RM600. You thought, let it run a little more.
- It reversed. Fast. No take profit was set. **You gave back everything.**
- **The EMA exit signal fired during the reversal.** You had no discharge condition, so you held and hoped.

"A doctor who admits a patient but never writes the discharge plan keeps them in the hospital indefinitely."

The chart: uptrend, entry, "profit window" at the top with "TP (never set)" as a dashed line, then reversal through EMA 50, "closed at loss" at the bottom. Two things to notice:

- The slide names the **EMA exit signal** as the discharge condition that fired and was ignored. So the Module 1 cross-back rule is still part of the plan in this deck, as the backstop. Module 4's climax exit (volume maximal, MACD peak, PTP 75%) would have fired earlier, at the "profit window", and is the primary.
- "Held and hoped" is the exact behaviour the GMX hedging case study in Module 5 section 4.8 presented as the method. This slide calls it skipping Discharge.

## 8. The three failures, mapped to the course's own examples

| Skipped D | Failure slide | Course example that did the same thing | Where |
|-----------|--------------|----------------------------------------|-------|
| Diagnose | Entered on a signal, no chart check | The 18/3 BMT entry from a "it's pumping!" chat message, "late trade is a losing trade" | Module 5, section 3.10 |
| Dose | Right trade, too heavy, panic cut | ZETA "took profit too early" | Module 5, section 2.3 |
| Discharge | No exit plan, held and hoped | GMX held overnight on cross margin to breakeven; PEOPLE hedged instead of stopped | Module 5, sections 4.8 and 4.11 |

The 3D review slides are the right lens. Applied to the deck's own case studies, they mark most of the "advanced" material in Module 5 as a skipped D.

## 9. Market uncertainty: "Trade scam coin, no BTC correlation"

### 9.1 The strategy slide

"Market Uncertainty. What's the strategy?" Answer on the slide: **"Trade Scam Coin"** with a starburst reading **"No BTC Correlation"**. The backdrop is a Coin Bureau video ("99.99% of crypto will go to zero, what to do now"), Chinese overlay "99.99% 多数是 Shit Coin!", over a CoinMarketCap page showing Fear and Greed at 24 (extreme fear).

The claim: when BTC is falling and the market is fearful, the trade is not BTC or the majors. It is the small coins that move on their own drivers, chiefly exchange-driven pumps, and therefore do not fall with BTC. The course calls them scam coins or shit coins without irony. This is the "shit coin" list from Module 2 section 1.3 in use, with the direction flipped to long.

### 9.2 Case study: "Kpnd", AERGO on Black Monday

"Kpnd" is **Korean pump and dump** (confirmed from the session). AERGO is a Korean project and the shape of the trade is a Korean-exchange pump.

Two TradingView charts, 15-minute Heikin-Ashi, Bybit perpetuals, 6 to 8 April 2025:

| | BTCUSDT | AERGOUSDT |
|-|---------|-----------|
| Move | 83,774 → 74,456 low on 7 April ("7/4 Black Monday", the tariff sell-off), then a bounce to about 80,000 | 0.0665 low → 0.1353 high, roughly doubling over the same two days |
| Trade | none | Long, entry 0.07797, shown on two Bybit cards: **+76.82%** at 0.08402 and **+657.25%** at 0.12940 |
| Chat caption | | "Scalping > 30 mins + MMT #SSWB and PUMP!!" and "There is where we find opportunity when BTC dump!!" |

Checks: 0.07797 → 0.08402 is +7.8% on price, ×10 = 78%, card says 76.82%; 0.07797 → 0.12940 is +66%, ×10 = 660%, card says 657.25%. Both cards are the same 10× position at two moments. The green box on the chart runs from the entry to about 0.1294; a red box beneath it runs from the entry down to about 0.0746, which reads as the stop zone, 4.4% below entry (−44% ROI at 10×). Realised reward-to-risk on those levels: (0.1294 − 0.0780) ÷ (0.0780 − 0.0746) ≈ 15.

What the timestamps say: the first card is from about 09:49 on 7 April and the second from 10:22 on 8 April. The position was held for **over 24 hours**. The chat caption's "> 30 mins" is the course conceding that this was not a scalp. Golden Rule 6, do not hold, was not followed, and the deck labels the trade a success.

### 9.3 What is right and what is dangerous in this idea

**Right:** correlation to BTC is the main risk in an altcoin book during a crash, and coins moving on an idiosyncratic driver (a listing, a regional pump) can decouple for hours or days. The Module 2 sector and heatmap scan is exactly how you find them: when the heatmap is mostly red, the few strong green tiles are the candidates. AERGO was one on 7 April.

**Dangerous:**

- **You are trading someone else's manipulation.** The Module 2 screener slide listed "risk management for manipulation (pump and dump)" as a caveat. This section makes the pump the target. The exit on a pumped coin is a wick, the retrace is violent, and the depth check (screener check 4) is thin by construction. The Wick Tracker (Module 4) exists for exactly this, and it must be resting before you look away.
- **"No BTC correlation" is an observation after the fact.** AERGO decoupled on 7 April. Whether it would decouple on the next BTC leg down was unknown at entry. The course's evidence is one coin on one day.
- **Fear and Greed at 24 is the reverse of the Module 2 rule.** Module 2 said greed is a bias toward long but not a signal. Extreme fear is a bias toward short, or toward staying out. The slide uses extreme fear as the setup for a long, on the logic that the long is in a coin that ignores the index. That is coherent only if the coin really is uncorrelated, which is the point above.
- **The "scam coin" framing has a cost the slides never state.** Delistings, liquidity vanishing overnight, and exchanges halting trading are all outcomes on coins the course itself calls scams. A stop does not protect against a halt.

## 10. Q&A

The deck has no dedicated Q&A section; questions were answered as they came up, and one was promoted onto a slide.

### 10.1 "With 4/4 confirmed short, do we still need MACD before entering?"

Asked by a member (Joe) in the community chat, with a follow-up: which timeframe should we observe before entering? The slide shows the answer from another member, **Jasper Sia**, dated 21 April 2024, and the course endorses it by putting it on a slide:

> 对的，我一般跟着这几个步骤: 1. 4/4  2. volume 是否活跃  3. macd. 配合黄金或死亡交叉更好。我只用这些，其余我都没看，我还是 MMT 1.0

Translated: "Correct, I generally follow these steps: 1. 4/4, 2. is volume active, 3. MACD, better combined with a golden or death cross. I only use these, I don't look at anything else. I'm still on MMT 1.0."

**The answer is no, 4/4 is not enough to enter.** The division of labour it states:

| Step | Job |
|------|-----|
| Screener 4/4 | Qualifies the coin and the direction |
| Volume active | Confirms there is something to scalp |
| MACD, with a golden or death cross | Times the entry |

That is the same structure as the full method (screener → direction → SPE → climax exit) with the SMC, Donchian and liquidation-heatmap layers dropped. It is a legitimate reduced stack, and the fact that a long-standing member runs "MMT 1.0" with three tools is a useful counterweight to the seven-tool chart in Module 3.

The member's question about timeframe was not answered on the slide. From the rest of the course the answer is: direction on the higher frames, entry on the 1-minute.

### 10.2 Everything else

No other questions were captured on slides. Anything else was answered verbally and is only in the transcript ([08](08-transcript.md)).

## 11. Closing slide: "Synchronization"

"Resonance at the SAME frequency, attraction of the SAME nature" (同频共振，同质相吸). A mindset close, matching the "90% mindset" Golden Rule and the Know / Enlighten / Do pyramid from Module 0. No trading content.



## Open questions

- Is trading uncorrelated pumps during a BTC crash a taught setup with rules (which scan, which stop, which exit), or a single observation from 7 April 2025?

- The deck contains no case study showing one trade with all three Ds executed and shown (entry, stop, partial TP, runner). Every case study is either a setup with no outcome, a result card with no method, or a schematic failure. See the note under the index in section 1.
