# 🏀 NBA Opening & Closing Odds — Pinnacle + 7 World Books (2008–2026)

**20 games — every season from 2008-09, every stage: regular season, play-in, playoffs, NBA Finals and the first NBA Cup final**

Most NBA odds archives give you the US books, or one closing number per game.

The full dataset puts **up to 8 books side by side on each game, in decimal odds**: Pinnacle, Bet365, William Hill,
Bwin, Betway, Betfair Exchange, SBOBET and 1xBet. Moneyline, spread and total, plus the 1X2 in regular time at Bwin,
Betway and 1xBet: **the opening and the closing price, each with the time it was recorded**.

→ **[Get the full archive](https://sportsdataolivier.gumroad.com/l/oeuoto?utm_source=github&utm_medium=readme&utm_campaign=nba_world&utm_content=hero)** — 23,212 games, 2008-09 to 31 October 2026 · also on [Whop](https://whop.com/oliviersportsdata/nba-opening-closing-odds-pinnacle-7-world-books-2008-2026/?utm_source=github&utm_medium=readme&utm_campaign=nba_world&utm_content=whop_hero)

This sample is cut from the full file: the same 182 columns, the rows copied byte for byte, at about 0.1% scale.

---

## One game, every book

Pistons at Hawks, 20 January 2021, moneyline. All 8 books opened and closed it, and every one of them closed the
Hawks longer than it opened them. The game went to overtime, 123-115 for the Hawks: the 1X2 draw, regular time only,
won at Bwin (10.5), Betway (13.25) and 1xBet (18).

| Book | Open, Hawks / Pistons | Close, Hawks / Pistons |
|---|---|---|
| Pinnacle | 1.4132 / 3.11 | 1.5556 / 2.61 |
| Bet365 | 1.4 / 3.1 | 1.55 / 2.6 |
| William Hill | 1.4 / 3.1 | 1.54 / 2.65 |
| Bwin | 1.36 / 3.2 | 1.53 / 2.55 |
| Betway | 1.44 / 2.8 | 1.54 / 2.55 |
| Betfair Exchange | 1.47 / 2.92 | 1.55 / 2.62 |
| SBOBET | 1.38 / 2.92 | 1.49 / 2.58 |
| 1xBet | 1.48 / 2.96 | 1.55 / 2.71 |

---

## What's in this sample

| | |
|---|---|
| Games | 20 — one per season from 2008-09 to 2025-26, two in 2026-27 |
| Stages | 9 regular season · 2 play-in · 8 playoffs (7 NBA Finals) · 1 NBA Cup final |
| Overtime | 3 games |
| Prices | 1,043 |
| Books | 8 — Pinnacle, Bet365, William Hill, Bwin, Betway, Betfair Exchange, SBOBET, 1xBet |
| Columns | 182 |
| File | `NBA_World_Opening_Closing_Odds_2008-2026_SAMPLE.csv`, plus the README of the full product |

| Date (ET) | Game | Stage | Final, away–home | Books, closing / opening ML |
|---|---|---|---|---:|
| 17 Feb 2009 | Timberwolves @ Wizards | Regular Season | 103–111 | 4 / 4 |
| 3 Jun 2010 | Celtics @ Lakers | Playoffs | 89–102 | 4 / 4 |
| 7 Mar 2011 | Trail Blazers @ Magic | Regular Season | 89–85 | 5 / 4 |
| 25 Dec 2011 | Bulls @ Lakers | Regular Season | 88–87 | 5 / 3 |
| 20 Jun 2013 | Spurs @ Heat | Playoffs | 88–95 | 5 / 4 |
| 29 Apr 2014 | Grizzlies @ Thunder | Playoffs | 100–99 OT | 5 / 5 |
| 28 Oct 2014 | Mavericks @ Spurs | Regular Season | 100–101 | 4 / 3 |
| 19 Jun 2016 | Cavaliers @ Warriors | Playoffs | 93–89 | 5 / 4 |
| 24 Feb 2017 | Jazz @ Bucks | Regular Season | 109–95 | 6 / 6 |
| 31 May 2018 | Cavaliers @ Warriors | Playoffs | 114–124 OT | 6 / 2 |
| 16 Oct 2018 | 76ers @ Celtics | Regular Season | 87–105 | 7 / 2 |
| 15 Aug 2020 | Grizzlies @ Trail Blazers | Play-In | 122–126 | 8 / 7 |
| 20 Jan 2021 | Pistons @ Hawks | Regular Season | 115–123 OT | 8 / 8 |
| 15 Apr 2022 | Hawks @ Cavaliers | Play-In | 107–101 | 7 / 6 |
| 12 Jun 2023 | Heat @ Nuggets | Playoffs | 89–94 | 7 / 6 |
| 9 Dec 2023 | Pacers @ Lakers | NBA Cup Final | 109–123 | 1 / 1 |
| 22 Jun 2025 | Pacers @ Thunder | Playoffs | 91–103 | 7 / 6 |
| 3 Jun 2026 | Knicks @ Spurs | Playoffs | 105–95 | 5 / 5 |
| 23 Oct 2026 | Raptors @ Wizards | Regular Season | 112–102 | 5 / 5 |
| 31 Oct 2026 | Thunder @ Rockets | Regular Season | 98–119 | 7 / 6 |

*Books* counts, out of 8, the books with a closing / opening moneyline for that game. Why each game is
here, game by game: `sample/README.md`.

---

## In this repository

| File | Content |
|---|---|
| `sample/NBA_World_Opening_Closing_Odds_2008-2026_SAMPLE.csv` | the 20 games, 182 columns |
| `sample/README.md` | why each game is here, then the README of the full product |
| `matchup_stats_sample/` | the same 20 games in NBA Matchup & Stats: game sheets, team and player box scores, inactive players (4 CSV + README) |
| `NBA_World_Verify_Before_You_Buy.ipynb` | the figures of the listing and of its README recomputed from the full file (all the file can show), results shown |

---

## Columns

| Block | Columns | Content |
|---|---:|---|
| Game | 14 | `League`, `Game_ID` (`YYYYMMDD_AWAY_HOME`, US Eastern date), `Season`, `Stage`, `Kickoff_UTC`, `Epoch`, teams, final score, `Winner`, `Total_Score`, `Margin`, `Match_Ending` |
| Pinnacle, Bet365, SBOBET | 22 each | moneyline, spread and total, opening then closing, with the time of each |
| Bwin, Betway, 1xBet | 30 each | the same, plus the 1X2 in regular time |
| William Hill, Betfair Exchange | 6 each | moneyline only |

`{Book}_ML_Home_Open` · `{Book}_ML_Home_Close` · `{Book}_ML_Close_Time` · `{Book}_Spread_Home_Line_Close` · `{Book}_Total_Line_Close` · `{Book}_1X2_Draw_Close` — the prefixes are `Pinnacle_`, `Bet365_`, `WilliamHill_`, `Bwin_`, `Betway_`, `BetfairExchange_`, `SBOBET_`, `1xBet_`.

### How to read it

**Prices are decimal odds**, up to 4 decimals: `1.91`, `2.375`. **The spread line is the home team's handicap:** `-6.5` means the home team gives 6.5 points. **Moneyline, spread and total include overtime; the 1X2 is regular time only**, so a tie after four quarters wins the draw. **Times are UTC**, ISO 8601 with the T and the Z. **The opening price is the first price recorded for the main line, the closing price the last one before tip-off**; each one carries its own time, so you can see how close to tip-off it was taken.

```python
import pandas as pd

df = pd.read_csv("NBA_World_Opening_Closing_Odds_2008-2026_SAMPLE.csv")

# Pinnacle's no-vig probability of the home team at the close
h, a = 1 / df["Pinnacle_ML_Home_Close"], 1 / df["Pinnacle_ML_Away_Close"]
pinnacle_home = h / (h + a)

# how far each book moved the spread, open to close
books = ["Pinnacle", "Bet365", "Bwin", "Betway", "SBOBET", "1xBet"]
spread_move = pd.DataFrame({b: df[b + "_Spread_Home_Line_Close"] - df[b + "_Spread_Home_Line_Open"] for b in books})

# how close to tip-off Bet365's closing moneyline was recorded, in minutes
tip = pd.to_datetime(df["Kickoff_UTC"])
bet365_close_min = (pd.to_datetime(df["Bet365_ML_Close_Time"]) - tip).dt.total_seconds() / 60
```

---

## Said plainly

- **Pinnacle starts on 16 October 2018**, with the moneyline and the total; its spread starts with the July 2020 restart. Before the restart, its closing price is its last recorded price, hours before tip-off.
- **2008-09 is a partial season for the books** (Bet365 from 19 January 2009). 623 games carry no price at all: 602 in 2008-09 and 21 in 2010-11. They stay in the file so that the schedule is complete.
- **William Hill and Betfair Exchange: moneyline only.** William Hill starts with the 2010 Finals and is absent from the start of 2025-26 to 31 March 2026. Betfair Exchange's prices appear to be net of the exchange's commission; it is missing in 2014-15 and has few openings.
- **SBOBET: spread and total from 2010-11 to 2021-22**, moneyline from April 2019 to 2021-22. **1xBet: the 1X2 from October 2014**, spread and total from January 2015, moneyline from October 2015.
- **Betway prices the spread and the total from March 2011, with gaps:** no spread from 2016-17 to 2023-24, and neither from 7 December 2024 to the end of 2025-26 (both back in 2026-27). Its 1X2 runs from 2016-17 to February 2022 and from December 2024 to December 2025, then on 35 games of 2026-27.
- **Opening spreads and totals are thin at Bwin from 2008-09 to 2013-14 and at Bet365 from 2015-16 to 2025-26.**
- **Closing times differ by book and market.** Median against the scheduled tip-off: Pinnacle 8 minutes after, William Hill 69 minutes before on the moneyline, Bet365 92 minutes before on the total. The time columns show it game by game.
- **2026-27 so far: Pinnacle, Bet365, William Hill, Bwin and Betway.** Betfair Exchange and 1xBet price 4 of the 88 games each.
- **The NBA Cup knockout games (21) carry Pinnacle prices only.**
- **No preseason, no All-Star games, no player props, no quarters or halves, no live odds, no futures.** One opening and one closing price per book and market, not every move in between.

---

## Verify before you buy

The figures of the listing and of its README — games, prices, the books and their first price, coverage season by
season, opening and closing times, margins, the games on the listing's images — recomputed from the full file and
printed PASS or FAIL, all but what the file cannot show (the counts of prices left out while it was built, the 8
corrected tip-off times, the 145 Pinnacle closes taken from a second record):
[on Kaggle](https://www.kaggle.com/code/oliviersportsdata/nba-world-books-odds-verify-before-you-buy) · [on GitHub](https://github.com/ovignez-hash/nba-opening-closing-odds-world-books-pinnacle/blob/main/NBA_World_Verify_Before_You_Buy.ipynb) (results shown).

---

## The full dataset

| | Sample | Full |
|---|---|---|
| Games | 20 | 23,212 |
| Seasons | 2008-09 to 2026-27 | 2008-09 to 2026-27, through 31 Oct 2026 |
| Prices | 1,043 | 1,203,088 |
| Columns | 182 | 182 |
| Files | 1 CSV + README | 1 CSV + README |

Once a year, after the Finals, the file adds the completed season. The games after 31 October 2026 come with the
[NBA World Books monthly updates](https://sportsdataolivier.gumroad.com/l/konvk?utm_source=github&utm_medium=readme&utm_campaign=nba_world&utm_content=monthly): each month's games, same 182 columns, ready to append.

The box score behind each game is sold separately: [NBA Matchup & Stats](https://sportsdataolivier.gumroad.com/l/nnadkm?utm_source=github&utm_medium=readme&utm_campaign=nba_world&utm_content=matchup) (also on [Whop](https://whop.com/oliviersportsdata/nba-matchup-stats-game-sheets-box-scores-2008-2026/?utm_source=github&utm_medium=readme&utm_campaign=nba_world&utm_content=matchup_whop)): game sheets, team and player box scores and inactive players since 2008-09, on the same Game_ID. Its 20-game sample is in `matchup_stats_sample/`.

→ **[Get the full archive](https://sportsdataolivier.gumroad.com/l/oeuoto?utm_source=github&utm_medium=readme&utm_campaign=nba_world&utm_content=footer)** · also on [Whop](https://whop.com/oliviersportsdata/nba-opening-closing-odds-pinnacle-7-world-books-2008-2026/?utm_source=github&utm_medium=readme&utm_campaign=nba_world&utm_content=whop_footer)

---

## Licence

Sample: free to explore and evaluate.
Full product: single commercial user. Use the data as you wish, including the models, predictions and products you sell.
Redistribution and resale of the files, or of the raw data in another format, are not permitted.

A question before buying: contact@oliviersportsdata.com

---

*Olivier Sports Data — From Chicken Area 🐔*
