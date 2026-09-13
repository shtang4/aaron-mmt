# MMT One-Page SOP

Distilled from Modules 0 to 6. Only what the course itself states, minus what it contradicts elsewhere; where the deck says two incompatible things, the version consistent with the Module 1 Discharge rule and the Module 5 risk slide is kept. The formatted, printable version is [tools/sop.html](../tools/sop.html).

## 0. Setup, once
- **Bybit chart:** Heikin-Ashi on · EMA 9, 25, 55, 155, 255 · MACD 8/13/9 · Volume VOLMA 5, 10.
- **TradingView:** Market Structure (Leviathan), BOS on close, CHoCH on · Donchian Trend Ribbon 20.
- **Coinglass:** liquidation heatmap, 1-week view.
- **Account:** isolated margin · one-way mode · TP triggers on Last, SL on Mark · Order by Value.

## 1. Scan the market (Diagnose)
1. Heatmap: mostly green → long bias; mostly red → short bias; mixed → no trades today.
2. Hot sectors → leading coin in each → Top Movers (24h, and the 15m tabs). A gainer is a candidate, never a trade.
3. Screener per candidate, scored out of 4: EMA 20 above/below on 1D + 4H + 1H · OI rising with price · funding on your side (≤ −0.01% for a long, ≥ +0.05% for a short; positive is accepted on longs in a bull market) · book lighter on the side you are trading. **4/4 → full size. 3/4 → 50–75% size, tighter stop. Below 3 in one direction → no trade.** Mixed timeframes → reduce size; all disagree → skip the coin.
4. Sentiment gauge is a clue, not a signal.

## 2. Set direction (Diagnose)
1. **EMA 155 rule:** three consecutive full-body candles above → long only; below → short only. Nothing else sets direction.
2. Heikin-Ashi run with no trend-side wicks confirms. Dojis or small-body clusters → wait.
3. Donchian ribbon solid in the same colour confirms. Mixed → skip.
4. Seahorse (vertical move done, flat beak, EMAs converging) → stay out.
5. Hockey stick (slow decline, sharp V, vertical blade): enter only on the golden cross *with* the EMA 155 three-candle rule. Never buy the blade.

## 3. Sniper entry (Diagnose, SPE)
1. TradingView: nearest demand zone below (long) or supply zone above (short), and any FVG. Take the near edge.
2. Bybit: **EMA 9** is the first target; if the zone edge sits deeper, the EMA closest to the edge. That is the price.
3. Rest a limit order there. Re-place it if the EMA moves. Never market-buy the running candle.
4. Correlated alts making the same move at the same minute are one trade. Size the total.

## 4. Size and stop (Dose)
1. Isolated margin. Leverage 5× to 10×.
2. Margin per trade: $20 to learn; then 1% of wallet; never above 10%. Bigger wallet, smaller trade. **Loss at the stop never above 1–2% of account equity**, whatever the confluence score.
3. Stop as ROI on margin by tier: beginner 5–20%, intermediate 20–50%, advanced 50%+. Convert to price; it must sit beyond the structural level (far edge of the zone, or the heel low). If it does not, **lower the leverage** until it does (session-confirmed). Never move the level, never widen the tier.
4. Write the money at risk in USDT before entry.

## 5. Exit plan, both ways (Discharge)
1. TP first. Wick Tracker is a Bybit TP trigger at a level a wick will reach: prior wick high, supply-zone bottom, liquidation cluster, or 50% ROI raised to 55–60% for fees. Trigger on **Last**; set it slightly inside the expected wick so it fills.
2. SL from step 4, trigger on Mark, **resting before the entry fills**. Both orders in before you look away.
3. Climax exit: volume bar far above VOLMA + MACD histogram at its **tallest bar**, confirmed when the next bar prints shorter → close 75%. Move the runner's SL to entry.
4. Runner: Hunting SL locks a rising ROI. EMA 9 crossing back through EMA 25 is the backstop: exit, no questions.
5. Stop hit = the plan worked. Take it.

## 6. After the close (Follow up)
1. Sweep realised profit from Derivatives to Funding.
2. Close and go. Next coin. Never re-enter the same beak.
3. Stop at the daily target or ten trades, whichever first. Rest.
4. Log it in the journal: which D, which rule, what you would change. Thirty trades before you believe any number.

## 7. When it goes wrong (Discharge)
1. The stop is the answer. It was written before entry; honour it.
2. If you skipped the stop and are underwater: close it. The loss is the loss.
3. If you want the opposite direction: close the loser first, open the new trade as its own sized position with its own stop. Never both legs at once.
4. **The one hedging case:** a position opened in cross mode by mistake. Hedge it to freeze exposure, then close it or switch it to isolated, then close the hedge. Damage control for an execution error, nothing more.
5. News, FOMC, black-swan candles: no method is 100%. Smaller dose, or flat.

## Formulas
| | |
|-|-|
| Stop / TP distance | `entry × ROI% ÷ leverage` (Bybit ROI = P&L ÷ margin) |
| Round-trip fees as ROI | `2 × 0.055% × leverage` (taker; 20× ≈ 2.2%) |
| Reward : risk | `|TP − entry| ÷ |entry − stop|` · breakeven win rate `1 ÷ (1 + R)` |
| Money at risk | `margin × stop ROI%` (+ fees); handouts: never above 1–2% of equity |
| Max leverage for a structural stop | `entry × ROI% ÷ |entry − level|` |
| Hunting SL trigger | `entry ± entry × locked ROI% ÷ leverage` |

## Never, because the course's own risk module says so
- Cross margin. Liquidation takes the whole wallet.
- A position without a resting stop. Handouts: "set it before the entry order fills."
- Hedging instead of taking the stop. The only hedge is on an accidental cross-mode position, and it ends with closing it.
- Holding a loser to breakeven.
- Trading a mixed heatmap or a seahorse.
- Entering on a chat call without the chart check.
- Holding for days. This is not swing trading.
- New listings beyond a few days.
- Adding size after a loss.
- Blaming mindset before checking which D you skipped.
