# 06 — Case Study & Review

Source: Module 6 slides, Momentum Mastery Trading (MMT), Dr. Aaron MMT, 2026. Several slides in this module carry the "Future Trends FZCO" copyright line rather than "Dr. Aaron MMT".

## 1. RAD: the multi-timeframe check, done on the Bybit app

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

## 2. "What happens if you skipped one D?"

Three slides, one per D. Each has a schematic chart with **EMA 50 and EMA 5** (the generic pair from the shared deck, not the MMT five) and a medical one-liner.

### 2.1 Skip Diagnose: "What the chart was saying"

"The signal came in. You entered. No chart check."

- EMA 50 was pointing down. The chart was in decline before you entered.
- The death cross had already formed. The diagnostic line said stay out.
- You blamed the signal. **The signal was not wrong. The timing was.**

"A doctor who prescribes without diagnosing does not blame the medicine when the patient gets worse."

The chart: a downtrend, death cross marked, entry marked several candles *after* the cross, price continuing down. The failure is entering long on a "signal" (a trade call, a chat message) without reading direction from the chart. The fix is Module 3: EMA 155 three-candle rule, Heikin-Ashi run, Donchian alignment, all before any entry.

### 2.2 Skip Dose: "Right trade. Wrong size. Could not hold."

"EMA confirmed. Entry valid. But you went in too heavy."

- The trade dipped 3%, a normal pullback. But it felt like a disaster. You panicked and cut.
- After you exited, the trade ran exactly where you thought it would. Without you.

"A doctor who prescribes 10× the correct dose does not get 10× the result."

The chart: uptrend above EMA 50, valid entry, a three-candle red dip, "panic cut" at the dip low, then the run resumes. This is the ZETA slide from Module 5 section 2.3 in schematic form. The fix is Module 5 section 3.6: stake small enough that a 3% pullback at your leverage is a tolerable ROI swing. At 20× a 3% dip is −60% ROI; at 5× it is −15%. The "felt like a disaster" is a leverage choice, not a personality flaw.

### 2.3 Skip Discharge: "Won the trade. No exit plan. Gave it all back."

"Perfect entry. Correct dose. No exit plan."

- The trade went green. RM200. RM400. RM600. You thought, let it run a little more.
- It reversed. Fast. No take profit was set. **You gave back everything.**
- **The EMA exit signal fired during the reversal.** You had no discharge condition, so you held and hoped.

"A doctor who admits a patient but never writes the discharge plan keeps them in the hospital indefinitely."

The chart: uptrend, entry, "profit window" at the top with "TP (never set)" as a dashed line, then reversal through EMA 50, "closed at loss" at the bottom. Two things to notice:

- The slide names the **EMA exit signal** as the discharge condition that fired and was ignored. So the Module 1 cross-back rule is still part of the plan in this deck, as the backstop. Module 4's climax exit (volume maximal, MACD peak, PTP 75%) would have fired earlier, at the "profit window", and is the primary.
- "Held and hoped" is the exact behaviour the GMX hedging case study in Module 5 section 4.8 presented as the method. This slide calls it skipping Discharge.

## 3. The three failures, mapped to the course's own examples

| Skipped D | Failure slide | Course example that did the same thing | Where |
|-----------|--------------|----------------------------------------|-------|
| Diagnose | Entered on a signal, no chart check | The 18/3 BMT entry from a "it's pumping!" chat message, "late trade is a losing trade" | Module 5, section 3.10 |
| Dose | Right trade, too heavy, panic cut | ZETA "took profit too early" | Module 5, section 2.3 |
| Discharge | No exit plan, held and hoped | GMX held overnight on cross margin to breakeven; PEOPLE hedged instead of stopped | Module 5, sections 4.8 and 4.11 |

The 3D review slides are the right lens. Applied to the deck's own case studies, they mark most of the "advanced" material in Module 5 as a skipped D.

## 4. Q&A

_Not yet received._

## Open questions

- Are there further Module 6 case studies showing a complete trade with all three Ds executed, rather than one skipped?
- Does the Q&A address any of the open questions in Modules 1 to 5?
