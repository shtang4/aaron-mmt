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

So the SMC zone tells you *where* the pullback should end, and the EMA gives the *exact price* to rest the order at. The two are read on different platforms because the SMC indicator is TradingView-only and the trade is placed on Bybit.

### 1.2 What the slide leaves out

- **The stop.** SPE places the entry and says nothing about the stop. The natural structural stop for a zone entry is just beyond the far edge of the zone: below the bottom of the demand zone for a long, above the top of the supply zone for a short. That sits close to the "below EMA 55 or 155" rule from Modules 1 and 3 in most cases, and it should be set by the ROI tier in Module 5 section 3.2 converted to price. If the zone's far edge is further than the ROI tier allows, the leverage is too high for that trade.
- **Which EMA first.** "Nearest" means the first EMA the retrace reaches, which in a strong trend is EMA 9 or 25. Those give the shallowest pullback and the most frequent fills, and they are also the ones price slices through first when the trend ends. The ZETA example in Module 3 (entry 0.8570) did not say which line was hit. A deeper line (55) with a zone behind it is the more conservative version of the same entry.
- **Direction is assumed.** SPE only tells you where to enter once the direction is set. The direction comes from EMA 155 (three full-body candles on one side, Module 3 section 2.2) and the screener (Module 2 section 5).
- **Time-in-force.** A resting limit at an EMA goes stale as the EMA moves. On a 1-minute chart EMA 9 moves every candle. Either re-place the order each candle or aim at the slower line.

### 1.3 How SPE connects to what came before

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

**Steps 2 and 3, MACD mid histogram.** With the MMT setting (8, 13, 9) the histogram reacts fast. "Mid histogram" is not defined on the slide. The reading that fits the surrounding steps: the histogram is at or near its **tallest bar** for the swing, the middle of the momentum burst, and the next bar is shorter. Momentum has peaked even though price may still be rising. That is the same signal the RAVE example in Module 5 annotated "IceBerg Tip" at the bottom of a crash, used in reverse at a top. An alternative reading, that "mid" means the histogram has fallen to half its peak height, would exit later and give back more; the "sip slowly" framing and step 5 argue for the earlier reading.

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

## 3. MMT Wick Tracker

Slide text: "To use the possible wick hit level as the guide of the TP entry, and when the wick hits, then it automatically self-TPs and closes the trade. No need monitoring."

### 3.1 What it is

A take-profit order placed at a level a **wick** is expected to reach, so that a spike fills the exit even if the candle closes lower. It is the exit counterpart of SPE: SPE rests a limit order where the pullback wick will reach; the Wick Tracker rests a take-profit where the extension wick will reach.

The "possible wick hit level" is not defined on the slide. Everything earlier in the course that names a level price is drawn to:

| Level | Source |
|-------|--------|
| A prior swing high's wick | Price action, this slide |
| Bottom of the next supply zone | SMC, Module 3 section 3 |
| The next FVG's near edge | SMC, Module 3 section 3 |
| A liquidation cluster above price | Coinglass heatmap, Module 3 section 4.2 |
| Equal highs (liquidity resting above) | SMC, Module 3 section 3 |
| Nearest resistance | Module 1 Discharge rule |

The SSWB SOP in Module 5 used the Wick Tracker differently: as a **50% ROI** target (55% to 60% with the fee buffer), "sometimes set lower than the previous high wick spike". So in practice the Wick Tracker is whichever is nearer: the ROI target or the wick level.

### 3.2 The mechanics that make or break it on Bybit

- **Trigger price type.** Bybit TP/SL orders trigger on Last, Mark or Index price. A wick is a Last-price event; the Mark price is smoothed and often does not reach the wick. The THETA screenshots in Module 5 section 3.4 had **TP triggered by Last** and **SL triggered by Mark**. That is the correct pairing: TP catches the wick, SL ignores it. Set it that way every time.
- **Trigger-then-market versus resting limit.** A TP set on the TP/SL screen is a trigger that sends a market order when touched. On a wick, the market order fills *after* the touch, at whatever price is there once the wick retraces, which can be well below the wick. A **resting limit sell** at the wick level fills only if price trades through it, and at that price or better. For a wick tracker the resting limit is the better instrument; the TP trigger is the fallback when a limit is not possible (for example, reduce-only on a partial).
- **"No need monitoring"** is true only if the stop is also in place. A TP order alone with no stop is a position that can be liquidated while you are not watching. The Wick Tracker is a Discharge tool for the winning side; the Module 5 ROI-tier stop is the losing side, and both must be resting before you leave the screen.

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

- What exactly is "mid histogram": the tallest bar of the swing, or the bar at half the peak height?
- Which EMA does SPE target first in practice: the nearest (9 or 25) or a deeper one with a zone behind it?
- Where does the SPE stop go: below the zone, or at the ROI tier, when the two disagree?
- Is the Wick Tracker placed as a resting limit or as a TP trigger? The slides show only the TP/SL screen.
- Does the course have a worked example of the full sequence on one trade, with entry, stop, PTP and runner all shown?
