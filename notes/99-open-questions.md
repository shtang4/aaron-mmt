# 99 — Consolidated open questions

The full deck (Modules 0 to 6) is captured. These are the questions the slides do not answer, grouped by what they would change. Each links to the module where it arose. Items answered from the session so far are recorded in the module files and not repeated here.

## A. Questions that change whether a trade is taken

| # | Question | Module | Why it matters |
|---|----------|--------|----------------|
| ~~A1~~ | ~~Minimum screener confluence?~~ Answered by the handouts: 4/4 full size; 3/4 at 50–75% size with a tighter stop; below 3 in one direction, no trade. | 7 §1.1 | |
| ~~A2~~ | ~~Depth check definition?~~ Answered: lighter ask → long, lighter bid → short, equal → skip; beware a single hidden wall. | 7 §1.2 | |
| ~~A3~~ | ~~Does the hockey stick override funding?~~ Answered: funding is a scored layer with a bull-market override; the SOL long was a 3/4 and should have been at reduced size. | 7 §1.3 | |
| A4 | When two of the seven chart tools disagree, which wins? | 3 §4.3 | Only EMA 155 has stated priority. Disagreement is the normal case. |
| ~~A5~~ | ~~Full-body candle, and on which chart?~~ Session: read on the **Heikin-Ashi** chart with the Bybit setup on. "Full body" is therefore the Heikin-Ashi strong-trend candle from Module 3 §1.2: body on the trade side of EMA 155 with no wick on the opposite side. | 3 §2.2 | |
| A6 | In the hockey stick rule, is "the EMA" the 155 or a faster line? | 2 §6.4 | Moves the entry by minutes and percent. |
| A7 | Is the RAVE crash-bottom (heel) entry a taught setup or a one-off? | 5 §3.9 | It contradicts the confirmed hockey stick rule. |
| A8 | Does the uncorrelated-pump trade during a BTC crash have rules (scan, stop, exit) or is it one observation? | 6 §4 | AERGO on 7 April 2025 is the only evidence. |
| ~~A9~~ | ~~Strong versus shit coin defined?~~ Session: strong = good background and fundamentals; shit = unknown background, rug-pull or manipulation risk. Then: "all coins are manipulative until proven otherwise." Category is not a filter; volatility and volume are. | 2 §2 | |

| ~~A10~~ | ~~Which EMA rule wins?~~ Session: the handouts are supplementary. The slides' EMA 155 three-candle rule sets direction; EMA 20 on 1D/4H/1H is an optional higher-timeframe filter. | 7 §2.1 | |
| ~~A11~~ | ~~Is 1-minute the execution chart?~~ Session: yes. The risk checklist's "danger" line refers to reading 1m without the higher timeframes. | 7 §2.2 | |

| **A12** | **Depth check direction.** Handouts: long when the ask side is lighter. Spoken session: long when the bid (green) side is lighter. These are opposites. Which did he mean? | 8 part 3 | The Fetch-from-Bybit panel ticks the depth box by the handout logic. If the spoken rule is intended, it ticks the wrong way. **Ask this one first.** |

## B. Questions that change the entry price

| # | Question | Module | Why it matters |
|---|----------|--------|----------------|
| ~~B1~~ | ~~Which EMA does SPE target first?~~ Session: **EMA 9**. The shallowest pullback and the most frequent fills; the stop and the EMA 155 direction rule carry the filtering. | 4 §1.2 | |
| B2 | Which EMA did the ZETA pullback touch at 0.8570? | 3 §2.3 | The course's showcase SPE entry, unlabelled. |
| B3 | Are the 15m Gainers/Losers tabs used, or only 24h? | 2 §4.4 | The 15m tabs match the holding period; the course uses 24h. |

## C. Questions that change the stop

| # | Question | Module | Why it matters |
|---|----------|--------|----------------|
| ~~C1~~ | ~~Where does the SPE stop go when the zone is wider than the ROI tier allows?~~ Session: **lower the leverage** until the tier stop sits beyond the zone's far edge. The tier and the money at risk stay; the leverage gives. | 4 §1.2 | |
| ~~C2~~ | ~~Does the SSWB SOP use a stop?~~ Session: yes, with isolated margin. The ROI tier is the Module 5 §3.2 table. | 5 §3.12 | |
| ~~C3~~ | ~~Is the stop ever stated as the rule?~~ Yes, in both handouts: "Always set your stop loss before the entry order fills." The hedging section stands contradicted by the course's own handouts. | 7 §1.5 | |
| ~~C4~~ | ~~What does "hedging when suitable" mean?~~ Session: hedge only for a trade accidentally opened in cross mode. Never as a substitute for the stop on an isolated position. | 5 §4.12 | |
| C5 | Was Bybit hedge mode mentioned? | 5 §4.5 | Without it a short against a long on one contract closes the long. |

## D. Questions that change position size

| # | Question | Module | Why it matters |
|---|----------|--------|----------------|
| D1 | Which stake is the taught one: $20 (SOP), $150 (real example), 1% to 10% of wallet, or the $1,000 on the 1% slide? | 5 §3.13 | Four unreconciled numbers. |
| ~~D2~~ | ~~Margin or loss?~~ Answered: "never risk more than 1% to 2% of total account equity on any single trade" is a maximum-loss rule. The $20 stake with a 20% stop is 0.2% of a $2,000 wallet. | 7 §1.5 | |
| D3 | Is 25× (demo) or 5× to 10× (slide) the recommendation? | 5 §3.4 | The demo and the rule disagree. |
| D4 | Was the THETA demo isolated or cross? | 5 §3.4 | Its liquidation distance does not match isolated 25×. |
| D5 | How were the six simultaneous cross-margin positions on the "execute 10 trades" slide explained? | 5 §3.12 | They contradict the SOP's TP, hold time and margin mode. |
| D6 | Was BMT on cross 15× presented as the recommended setup? | 5 §3.10 | The showcase trade used the mode the risk slide prohibits. |

## E. Questions that change the exit

| # | Question | Module | Why it matters |
|---|----------|--------|----------------|
| ~~E1~~ | ~~What is "mid histogram"?~~ Session: **the tallest bar** of the swing. The 75% partial fires when the next bar is shorter. | 4 §2.1 | |
| ~~E2~~ | ~~Volume "maximal" definition?~~ Session: no specific rule. **Working rule (mine, to be validated in the journal):** the bar is the tallest since entry and at least 2× VOLMA 10. | 4 §2.1 | |
| ~~E3~~ | ~~Wick Tracker: limit or trigger?~~ Session: a **TP trigger**; when price reaches it the position closes automatically. Set it to trigger on Last so a wick reaches it; expect the fill a few ticks after the touch. | 4 §3.2 | |
| E4 | Which timeframe is the EMA cross-back exit read on? | 1 §3.3 | On 1m it is late; on 15m it is a different trade. |
| E5 | Is there a minimum reward-to-risk ratio? | 1 §3.3 | Never stated in six modules. |

## F. Questions about the evidence

| # | Question | Module | Why it matters |
|---|----------|--------|----------------|
| F1 | Over what period did 1,993 → 18,288 USDT happen, and how many losing trades were in it? | 5 §3.10 | The only account-level result, undated and loss-free. |
| F2 | How many held-to-breakeven positions did not recover? | 5 §4.8 | GMX is one that did. |
| F3 | Does any complete trade exist with entry, stop, partial TP and runner all shown? | 6 | None in the deck. |

## What the deck settles without the session

For contrast, the things that needed no clarification: the exchange and product (Bybit USDT perpetuals), the 1-minute entry chart, the five EMA periods and colours, the MACD and volume settings, the TradingView SMC and Donchian settings, the Coinglass heatmap, the EMA 155 three-candle direction rule, the SPE two-platform procedure, the climax take-profit with PTP 75%, the Hunting SL formula, the ROI-tier stop conversion, the SSWB eight steps, the twelve Golden Rules, and the arithmetic on every result card, all of which reconciles.
