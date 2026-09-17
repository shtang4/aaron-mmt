# 04 — Advance MMT Sniper Entry & Exit

Source: Module 4 slides, Momentum Mastery Trading (MMT), Dr. Aaron MMT, 2026.

Module contents (from the section title slide, with the 3D role of each):

| Item | 3D role |
|------|---------|
| MMT SPE (Sniper Price Entry, 狙击价格入场) | Diagnosis |
| MMT Take Profit Strategy (the outline called it "New TP") | Discharge |
| MMT Wick Tracker (烛芯跟踪器) | Discharge |

## 1. MMT Sniper Price Entry (SPE)

Slide text, verbatim with light cleanup:

- Use the SMC indicator.
- Define where the Supply and Demand zones are, and any FVG, in TradingView.
- If there is any:
  - aim at the **bottom of the Supply Zone** if planning to SHORT;
  - aim at the **top of the Demand Zone** if planning to LONG;
  - the same for an FVG, which becomes the baseline of it.
- After that, go back to Bybit and **aim at the nearest of the 5-line EMAs** and enter at that point.
- Sometimes the aim can be higher than the Demand Zone, on one of the 5 EMAs; or lower than the Supply Zone, on one of the 5 EMAs.

### 1.1 The procedure, assembled

SPE is a two-platform confluence entry:

1. **TradingView** (Leviathan Market Structure indicator, Module 3 section 3.4): mark the nearest demand zone below price (for a long) or supply zone above price (for a short), and any FVG.
2. Take the **proximal edge** of the zone: the top of a demand zone, the bottom of a supply zone. That is the first price the retrace will touch. An FVG's near edge works the same way.
3. **Bybit** (5-line EMA, Module 3 section 2.2): find the EMA closest to that edge. The entry is a **limit order at that EMA**.
4. If the EMA sits inside or beyond the zone (above the demand zone for a long), the EMA still wins: the slide's last bullet says the aim can be above the demand zone or below the supply zone when the EMA is there.

**The limit order is the default, not a variant.** From the A8 case study ([06 §6.2](06-case-studies.md)): "Buy now means you enter by market price, limit buy you enter by limit order ... **Don't enter as a market order unless some critical condition.**" The slide's own arithmetic: the member who asked "buy now or limit buy" at a price of 0.23861 was filled at 0.23152, 3.0% better, which at 10× leverage is **30 percentage points of ROI**. A market order is something you have to justify — a breakout you have already drawn, a stop that must go on now — not the normal way in.

So the SMC zone tells you *where* the pullback should end, and the EMA gives the *exact price* to rest the order at. The two are read on different platforms because the SMC indicator is TradingView-only and the trade is placed on Bybit.

### 1.2 What he says SPE actually means, and why it is not a rule

From the ZETA walkthrough, the only time in the course he defines the term:

> "What do you mean sniper price entry? Sniper price entry whereby **whatever price entry you enter and it will come back and challenge you, that's not considered.** But if let's say keep on retrace, go up, retrace go up, and **the further the distance from your entry level the better** is. This is what you call sniper price entry."

Read it carefully, because it is a **verdict, not a procedure**. A sniper entry is defined by what happens *after* the fill: price never returns to challenge the level, and the gap between price and your entry keeps widening. Nothing in that definition tells you where to put the order. You find out whether your entry was a sniper entry by waiting.

Three consequences worth being clear about:

- **The actionable content of SPE is elsewhere**: the zone edge, the EMA, the limit order, and the EMA 155 direction rule. That is the procedure in 1.1. The definition above grades it afterwards.
- **It is a good grading rule even so.** "Price came back and challenged my entry" is a clean, checkable journal field, and a run of challenged entries means you are buying into the move rather than in front of it. It belongs in the journal, not in the checklist.
- **It quietly rules out chasing.** An entry taken into a running candle is, by this definition, almost never a sniper entry: price is already extended and any pause brings it back through your level. That is the same rule as "don't enter as a market order unless some critical condition", arrived at from the other direction.

**Every line is parkable, and the order follows the line.** "If you miss this, you can up here. If you miss this here, you park here. **Just follow along the line.**" So the resting order is re-placed up the EMA as the trend advances, and any of the five lines qualifies — he points at EMA 155 on the ZETA chart. EMA 9 (the confirmed first target) is the shallowest and most frequently filled; EMA 155 is the deepest with the pivot rule behind it; EMA 255 is "the last guard". The choice is a trade-off between fill rate and how far the stop must sit.

### 1.3 What the slide leaves out

- **The stop.** SPE places the entry and says nothing about the stop. The structural stop for a zone entry is just beyond the far edge of the zone: below the bottom of the demand zone for a long, above the top of the supply zone for a short. The stop distance is set by the ROI tier in Module 5 section 3.2 converted to price. **Confirmed from the session: when the zone's far edge is further than the tier allows, lower the leverage until the tier stop sits beyond the zone.** The tier (and so the money at risk) stays fixed; the leverage gives. Formula: max leverage = entry × tier ROI ÷ |entry − zone far edge|. The pre-trade checklist prints this number.
- **Which EMA first.** Confirmed from the session: **EMA 9.** That is the shallowest pullback and the most frequent fill, and it is also the line price slices through first when the trend ends. The consequences: the stop does the filtering (it must sit beyond the zone, not just under EMA 9), the EMA 155 three-candle rule must already be true, and on a 1-minute chart the EMA 9 moves every candle, so the limit order has to be re-placed as it moves. A deeper line with a zone behind it is a more conservative variant, not the taught one.
- **Direction is assumed.** SPE only tells you where to enter once the direction is set. The direction comes from EMA 155 (three full-body candles on one side, Module 3 section 2.2) and the screener (Module 2 section 5).
- **Time-in-force.** A resting limit at an EMA goes stale as the EMA moves. On a 1-minute chart EMA 9 moves every candle. Either re-place the order each candle or aim at the slower line.

### 1.4 How SPE connects to what came before

| Earlier slide | What it said | What SPE adds |
|---------------|-------------|---------------|
| Module 3, ZETA 2-EMA vs 5-EMA | "SPE Entry" at a pullback to one of the five EMAs | The zone check that qualifies which pullback |
| Module 3, tips | "Setting entry price with prediction" | The prediction is the zone edge; the price is the EMA |
| Module 3, airport analogy | Wait at the lounge, don't chase | The lounge is the zone-plus-EMA level |
| Module 5, SSWB step 4 | "Enter using MMT SPE" | This is that step |

## 2. MMT Take Profit Strategy

Title slide: **"MAVol + MACD + Take Profit / Mãn Mãn Tiàp → Sip the profit slowly."** "Mãn Mãn Tiàp" is Hokkien for "slowly sip" (慢慢啜).

Five-step flow, verbatim:

1. When the **Volume hits maximal**
2. Observe **MACD**
3. Choose the **mid Histogram**
4. Then **TP, or PTP 75%**, set **SL to entry** or **Hunting SL**
5. **Do not be greedy!!**

### 2.1 What each step means

**Step 1, volume maximal.** The exhaustion spike from Module 3 section 2.7: a volume bar far above the VOLMA 5 and 10 lines, at the climax of the move. In a long, that bar is the buyers' last push. The take-profit process starts on that candle, not after it.

**Defined, from the spoken session** ([03 §2.7a](03-entry-direction.md)), and it replaces the working rule these notes carried: *"whichever volume bar pump across this two lines — these are the abnormal volume."* **A bar that rises above both VOLMA lines (5 and 10) is abnormal; bars under the lines carry no signal.** The threshold is the indicator, not a multiple, which is better because the two averages adapt to the coin and the session.

Two readings come with it. **Colour is the side** — red is selling power, green buying. And **a long wick on the candle means the bar was a liquidity sweep, not a move**: "it's just want to sweep the liquidity, it's not a full block". A full-bodied candle on abnormal volume is the real thing. So for the exit: an abnormal green bar with a long upper wick at a high is the climax; an abnormal green bar with a full body may be a breakout that keeps going.

The stricter filter I had proposed (tallest since entry, and 2× VOLMA 10) is retired as the definition but is worth keeping as an optional second gate if the journal shows the exit firing too early.

**Steps 2 and 3, MACD mid histogram.** With the MMT setting (8, 13, 9) the histogram reacts fast. Confirmed from the session: "mid histogram" is **the tallest bar** of the swing — his "**mountain peak**" ([03 §2.6a](03-entry-direction.md)). The partial fires when the next bar prints shorter than it: momentum has peaked even though price may still be rising.

**And that bar is visible without measuring it.** On Bybit a histogram bar smaller than the one before it is drawn **hollow**. So **the first hollow bar after a run of solid bars is this trigger** — no height comparison needed. The course explains the hollow bar as "caused by counter volume", which is mechanically impossible since MACD is computed from price EMAs alone and never sees volume; the correction and why it makes the signal better are in [03 §2.6b](03-entry-direction.md). Confirm the convention once on your own chart before relying on it.

**The cost of missing the peak, in his own ladder:** peak → equilibrium is **half the profit gone** → back to entry is all of it → below entry is a loss. Same argument as the ZETA closing slide, made on the indicator instead of the price. That is the same signal the RAVE example in Module 5 annotated "IceBerg Tip" at the bottom of a crash, used in reverse at a top. In practice the tallest bar is only known once the next bar is shorter, so the exit is one candle after the peak, on the 1-minute chart.

**Step 4, TP or PTP 75%.** Either close the whole position, or close **75%** and keep 25% as the runner. On the runner, move the stop to entry (it can no longer lose) or apply the Hunting SL from Module 5 section 3.3 (lock a rising fraction of ROI). Note the number: 75% off is a much larger partial than the Module 5 example's "take 20% profit, leave 80% for the wick", which was about locking ROI with a stop, not about position size. Here most of the position is closed at the climax.

**Step 5.** The runner is the concession to greed, and it is small by design.

### 2.2 This replaces the Module 1 exit rule

Module 1 said: "Exit signal: short-term EMA crosses back below long-term EMA. Exit. No questions." That is a lagging exit; it fires after the pullback has already taken a large share of the gain, as the course's own Diagnose comparison chart showed.

The Module 4 rule exits **at the climax**, before the pullback, on volume and momentum. Then the runner is protected by a breakeven or trailing stop, and the EMA cross-back, if it comes, takes out the runner only. Read together:

| Exit | Trigger | Applies to |
|------|---------|-----------|
| Primary (Module 4) | Volume maximal + MACD histogram peaking | 75% to 100% of the position |
| Runner protection (Module 5) | Stop to entry, then Hunting SL | Remaining 25% |
| Backstop (Module 1) | EMA cross-back | Whatever is still open |
| Hard stop (Module 1, Module 5) | Structural level, ROI tier | Whole position, from entry |

The Module 5 ZETA slide ("right trade, but take profit too early?") argued for holding through a retrace. Module 4's own rule would have taken 75% at the first climax on ZETA and left a 25% runner for the eventual tripling. That is a coherent answer to the ZETA slide, and a better one than "hold everything".

### 2.3 The second regime: an opening fan needs no fixed target

From the A8 case study ([06 §6.4](06-case-studies.md)): "by looking at the EMA, the opening is exponentially, never cross yet, so means that **you can hold very nicely without a TP as well.** So you can see, all not crossing each other."

So the course runs **two exit regimes**, and the EMA fan decides which one you are in:

| Fan state | Target | What closes the trade |
|-----------|--------|----------------------|
| Fan widening, no two lines crossing | **No fixed TP needed** | The climax rule, then the first EMA cross (9 back through 25). The Wick Tracker still rests as the unattended backstop. |
| Fan flat, bunched, or lines crossing back and forth | **Set the target** | Wick Tracker level or the ROI target, whichever is nearer. This is also a chart the direction rules say to skip. |

Neither regime touches the stop: it is set before entry, it rests, and it does not move except to lock profit. The A8 rule and the SOMI line ("most of the time it never hits the TP; for a scalper the TP is an art") are the same position stated twice — **the stop is mechanical, the target is conditional** — and the fan width is the test for which case you have. The retracement test ([03 §2.2](03-entry-direction.md)) is what keeps you in during the regime-one hold: losing one, two or three fast lines is a dip, three full bodies below EMA 155 is the exit.


## 3. MMT Wick Tracker

Slide text: "To use the possible wick hit level as the guide of the TP entry, and when the wick hits, then it automatically self-TPs and closes the trade. No need monitoring."

### 3.1 What it is

A take-profit order placed at a level a **wick** is expected to reach, so that a spike fills the exit even if the candle closes lower. It is the exit counterpart of SPE: SPE rests a limit order where the pullback wick will reach; the Wick Tracker rests a take-profit where the extension wick will reach.

The "possible wick hit level" is not defined on the slide. Everything earlier in the course that names a level price is drawn to:

| Level | Source |
|-------|--------|
| **Slightly above** the prior swing high's wick | Price action, this slide. Session ([03 §2.7b](03-entry-direction.md)): "the last higher was around here, like wick tracker — you can set somewhere higher a bit, so this one is higher than this one. Then the next pump will trigger your wick tracker." Stops rest above a prior high, so a sweep aiming at that liquidity overshoots it. A member rule endorsed on the MAVIA slide ([06 §5.2](06-case-studies.md)): on a manipulative coin, "set higher price, refer to previous high or set even higher" |
| Bottom of the next supply zone | SMC, Module 3 section 3 |
| The next FVG's near edge | SMC, Module 3 section 3 |
| A liquidation cluster above price | Coinglass heatmap, Module 3 section 4.2 |
| Equal highs (liquidity resting above) | SMC, Module 3 section 3 |
| Nearest resistance | Module 1 Discharge rule |

The SSWB SOP in Module 5 used the Wick Tracker differently: as a **50% ROI** target (55% to 60% with the fee buffer), "sometimes set lower than the previous high wick spike". So in practice the Wick Tracker is whichever is nearer: the ROI target or the wick level.

### 3.2 The mechanics that make or break it on Bybit

- **Trigger price type.** Bybit TP/SL orders trigger on Last, Mark or Index price. A wick is a Last-price event; the Mark price is smoothed and often does not reach the wick. The THETA screenshots in Module 5 section 3.4 had **TP triggered by Last** and **SL triggered by Mark**. That is the correct pairing: TP catches the wick, SL ignores it. Set it that way every time.
- **It is a TP trigger.** Confirmed from the session: the Wick Tracker is set on Bybit's TP/SL screen, and when price reaches it the position closes automatically. That is a trigger that sends a market order on the touch, so on a wick the fill lands a few ticks after the touch, once the wick starts retracing. Two consequences: trigger on **Last** (Mark rarely reaches a wick), and set the level a little inside the wick you expect rather than at its extreme, so the trigger fires with room to fill. A resting limit at the level would fill at the price or not at all; it is the more precise instrument, but it is not what the course teaches.
- **"No need monitoring" is contradicted by the session.** On the SOMI trade call ([06 §2.5](06-case-studies.md)) he says the opposite in plain words: "Most of the time, it never hits the TP ... **If you do not monitor, this will happen to you.** For a scalper, the TP sometimes is an art, it is not a definite setting there. Enter, set stop loss, set the TP and walk away: that is swing trade. We are scalping."

  The reconciliation these notes use: **the stop is mechanical and fixed, the target is a plan you may improve on while watching.** The Wick Tracker still rests, because an unattended spike should fill it, but treat it as the backstop rather than the expected exit. The expected exit is the climax rule in section 2, and near the funding settlements (8 AM, 4 PM and midnight Malaysian time) taking what is on the table beats waiting for a level that usually is not reached.
- **The case that justifies the whole idea.** The ZETA closing slide ([06 §7.5](06-case-studies.md)) is the Wick Tracker's best evidence in the course. The level was set at **2.8530** against an eventual high of **2.8700** — one and a half cents of headroom, chosen before the trade — and it fired. The coin then fell to **0.04533** by April 2026, 98% off the high and 95% below the entry. His own caption: **"Current Price (Never exit will liquidate)."** So on the one trade the course shows end to end, the pre-set take-profit is the only thing between the position and zero. Whatever else is arguable about the Wick Tracker, *having a written level and taking it* is the rule the deck proves.
- **And it fixes the level-choosing problem in 3.1.** 2.8530 was not a round number or an ROI target; it was a wick level read off the chart, and the wick came within 0.6% of it. That is the table in 3.1 working as intended.
- A TP order alone with no stop is a position that can be liquidated while you are not watching. Both must be resting before you leave the screen, whatever your intention about monitoring.

### 3.3 Golden Rule 11, "Wick Player / Wick Catcher"

Module 5's rule 11 teased "how to be a Wick Catcher without a Master". This slide is the answer, and it is one sentence. The skill in it is choosing the level, which is the table in 3.1; the mechanics are the trigger type and order type in 3.2.

## 4. The full trade, all six modules

| Step | Tool | Module |
|------|------|--------|
| Scan for candidates | Bybit Opportunities: sentiment, heatmap, hot sectors, top movers | 2 |
| Grade the candidate | Coin Trend Screener: multi-TF EMA, OI, funding, depth | 2 |
| Set direction | EMA 155, three full-body candles; Donchian ribbon aligned; Heikin-Ashi run | 3 |
| Choose the entry level | SMC zone edge on TradingView, nearest 5-line EMA on Bybit | 4 (SPE) |
| Size | Isolated, 5× to 10×, $20 to $150 or 1% to 10% of wallet | 5 |
| Stop | ROI tier converted to price, beyond the zone's far edge; trigger by Mark | 5, 4 |
| Take profit | Wick Tracker at a wick level or 50% ROI; trigger by Last or resting limit | 4 |
| Manage | Volume maximal + MACD peak → PTP 75%, SL to entry, Hunting SL | 4, 5 |
| Close and go | Sweep profit to Funding, next coin, stop at daily target | 5 |

## Open questions

- Where does the SPE stop go: below the zone, or at the ROI tier, when the two disagree?
- Does the course have a worked example of the full sequence on one trade, with entry, stop, PTP and runner all shown? (No: see Module 6. ZETA comes closest and still shows no stop.)
- ~~Volume "maximal" is defined by my working rule, not the course's.~~ **Answered:** a bar above both VOLMA lines is "abnormal"; no multiple. See §2.1 and [03 §2.7a](03-entry-direction.md).
- Does the hollow-bar convention on Bybit match the standard "smaller than the previous bar"? Confirm once on a live chart; the climax trigger becomes a glance if so.
