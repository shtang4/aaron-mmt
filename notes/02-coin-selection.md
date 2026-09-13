# 02 — How To Select Which Coin To Trade

Source: Module 2 slides, Momentum Mastery Trading (MMT), Dr. Aaron MMT, 2026.

Module contents (from the section title slide):

- How to select a coin? (如何选择一个加密货币？)
- Trend is King (趋势为王)
- Basic tool: Potential Coin Finder
- Advance tool: MMT Coin Trend Screener (MMT加密货币趋势筛选器)

The course outline also lists a **hockey stick pattern** under this module; it is absent from the section title slide.

## 1. How to select a coin: three criteria

| # | Criterion | Slide detail |
|---|-----------|--------------|
| 1 | **Volatility** | Evaluate the coin's historical volatility. Higher volatility gives more opportunities but carries higher risk. Weigh it against your risk tolerance and strategy. |
| 2 | **High volume trade** (高成交量交易) | Illustrated with an exchange app's **Gainers** tab on USDT perpetuals, sorted by 24-hour change. |
| 3 | **Coin category** | "Choose strong coin, meme coins, shit coins, new coins." Two lists are given, one of strong coins and one of shit coins. |

### 1.1 Volatility

Slide text, verbatim: "Evaluate the historical volatility of the coin. Higher volatility can provide trading opportunities but also carries higher risks. Consider your risk tolerance and trading strategy when assessing the coin's volatility."

No measure is given (no ATR, no percentage range, no lookback). This is a principle, not a screen.

### 1.2 High volume trade

The slide's example is the **Gainers** list on an exchange's USDT-Perp market (tabs shown: Hot, Gainers, New, Leaderboard; markets: Spot, USDT-Perp, USDC-Perp, USDC Futures, Leverage). Pairs shown, top to bottom, with 24H change:

| Pair | Price | 24H change |
|------|-------|------------|
| 10000LADYSUSDT | 0.0004385 | +20.97% |
| FITFIUSDT | 0.003545 | +18.17% |
| FXSUSDT | 5.3175 | +13.56% |
| SSVUSDT | 17.910 | +12.46% |
| BLURUSDT | 0.3610 | +10.80% |
| ORDIUSDT | 6.412 | +10.12% |
| ICXUSDT | 0.1906 | +9.98% |
| 1000BONKUSDT | 0.000319 | +9.25% |

What the slide is actually demonstrating: the coins to look at are the ones **already moving** in the last 24 hours on the perpetuals market. The heading says volume; the screen shown is sorted by price change, not volume. Read the criterion as "in play today" rather than as a volume threshold. The two usually coincide on a gainers list, but not always: a thin coin can post a +20% day on little volume.

Practical inference: the course trades **USDT perpetual futures**, since that is the tab selected. That is where shorting and leverage are available, which the next slide assumes.

### 1.3 Coin category: strong coins vs shit coins

Two lists, transcribed verbatim from the slide.

**"What are the strong coins to avoid shorting?"**

| # | Coin | # | Coin |
|---|------|---|------|
| 1 | Bitcoin (BTC) | 15 | Avalanche (AVAX) |
| 2 | Ethereum (ETH) | 16 | DAI (DAI) |
| 3 | Tether (USDT) | 17 | Chainlink (LINK) |
| 4 | BNB (BNB) | 18 | Cosmos (ATOM) |
| 5 | USD Coin (USDC) | 19 | Uniswap (UNI) |
| 6 | Ripple (XRP) | 20 | Lido DAO (LDO) |
| 7 | Cardano (ADA) | 21 | Arbitrum (ARB) |
| 8 | Polygon (MATIC) | 22 | Aave (AAVE) |
| 9 | Solana (SOL) | 23 | PAXG (PAXG) |
| 10 | Polkadot (DOT) | 24 | PEPE (PEPE) |
| 11 | Litecoin (LTC) | 25 | Floki Inu (FLOKI) |
| 12 | Binance (BUSD) | 26 | Optimism (OP) |
| 13 | Shiba Inu (SHIB) | 27 | Apecoin (APE) |
| 14 | Tron (TRX) | 28 | Sandbox (SAND) |

**"What are the best shit coins to short?"**

| # | Coin | # | Coin |
|---|------|---|------|
| 1 | CTC | 18 | ONT |
| 2 | CEEK | 19 | PEOPLE |
| 3 | TOMO | 20 | CVC |
| 4 | ANT | 21 | LRC |
| 5 | IOTX | 22 | BAND |
| 6 | BNX | 23 | JASMY |
| 7 | GTC | 24 | C98 |
| 8 | CVX | 25 | SWEAT |
| 9 | NEO | 26 | SSV |
| 10 | XEM | 27 | ALICE |
| 11 | CTK | 28 | RPL |
| 12 | SXP | 29 | BEL |
| 13 | OCEAN | 30 | OMG |
| 14 | CELO | 31 | LINA |
| 15 | LUNC | 32 | COCOS |
| 16 | LUNA | 33 | LINA |
| 17 | EGLD | 34 | GPT |

(The slide numbers the right column of the shit-coin list starting at 8, which is a typo; it continues from 18.)

**The rule the two lists encode:** coin category sets a **directional bias**.

- Strong coins: long-biased. Do not short them.
- Shit coins: short-biased. These are the candidates when the Diagnose step (Module 1) gives a death cross.

That is the useful content. The specific names are less useful, for reasons below.

## 2. Problems with the lists as given

- **Stablecoins on the "strong coin" list.** USDT, USDC, DAI, BUSD and PAXG (gold-backed) do not trend. They cannot be scalped and "avoid shorting" is vacuous for them. Their presence says the list was assembled by market cap, not by tradability.
- **The lists are dated.** BUSD was wound down in 2023 and 2024. MATIC migrated to POL. LUNA and LUNC are on the short list, which places the list after the May 2022 collapse. Several shit-coin names may no longer be listed on perpetuals. Treat both lists as a **2023 snapshot**, and regenerate them from the current market before use.
- **No definition of "strong" or "shit".** Market cap, exchange tier, project fundamentals and age are all plausible criteria, and none is stated. Without a definition you cannot classify a coin that is on neither list, which is most coins.
- **The heading promises four categories** (strong, meme, shit, new) and the slide delivers two. Meme coins are scattered across both lists (PEPE, FLOKI, SHIB on strong; none on the short side), so "meme" is not itself a directional category here. "New coins" get no treatment at all on this slide; the Gainers screenshot's **New** tab is presumably where they come from.

## 3. Trend is King (趋势为王)

### 3.1 Four market phases

The slide reuses a public diagram ("Four Market Phases Every Trader Must Know", credited to tradingwithrayner.com). Phases in order:

| # | Phase | What it looks like | 200 MA |
|---|-------|-------------------|--------|
| 1 | **Accumulation** | Range after a 6-month decline. Long consolidation. | Flattening |
| 2 | **Advancing** | Breakout from the accumulation range. Forms an uptrend. | Price above 200 MA |
| 3 | **Distribution** | Range after a 6-month advance. Long consolidation. | Flattening |
| 4 | **Declining** | Breakdown from distribution. "Where traders become long-term investors." | Price below 200 MA |

The right half of the slide shows a plain uptrend and downtrend candlestick example.

Reading: only phases 2 and 4 are tradeable with a trend method. Phases 1 and 3 are ranges, and the Diagnose step (Module 1) will produce whipsaw EMA crosses inside them. "Trend is King" therefore means **do not trade the coin at all** unless it is in phase 2 or 4. This is the Skip decision from the course's outcome 3.

Phase 4's caption, "where traders become long-term investors", is a warning about refusing to take the stop and holding a losing position. It connects back to the Discharge rule: stop below EMA 50, structural, not emotional.

### 3.2 Trend structure

Second slide, two parts:

- A chart showing the sequence uptrend, downtrend, sideways, uptrend, downtrend, with trend lines drawn under the uptrends and over the downtrends, and a horizontal box around the sideways range.
- A schematic definition:

| Structure | Definition |
|-----------|------------|
| **Uptrend** | Higher highs and higher lows |
| **Sideways / trading range** | Highs and lows at roughly the same level |
| **Downtrend** | Lower highs and lower lows |

This is the swing-structure definition of trend, independent of any indicator. Together with the EMA cross from Module 1, the course now has two trend tests: structure (HH/HL or LH/LL) and momentum (EMA cross). A valid direction should pass both.

### 3.3 Two maxims

**"We can go against the Market, but not against Money."** (我们可以跟市场做对，但不能跟金钱做对。)

The slide gives no gloss. Most consistent reading with the surrounding slides: "the market" is the crowd's opinion or sentiment, "money" is where volume is actually flowing. You may take a view the crowd disagrees with, but never trade against the direction volume is pushing. That ties the maxim to criterion 2 (high volume) and to the trend phases above. Treat this interpretation as an inference, not the slide's words.

**"Regardless of whether it is a black cat or a white cat, a cat that catches mice is a good Maneki cat."** (不管黑猫白猫，能捉到老鼠就是好的招财猫)

Deng Xiaoping's pragmatism line with a Maneki-neko (lucky cat) substituted. Applied here: it does not matter whether the coin is strong or shit, or whether the trade is long or short. A coin that produces a clean trend move is a good coin. The colouring on the slide (black cat green, white cat red) maps to long and short.

## 4. Basic tool: Potential Coins Finder (潜在币种寻找器)

Not a tool in the software sense. It is a navigation path in the Bybit app, and a set of screens under it:

1. Bottom menu: **Markets**
2. Top menu: **Opportunities**

The Opportunities screen (tabs: Hot, New, Gainers, Turnover, Opportunities) contains four panels the course walks through: **Market Sentiment**, **Hot Sectors**, **Heatmap**, and **Top Movers**. The "Steps to find coin to trade" slides use each in turn.

This confirms the exchange (Bybit) and the product (USDT perpetuals) for the whole course.

### 4.1 Step: Market Sentiment. "Use sentiment as a clue, not a signal."

The Market Sentiment panel shows a Fear and Greed gauge (screenshot: 71, Greed), the BTC long/short ratio (68.0 / 32.0), a gainers-vs-losers bar, a "How do you feel about the market today?" poll, and a TrendMiner card of the coin with the most KOL (key opinion leader) mentions in the last hour (screenshot: SOL, 100% bullish).

Slide's rules, verbatim:

- Greed ≠ auto long. Confirm first.
- Greed sentiment ≠ blindly go long.
- Greed = bullish bias, not buy signal.

And the reason: greed also means price may already be extended, late buyers may get trapped, and a pullback or reversal is possible.

So sentiment sets **bias** only. It has the same standing as the coin lists in section 1.3: it tells you which direction to look, not when to enter.

### 4.2 Step: Hot Sectors. "Follow the money flow if you want to make the money."

Hot Sectors panel: sector cards with 24H change and the leading coin in each (screenshot: Zero Knowledge +8.07% led by ZEN, DCG Portfolio +6.71%, Privacy Coins +6.39% led by SCRT, Layer 1 +6.16% led by SEI, a16z Portfolio +6.12% led by AR, NFT +6.03% led by CHZ).

Slide text: "Hot sectors = where the volume, hype, attention are right now." Procedure, "Spot active narrative":

1. Top-performing sectors (highest percentage gain).
2. Leading coins in each sector.
3. Short-term momentum = possible trade setups.

"Smart traders watch for fast-moving plays."

This is the operational meaning of the "not against Money" maxim in section 3.3: money flow is read off the sector ranking. Sector first, then the leader within it.

### 4.3 Step: Heatmap. "Market Sentiment Scanning."

The Heatmap panel tiles the USDT-perp market by size, green for up and red for down, with 24H change. Two screenshots are contrasted: one almost entirely green (BTC +3.32%, ETH +4.33%, SOL +5.38%, most alts up), one mixed (BTC +1.57% but ETH, SOL, XRP, DOGE red, a few alts strongly green).

Classification rule:

| Heatmap | Market sentiment |
|---------|-----------------|
| Mostly green | Bullish |
| Mostly red | Bearish |
| Green and red distributed evenly | Ranging |

This is the intraday version of the four-phase diagram in section 3.1. "Ranging" here is the Skip condition: when the heatmap is mixed, the market has no direction to follow, and individual green tiles are idiosyncratic pumps rather than money flow.

### 4.4 Step: Top Movers, and the SOMI case study

Top Movers panel (tabs: All, 15m Gainers, 15m Losers, 24h Gainers, Breakout). The case study walks Heatmap → Opportunities → Top Movers and lands on **SOMI**, showing +46.56% on the heatmap tile and +47.39% as a 24h gainer, top of the list by a wide margin (next best CORN +16.29%, DRIFT +20.76%).

Stated conclusion: a 24H top gainer is a **potential coin to further analyse**. Not a trade.

The slide also shows a BTCC share card: SOMIUSDT, "Open Long Perp 50x", +554.50%, average open 0.9901, latest 1.0999, with an invitation code. Two things to notice:

- The arithmetic checks: 0.9901 → 1.0999 is +11.1% on price, and 11.1% × 50 leverage = 555%. The headline number is the leverage, not the trade.
- The card is from BTCC, not Bybit, and carries a referral code. It is promotional material inside the lesson. The scanning method is Bybit's; the result card is a different exchange's marketing graphic. Treat the +554% as an illustration of leverage, not as evidence the method produced it.

Note that the 15m Gainers and 15m Losers tabs exist on the Top Movers screen. They are the scalping-timeframe equivalent of the 24h list, and the slides do not mention them. Worth testing whether they are the better feed for a minutes-long holding period.

### 4.5 Step: Confirm first. "Volume and narrative drive opportunity."

Warnings, verbatim:

- Sector pumping ≠ safe to enter now.
- Hot narrative doesn't mean good entry. Confirm first.

How to confirm:

| Method | Slide detail |
|--------|-------------|
| Fundamental analysis (FA) | Check background and news |
| Technical analysis (TA) | Analyse the chart |
| Trading strategy | Wait for a retrace, a breakout, or confirmation before trading |

The third row is the bridge to Modules 3 and 4. "Wait for retrace, breakout, or confirmation" is what the Sniper Price Entry is presumably formalising.

### 4.6 The workflow, assembled

Putting the five steps in order:

1. **Sentiment gauge**: read the Fear and Greed value and long/short ratio. Sets bias only.
2. **Heatmap**: classify the day as bullish, bearish, or ranging. Ranging means skip.
3. **Hot Sectors**: find the top sectors and the leading coin in each. This is where money is flowing.
4. **Top Movers**: cross-check the leaders against the 24h (or 15m) gainers list. A top gainer is a candidate, not a trade.
5. **Confirm**: check news, read the chart, and wait for a retrace or breakout. Then hand off to the Diagnose step (Module 1) and the entry modules.

Every step except the last is a Bybit screen. The course's contribution is the ordering and the repeated instruction that none of these screens is an entry signal.

## 5. Advance tool: MMT Coin Trend Screener (MMT加密货币趋势筛选器)

A four-check confluence table run on a candidate coin after the Bybit scan. Order on the flow slide: **EMA (all TF) → OI Data → Contract (FR): counter/opposite → Depth (choose the lower volume)**.

The worked example on the second slide, for a long:

| # | Indicator | Trend reading | Signal |
|---|-----------|---------------|--------|
| 1 | EMA, checked on every timeframe: Day → 1 Hour → 4 Hours → 15 Mins → 5 Mins → 1 Min | Up | Long |
| 2 | OI (open interest) data | Up | Long |
| 3 | Contract funding rate | Negative | Long ("no funding rate", i.e. longs do not pay) |
| 4 | Depth volume | Low | Long |
| | **Overall confluence** | **4/4** | **Long** |

Slide notes, verbatim:

- Use additional complementary indicator to enhance accuracy and entry.
- Some trade might not fulfil all indicators.
- Risk management for manipulation (pump and dump, news, black swan event).
- Vice versa for short.

### 5.1 What each check means

**1. EMA on all timeframes.** The EMA direction (from the Module 1 golden/death cross) must agree from the daily chart down to the 1-minute chart. This is the multi-timeframe alignment the earlier slides implied but never stated. It also settles the scalping-versus-daily tension: direction is confirmed top-down, and the 1m and 5m charts are where the entry is timed.

The slide lists the order as Day → 1H → 4H → 15m → 5m → 1m. The 1H and 4H are out of sequence; the intended order is almost certainly Day → 4H → 1H → 15m → 5m → 1m.

**2. Open interest.** Rising OI with rising price means new money is entering longs, which confirms the uptrend. "Vice versa for short" is loose here: for a short, the confirming pattern is OI rising while price falls (new shorts entering), not OI falling. Falling OI in either direction means positions are closing, which is a weakening trend, not a signal.

**3. Funding rate, counter or opposite.** The flow slide says "counter/opposite" and the table says negative funding = long. Read together: trade against the funding rate. Negative funding means the crowd is net short and shorts pay longs. Going long means you are paid to hold, and you are positioned against a crowded side that can be squeezed. For a short, look for positive funding.

**4. Depth, "choose the lower volume".** The least explained check. Depth is the order book. The reading most consistent with the other three checks: compare the bid-side and ask-side depth, and trade in the direction where the book is thinner, because price meets less resistance moving that way. For a long, a thin ask side (low sell-wall volume) is the confirming condition. This is an inference; the slide does not define which side's volume is being compared.

### 5.2 What the screener does and does not do

- It is the only place in Module 2 where a coin gets a **rule-based** direction rather than a list-based or sentiment-based bias. This is the real tool in the module.
- It **does not** set a threshold. "Some trade might not fulfil all indicators" means 4/4 is not required, and 3/4 or 2/4 is left to judgement. Ask what the minimum confluence is.
- It **does not** replace the Bybit Opportunities scan. The scan produces candidates; the screener grades them. The scan is broad and free, the screener is per coin and manual.
- The manipulation warning is the course acknowledging that all four checks can be gamed on a thin coin. That points back to the volume criterion in section 1: run the screener on liquid coins only.

## 6. Hockey stick pattern

_Listed in the course outline under this module. Not on the section title slide and not yet seen. May be covered elsewhere or dropped._

## Timeframe: resolved by the screener

The four-phase diagram in section 3.1 is daily. The scalping definition in Module 1 is minutes. The screener's EMA check runs on every timeframe from daily to 1 minute, which makes the method explicitly multi-timeframe: **direction is set from the daily down, entry is timed on 1m to 15m.** A coin whose EMAs disagree across timeframes fails check 1.

## Open questions

- What is the course's definition of a strong coin versus a shit coin, so that a coin on neither list can be classified?
- What is the minimum confluence on the screener: 4/4, 3/4, or judgement?
- Module 6 section 1 has a worked example of check 1 (RAD, four timeframes, price above all five EMAs on each).
- In the depth check, which side of the order book is "the lower volume" compared against?
- Are the 15m Gainers / 15m Losers tabs used anywhere in the course, or only the 24h list?
- Where does the "wait for retrace, breakout, or confirmation" instruction get made precise: Module 3 (direction) or Module 4 (SPE)?
- Does the hockey stick pattern appear anywhere in the delivered slides?
