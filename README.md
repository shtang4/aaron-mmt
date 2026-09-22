# Momentum Mastery Trading (MMT) — Course Notes

Personal study notes for **Momentum Mastery Trading** by Dr. Aaron MMT.
Source material: course slides (Copyright 2026, Dr. Aaron MMT). Not financial advice.

## Notes index

| # | File | Topic |
|---|------|-------|
| 0 | [notes/00-mindset-and-outline.md](notes/00-mindset-and-outline.md) | Mindset pyramid, learning outcomes, full course outline |
| 1 | [notes/01-what-is-scalping.md](notes/01-what-is-scalping.md) | Scalping definition, MMT 3D framework |
| 2 | [notes/02-coin-selection.md](notes/02-coin-selection.md) | Coin selection, Trend is King, Potential Coin Finder, Coin Trend Screener, hockey stick pattern |
| 3 | [notes/03-entry-direction.md](notes/03-entry-direction.md) | Heikin-Ashi, 3 main indicators, SMC, new indicators, trend lines / S&R / tunnel, seahorse pattern |
| 4 | [notes/04-sniper-entry-exit.md](notes/04-sniper-entry-exit.md) | MMT New TP, Sniper Price Entry (SPE), Wick Tracker |
| 5 | [notes/05-risk-and-hedging.md](notes/05-risk-and-hedging.md) | Risk management, MMT Hedging, MMT Golden Rules |
| 6 | [notes/06-case-studies.md](notes/06-case-studies.md) | Every case study in the course, indexed: SOMI, BTC, 10000LADYS, MAVIA, A8, Jane, ZETA, RAD, RAVE, BMT, GMX, PEOPLE, AERGO, the skipped-D triptych, and the Q&A |
| 7 | [notes/07-handouts.md](notes/07-handouts.md) | The three PDF handouts: screener cheat sheet, risk checklist, trade call guide. Scorecard, funding thresholds, stop and 1–2% rules; where they contradict the slides. |
| 8 | [notes/08-transcript.md](notes/08-transcript.md) | What the spoken session adds or changes, filed by module as transcript parts arrive. |
| 99 | [notes/99-open-questions.md](notes/99-open-questions.md) | Every question the deck leaves open, grouped by what it would change |

All six modules are captured from the slides, and the spoken session is transcribed in file 8 (parts 1–30). **Three spoken sections are still outstanding:** the GMX and PEOPLE hedging case studies (`05 §4.8`, `§4.11`), the AERGO "trade scam coin, no BTC correlation" section (`06 §12`), and two short Module 5 framing slides (`05 §4.9`, `§4.12`). Questions no transcript can answer — things never said in six modules — are in file 99.

## Source slides

`slides/mmt-part1.pdf` — the course deck as supplied by the author, pages 1–80 of 259. Page images only, no text layer, so it is read with a PDF page renderer rather than by search. Notes cite it as `slides/mmt-part1.pdf p.NN`, which makes every arithmetic claim in this repository re-checkable against the original slide. Remaining parts to be added.

## Tools

| File | What it does |
|------|-------------|
| [tools/sop.html](tools/sop.html) · [notes/SOP.md](notes/SOP.md) | One-page SOP. The whole method as numbered steps, the formulas, and the never list. Printable on one A4 sheet. |
| [tools/trade-journal.html](tools/trade-journal.html) | Trade journal. One entry per closed trade with the Diagnose, Dose and Discharge fields and the rule broken, if any. Computes win rate, expectancy in USDT and R, profit factor, drawdown, an equity curve, and a breakdown by setup and by clean versus rule-broken. Published as an artifact with a database so entries persist and can be read back from a Claude session; opened as a file it keeps entries in the browser only. |
| [tools/pretrade-checklist.html](tools/pretrade-checklist.html) | Pre-trade check. Walks Diagnose, Dose, Discharge; computes stop, TP net of fees, reward-to-risk, runner and Hunting SL; refuses plans that break rules the course itself states; emits the written plan. Has a "Fetch from Bybit" panel (public endpoints, no key) that fills last price, the five EMAs on Heikin-Ashi closes, the EMA 155 three-candle check, funding, open interest and depth. The fetch only works when the file is opened from your own computer; the hosted artifact cannot reach Bybit. Confirmed working from Malaysia with a VPN on, since Bybit is blocked by MCMC. |

## Conventions

- One file per course module, numbered in course order.
- Chinese terms from the slides are kept next to the English (e.g. *Trend is King (趋势为王)*) so the notes match the original vocabulary.
- Tool names (Potential Coin Finder, Coin Trend Screener, SPE, Wick Tracker, MMT Hedging) are proper nouns from the course and are written as such.
