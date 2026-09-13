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

## 3. SSWB (Advance Dose)

_Not yet captured. Acronym not expanded on the title slide._

## 4. Advance tool: MMT Hedging (Discharge)

_Not yet captured._

## 5. MMT Golden Rules (Follow up)

_Not yet captured._

## Open questions

- Is the "1% to 10% amount" margin per trade or risk per trade?
- Does the course prescribe a maximum leverage for the conservative style beyond "1× to 10×", and a number for the aggressive style beyond "maximise"?
- What does SSWB stand for, and what does it add to the 1% to 10% amount rule?
- Does Module 4's New TP or Wick Tracker replace the Module 1 "EMA cross-back, exit, no questions" rule? The ZETA case says hold through a cross-back; Module 1 says exit on it.
- Is hedging (section 4) a replacement for the stop loss or a tool used alongside it? This is the question that decides whether the Discharge rule survives contact with Module 5.
- What are the Golden Rules, and do they resolve the "no SL, cross margin" contradiction in the Module 3 seahorse slide?
