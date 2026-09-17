# MMT One-Page SOP

Distilled from Modules 0 to 6. Only what the course itself states, minus what it contradicts elsewhere; where the deck says two incompatible things, the version consistent with the Module 1 Discharge rule and the Module 5 risk slide is kept. The formatted, printable version is [tools/sop.html](../tools/sop.html).

## 0. Setup, once
- **Bybit chart:** Heikin-Ashi on · EMA 9, 25, 55, 155, 255 · MACD 8/13/9 · Volume VOLMA 5, 10.
- **TradingView:** Market Structure (Leviathan), BOS on close, CHoCH on · Donchian Trend Ribbon 20.
- **Research tabs, four on every coin** (session): TradingView chart · **CoinMarketCap** page · the project's **X** account · Coinglass heatmap. "Go to CoinMarketCap for basic fundamental, and check X and **Telegram** for news."
- **On the CoinMarketCap page, two numbers** (mine, not his): **volume ÷ market cap** — above ~50% the whole float is churning today, which is a pump, not accumulation (BSB 94%, RARE 211% on his own screenshots); and **FDV ÷ market cap**, the unlock overhang, which is why nothing is held for days. Community sentiment on that page is worth nothing.
- **Trend lines / tunnel:** standard construction, drawn on the **1D** chart, alongside the SMC labels rather than instead of them. They are the only subjective tool in the stack — keep them **subordinate**: if a trend line and the EMA 155 rule disagree, EMA 155 wins, and a broken trend line is not a BOS.
- **Coinglass:** liquidation heatmap. **12h is the working view** (session default); 24h for a longer read, 1w for context only. **Model 1** is the scalping view, **Model 2** the longer one — a band hottest in **both** is the one that gets hunted. Pick the **Bybit** pair, not Binance. Yellow = the cluster, blue-black = empty. Tap a band for its size in dollars; rank within a model, compare models on position only.
- **Account:** isolated margin · one-way mode · TP triggers on Last, SL on Mark · Order by Value.
- **Access:** Bybit is blocked by MCMC in Malaysia. VPN on before the session starts, and check it is still up before placing an order.

## 1. Scan the market (Diagnose)
1. Heatmap: mostly green → long bias; mostly red → short bias; mixed → no trades today.
2. Hot sectors → leading coin in each → Top Movers (24h, and the 15m tabs). Volatility and volume are the must; +4% in two hours is too slow. A gainer is a candidate, never a trade. **Weekends: volume dries up; widen the search or stay flat.**
3. Screener per candidate, scored out of 4: **EMA dominant direction** across 1D, 4H, 1H, 15m, 5m, 1m (one dissenting frame does not veto) · OI line tilting up at the right-hand end · funding **sign** counter to your side (negative for a long, positive for a short) · **depth lighter on your own side** (bid side thinner for a long, ask side thinner for a short). **4/4 → full size. 3/4 → 50–75% size, tighter stop. Below 3 in one direction → no trade** for a beginner; session: intermediates may take 2/4, advanced 1/4, at their own risk. Mixed timeframes → reduce size; all disagree → skip the coin. Funding settles 8 AM, 4 PM, midnight MYT; the sign is what scores, the size is what the hold costs.
4. **Exception, day-1 / day-2 listings only:** the multi-timeframe EMA check is impossible (the daily has two candles) and funding and depth are uninformative on a new book, so the screen is **EMA direction + OI direction only** — OI on Bybit's OI Data tab at 5m. Session: "that's good enough." It expires as soon as the coin has real higher-timeframe history. **It does not apply to any coin with history**, and a 2/4 screen is his advanced tier: beginners skip newborn coins instead.
5. **News-driven pump — four questions before you take it** (ZETA, 23 Mar 2025): **who pumps** (exchange volume breakdown; one venue above ~50% is that venue's retail flow — real while it is awake, gone when it sleeps) · **what news, and when** · **where is the liquidity**, both sides, both heatmap models · **how late am I** relative to the call. A call is a limit-on-retracement instruction, never "buy now".
6. Sentiment gauge is a clue, not a signal.

## 2. Set direction (Diagnose)
1. **EMA 155 rule, read on the Heikin-Ashi chart:** three consecutive candles with the body on one side of EMA 155 and no wick on the other side. Above → long only; below → short only. Nothing else sets direction. Order prices still come from real candles.
2. Heikin-Ashi run with no trend-side wicks confirms. Dojis or small-body clusters → **wait two to three candles**; same colour after = congestion, trend continues; colour change = the turn.
3. **EMA fan width is trend strength**: bunched lines are a weak signal, a spread fan is confirmed. Lines repeatedly crossing back and forth = ranging → skip.
   **Retracement test, once you are in**, in order of severity: EMA 9/25/55 tangling with each other while all three stay **above** EMA 155 is noise, hold · three full-body candles past EMA 155 is the **warning** that direction has gone · the fan **fully inverted** (255 > 155 > 55 > 25 > 9) is the confirmation — "cut loss or exit". ("EMA 155" is the fan's pivot; on another EMA set, the equivalent line.)
4. Donchian ribbon (period 20) solid in the same colour confirms. Mixed → skip. **The ribbon colour is a BOS proxy**: a pullback that is only a CHoCH leaves the colour alone; a CHoCH followed by a BOS flips it. Colour holds = retracement, colour flips = the structure broke. Sensitive on 1m.
5. **SMC sequence, the one entry trigger it gives:** equal lows at a strong low → CHoCH → BOS = long ("pump like crazy"). Equal highs → CHoCH → BOS = short ("dump very hard"). All three, in that order. The sweep itself is the abnormal-volume bar with the long wick.
6. Seahorse (vertical move done, flat beak, EMAs converging) → stay out.
7. Hockey stick (slow decline, sharp V, vertical blade): enter only on the golden cross *with* the EMA 155 three-candle rule. Never buy the blade.

## 3. Sniper entry (Diagnose, SPE)
1. TradingView: nearest demand zone below (long) or supply zone above (short), and any FVG. Take the near edge.
2. Bybit: **EMA 9** is the first target; if the zone edge sits deeper, the EMA closest to the edge. That is the price. **Any of the five lines is parkable** — EMA 9 fills most often, EMA 155 is the deep one with the pivot behind it, EMA 255 is "the last guard". Trail the order up the line as the trend advances.
3. Rest a limit order there. Re-place it if the EMA moves. **Limit is the default; a market order needs a reason** ("don't enter as a market order unless some critical condition"). Never market-buy the running candle.
4. Correlated alts making the same move at the same minute are one trade. Size the total.

## 4. Size and stop (Dose)
1. Isolated margin. Leverage 5× to 10×.
2. Margin per trade: $20 to learn; then 1% of wallet; never above 10%. Bigger wallet, smaller trade. **Loss at the stop never above 1–2% of account equity**, whatever the confluence score.
3. **Check the heatmap before you place the stop.** A cluster just beyond it will be swept before the move you want — move the stop past it or lower the leverage. A cluster is a **magnet, never support**: price is drawn into it and the forced orders accelerate through it.
   **KL to Penang:** the biggest band is the destination, but a smaller band on the *other* side is a detour often taken first — "it depends on the money maker". A sweep into the near cluster is the route, not a change of destination. Size the stop for the detour.
   **And re-read it before any re-entry.** Once price has reached a cluster, that cluster is **consumed** and the next destination is the one on the other side — the direction flips with it. "Finish liquidity here already ... then they have to come down to hunt this." A double top is the symptom; the emptied band is the cause.
4. Stop as ROI on margin by tier: beginner 5–20%, intermediate 20–50%, advanced 50%+. Convert to price; it must sit beyond the structural level (far edge of the zone, or the heel low). If it does not, **lower the leverage** until it does (session-confirmed). Never move the level, never widen the tier.
5. Write the money at risk in USDT before entry.

## 5. Exit plan, both ways (Discharge)
1. TP first. Wick Tracker is a Bybit TP trigger at a level a wick will reach: **slightly above** the prior wick high (a sweep aims at the stops resting beyond it), the supply-zone bottom, **the nearest large liquidation cluster** (rank them by the dollar figure, not the brightness), or 50% ROI raised to 55–60% for fees. Trigger on **Last**; set it inside the wick you expect, above the wick already made.
   **Two regimes, decided by the fan.** Fan widening with no two lines crossing → no fixed target is needed; ride it on the climax rule and the EMA cross, with the Wick Tracker resting only as the unattended backstop. Fan flat, bunched or crossing → set the target and take it. The stop is mechanical either way; only the target is conditional.
2. SL from step 4, trigger on Mark, **resting before the entry fills**. Both orders in before you look away.
3. Climax exit: a volume bar **above both VOLMA lines** ("abnormal", session-defined — no multiple) + the MACD histogram at its **mountain peak**, confirmed when the next bar prints shorter — **on Bybit that next bar is drawn hollow** → close 75%. Move the runner's SL to entry.
   Abnormal volume with a **long wick** is a liquidity sweep, not a move; with a **full body** it is real. Colour gives the side: red selling, green buying.
4. **MACD is two shapes.** Iceberg dip (deepest red bar) times the entry; mountain peak (tallest green) is the exit. Short reverses them. Miss the peak and you give back half at the zero line, all of it back at your entry, then it is a loss. If you cannot sit through a give-back, trade dip-to-peak and stop there.
5. Runner: Hunting SL locks a rising ROI. EMA 9 crossing back through EMA 25 is the backstop **for the runner only** — on a full position the fast lines crossing each other is noise while all three sit above EMA 155.
6. Stop hit = the plan worked. Take it.
7. **Take the written level — not sooner, not never.** ZETA is the course's own proof: the Wick Tracker at 2.8530 fired 1.5 cents under the high, and the coin was at 0.045 two years later. "Never exit will liquidate."

## 6. After the close (Follow up)
1. Sweep realised profit from Derivatives to Funding.
2. Close and go. Next coin. Never re-enter the same beak. **Nothing is held past 24 hours** (session: "minutes, hours, not more than days").
3. Stop at the daily target or ten trades, whichever first. Rest.
4. Log it in the journal: which D, which rule, what you would change, **and whether price came back and challenged your entry** — his test for whether it was a sniper entry at all. Thirty trades before you believe any number.

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
- Entering on a chat call without the chart check. "If you don't know the setup, don't take the shot."
- Shorting a pump that is still running. "No one can tell where the pump will get."
- Holding for days. This is not swing trading.
- New listings beyond a few days.
- Adding to a losing position to push liquidation away. Session: "against the money" means exactly this; a 100 loss becomes 500.
- Blaming mindset before checking which D you skipped.
