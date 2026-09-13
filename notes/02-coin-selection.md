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

Not a tool in the software sense. It is a navigation path in the Bybit app:

1. Bottom menu: **Markets**
2. Top menu: **Opportunities**

The Opportunities screen is where the Hot, Gainers, New and Leaderboard tabs from section 1.2 live. So the "basic tool" is: open Bybit's own ranked lists and pick from the coins already moving on USDT perpetuals.

This confirms the exchange (Bybit) and the product (USDT perpetuals) for the whole course.

## 5. Advance tool: MMT Coin Trend Screener

_Not yet captured._

## 6. Hockey stick pattern

_Not yet captured._

## Timeframe tension in this module

The four-phase diagram is built on a **200-period moving average** and describes ranges lasting **six months**. That is a daily or weekly chart. The scalping definition in Module 1 says holding periods of seconds to minutes. The two only reconcile if the course uses the higher timeframe to pick the coin and its direction (this module) and a lower timeframe to time the entry (Modules 3 and 4). The slides do not say this explicitly. Confirm when the indicator modules arrive.

## Open questions

- What is the course's definition of a strong coin versus a shit coin, so that a coin on neither list can be classified?
- Does the Coin Trend Screener replace the manual Bybit Opportunities scan, or sit on top of it?
- Is there a volume threshold, or is "high volume" satisfied by appearing on the Gainers or Hot tab?
- How are "new coins" handled, given the thin history for any 200 MA or EMA calculation?
- Which timeframe is the trend phase judged on, and which timeframe is the entry taken on?
