# 01 — What is Scalping (短线交易的定义)

Source: Module 1 slides, Momentum Mastery Trading (MMT), Dr. Aaron MMT, 2026.

## 1. Scalping strategy: definition table

Transcribed from the "What is scalping strategy?" slide.

| Term | Definition |
|------|------------|
| Scalping Strategy | A trading strategy that involves making multiple trades within a short period to profit from small price fluctuations. |
| Objective | To take advantage of small price differentials and accumulate small profits repeatedly. |
| Holding Period | Very short-term, typically ranging from seconds to minutes. |
| Focus | Capturing small price movements and exploiting bid-ask spreads. |
| Trading Volume | Relies on high trading volume and liquidity for quick trade execution. |
| Tools | Advanced trading platforms and tools for identifying short-term price patterns and technical indicators. |
| Risk Management | Strict risk management and disciplined trade execution are crucial. |
| Frequency | High-frequency trading strategy, involving numerous trades in a single day. |
| Skill Set | Requires technical analysis proficiency, quick decision-making, and effective risk management. |
| Suitable For | Traders experienced in short-term trading, capable of handling stress and making rapid trading decisions. |

## 2. What the definition commits you to

Reading the table as a set of constraints rather than a description:

- **Many small wins, so costs dominate.** If the target per trade is a "small price differential", then fees, spread and slippage are a large fraction of each win. Coin selection (Module 2) has to filter for liquidity, not only for trend, or the edge is eaten by execution cost.
- **Holding period of seconds to minutes** means the timeframe for every later module (Heikin-Ashi, indicators, SPE, Wick Tracker) is intraday. Check which chart timeframe the course actually uses when those modules arrive; "seconds to minutes" is the textbook definition and may not match the course's practice.
- **"Exploiting bid-ask spreads"** is a market-maker's edge, not a directional trader's. The rest of the outline (trend, direction, sniper entry) is directional. Treat this line as the generic definition, not as what MMT teaches.
- **Risk management and discipline are named twice** (Risk Management row and Skill Set row). The course flags this as the failure point before teaching any entry technique. Module 5 is where it is operationalised.
- **"Suitable for experienced traders"** is a stated prerequisite. The course does not claim scalping is beginner-friendly.

## 3. MMT 3D framework: "The System that makes the difference"

Three questions, asked in order, on every trade. The vocabulary is medical (diagnose the patient, dose the medicine, discharge from care), which fits the "Dr. Aaron" branding. Strip the metaphor and it is the standard three-part trade plan: **entry, size, exit**.

| D | Question | Covers |
|---|----------|--------|
| **Diagnose** | Is the entry valid? And in which direction? | Coin selection, direction, entry timing |
| **Dose** | How much to risk? | Position size and stop loss |
| **Discharge** | When do I get out? (Take Profit / Stop Loss) | TP level, exit signal, SL level |

### 3.1 Diagnose: is the entry actually valid, and in which direction?

Slide text: "A doctor never prescribes before diagnosing. They look at the evidence first, not the symptom alone. **The signal is the symptom.** Your job is to diagnose, identify the direction and entry."

**Tool: Exponential Moving Average (EMA)**, described as "the heartbeat monitor of the chart". Two EMAs are plotted, a short-term and a long-term.

| Cross | Definition | Reading | Action |
|-------|------------|---------|--------|
| **Golden Cross** | Short-term EMA crosses **above** long-term EMA | Momentum turning up, market going up | Look for a **Long** entry |
| **Death Cross** | Short-term EMA crosses **below** long-term EMA | Momentum turning down, market going down | Look for a **Short** entry |

The "To Confirm Direction" chart shows both crosses on a daily chart (Feb to Jul): a death cross near the top, a golden cross after the bottom. On that chart, the golden cross prints well after the low. The cross is a lagging confirmation, which is exactly why the course's outcome 4 says "enter at the right moment, not the first moment".

Note the wording "look for" an entry. The cross sets the **direction** you are allowed to trade. It is not itself the entry trigger; that is Modules 3 and 4. "The signal is the symptom" is the same warning: a cross alone is not a diagnosis.

### 3.2 Dose: how much are you risking?

Slide text: "A doctor prescribes the right dose before the patient takes anything. Too much kills. Too little does nothing. **Your Dose is your position size and stop loss. Decide before you enter. It is not just about capital.**"

Two things are being said:

- Dose is two numbers, not one: **position size** and **stop-loss distance**. Together they define the money at risk. Sizing without a stop is not a dose.
- "Too little does nothing" is the half students ignore. Under-sizing after a losing streak is named as a failure mode alongside over-sizing.

No numbers are given on this slide. The percentage-per-trade rule, if there is one, is deferred to Module 5.

### 3.3 Discharge: when are you getting out?

Slide text: "A doctor never admits a patient without a discharge plan already written. **You never enter a trade without knowing your exit, win or lose, before you click buy.**"

Three concrete rules, given for a long:

| Exit type | Rule | Slide's own qualifier |
|-----------|------|----------------------|
| **Take profit** | Nearest resistance | "Set it first." |
| **Exit signal** | Short-term EMA crosses back below long-term EMA | "Exit. No questions." |
| **Stop loss** | Below EMA 50 | "Structural. Not emotional." |

For a short, mirror each rule: TP at nearest support, exit when short EMA crosses back above long EMA, stop above EMA 50.

Observations:

- **Two exit triggers on the losing side.** The EMA cross-back and the EMA 50 stop can both fire. Which comes first depends on whether the long-term EMA is the EMA 50 (see open questions). If it is, the cross-back usually fires before a decisive break of EMA 50, and the hard stop is the backstop for a gap or fast move.
- **"Set it first"** on take profit means the TP order goes in at entry, not after. Combined with "no questions" on the exit signal, the discharge rules are meant to be mechanical.
- **Nearest resistance** caps the reward. With a stop below EMA 50, the reward-to-risk ratio is whatever the chart gives, and the course does not state a minimum. That is a gap: a valid entry with TP closer than the stop is still allowed by these rules as written.

### 3.4 How the modules map onto the 3 Ds

| D | Modules that implement it |
|---|---------------------------|
| Diagnose | 2 (coin selection), 3 (direction), 4 (SPE, Wick Tracker) |
| Dose | 5 (risk management strategy, trading style, risk level) |
| Discharge | 4 (MMT New TP), 5 (MMT Hedging, Golden Rules) |

- **Diagnose gets most of the course.** Three of six modules are about whether to enter. Dose gets a single sub-bullet in Module 5. The weighting says the course sees entry quality as the edge and sizing as a fixed rule.
- **Stop loss appears in both Dose and Discharge.** Dose sets its distance (it determines size); Discharge sets its location (below EMA 50). Read together: the stop location is fixed by structure, and position size is then solved from it, not the other way round.
- **Discharge is split across two modules.** Take profit is taught in Module 4 (MMT New TP). Hedging is taught in Module 5. Expect the hedging module to substitute for, or delay, the EMA 50 stop; that is the thing to scrutinise most.

### 3.5 The three questions before opening a trade ("Can you do this?")

Slide checklist, verbatim:

1. Can you diagnose the setup? Identify the direction and entry?
2. Have you dosed your risk?
3. Do you have a discharge plan **written**?

"Written" is the operative word in question 3. Filled-in form for one trade:

| Question | Answer to write down |
|----------|---------------------|
| Diagnose | Coin, timeframe, which cross (golden or death), why the entry is valid now |
| Dose | Position size, stop distance, money at risk as a percentage of account |
| Discharge | TP price (nearest resistance or support), exit-signal rule, SL price (EMA 50) |

If any cell is blank, the framework says the trade is not valid.

## Open questions

- Which EMA periods are the "short-term" and "long-term" EMA? The stop rule names EMA 50, which suggests the long-term EMA is the 50. The short-term period is not given.
- Does the course define Dose as a fixed percentage of account per trade, or does it vary by "risk level"?
- Is there a minimum reward-to-risk ratio, or is any nearest-resistance TP acceptable?
- In Discharge, is hedging (Module 5) a replacement for the EMA 50 stop or a tool used alongside it?
- ~~Which chart timeframe does the course scalp on in practice?~~ Answered in Module 2: EMA direction is checked on every timeframe from daily to 1 minute; entries are timed on the 1m to 15m charts.
