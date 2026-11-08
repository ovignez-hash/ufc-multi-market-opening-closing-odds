# 🥊 UFC Multi-Market — Opening & Closing Odds, Props & Results (2018–2026)

**Free sample: 20 fights, from the first fight of the file, 14 January 2018, to its last, 20 June 2026** — 15 title fights (2 of them for the BMF belt), 2 draws, 2 no contests, a disqualification and a technical decision.

Most UFC odds files give you one closing price per fight. The full dataset puts **the opening line and the closing prices of seven sportsbooks side by side, fight by fight**: Betcris, Heritage, BetOnline, Bovada, BetAnything, William Hill and Everygame. Moneyline and total rounds, **each book with its own line**, in American and decimal odds, plus **the public betting split**, **four prop markets from May 2020** and **the official result with the fight stats of both fighters**.

→ **[Get the full dataset](https://sportsdataolivier.gumroad.com/l/iiyon?utm_source=github&utm_medium=dataset&utm_campaign=ufc_oc&utm_content=hero)** — 4,249 fights, 14 January 2018 to 20 June 2026 · also on [Whop](https://whop.com/oliviersportsdata/ufc-opening-closing-odds-7-books-props-fight-stats-2018-2026/?utm_source=github&utm_medium=dataset&utm_campaign=ufc_oc&utm_content=whop_hero)

This repository holds the sample (`sample/`) and the *Verify before you buy* notebook (`UFC_Verify_Before_You_Buy.ipynb`, results shown). The sample is cut from the full file: the same 228 columns, the rows copied byte for byte.

---

## One fight, every market

UFC 298 — Ilia Topuria vs Alexander Volkanovski, Topuria by KO/TKO in round 2. Each book's closing prices, next to the opening line:

| Source | Topuria | Volkanovski | Total rounds | Over | Under |
|---|---:|---:|---:|---:|---:|
| Opening line | -105 | -115 | 3.5 | -155 | +125 |
| Betcris | +114 | -143 | 3.5 | -139 | +109 |
| Heritage | +112 | -136 | 4.5 | +105 | -129 |
| BetOnline | +115 | -135 | 3.5 | -144 | +114 |
| Bovada | +115 | -130 | 2.5 | -210 | +160 |
| BetAnything | +105 | -135 | 3.5 | -135 | +105 |
| William Hill | -110 | -110 | 3.5 | -125 | -110 |
| Everygame | +110 | -140 | 3.5 | -135 | +105 |

Props, consensus: the fight goes the distance +120, does not -164; Topuria by KO/TKO +350. Public betting split: 62% of the moneyline bets on Topuria, 70% of the total bets on the over.

---

## What's in this sample

| | |
|---|---|
| Fights | 20, from 2018 to 2026 |
| Prices | 1,057, each in American and decimal odds |
| Sources | the opening line + 7 sportsbooks; props across the US sportsbooks from May 2020 |
| Columns | 228 |
| File | `UFC_Opening_Closing_Odds_2018-2026_SAMPLE.csv` (semicolon-separated, UTF-8 with BOM), plus the README of the full product |

| Date | Fight | Why it is here | Result | Books with a closing ML | Prop markets |
|---|---|---|---|---:|---:|
| 14 Jan 2018 | Mike Santiago vs Mads Burnell | first fight of the file | Mads Burnell, U-DEC R3 | 6 | 0 |
| 9 Jun 2018 | Mike Jackson vs CM Punk | result overturned to a no contest after the event | No contest, Overturned R3 | 6 | 0 |
| 6 Oct 2018 | Conor McGregor vs Khabib Nurmagomedov | UFC 229, lightweight title | Khabib Nurmagomedov, SUB R4 | 6 | 0 |
| 29 Dec 2018 | Alexander Gustafsson vs Jon Jones | UFC 232, light heavyweight title | Jon Jones, KO/TKO R3 | 6 | 0 |
| 5 Oct 2019 | Israel Adesanya vs Robert Whittaker | UFC 243, middleweight title | Israel Adesanya, KO/TKO R2 | 6 | 0 |
| 2 Nov 2019 | Nate Diaz vs Jorge Masvidal | UFC 244, BMF title, doctor stoppage | Jorge Masvidal, KO/TKO R3 | 6 | 0 |
| 7 Mar 2020 | Joanna Jedrzejczyk vs Zhang Weili | UFC 248, strawweight title, split decision | Zhang Weili, S-DEC R5 | 5 | 0 |
| 12 Dec 2020 | Brandon Moreno vs Deiveson Figueiredo | UFC 256, flyweight title, majority draw | Draw, M-DEC R5 | 6 | 3 |
| 6 Mar 2021 | Aljamain Sterling vs Petr Yan | UFC 259, bantamweight title, won by disqualification | Aljamain Sterling, DQ R4 | 6 | 3 |
| 24 Apr 2021 | Jorge Masvidal vs Kamaru Usman | UFC 261, welterweight title, knockout | Kamaru Usman, KO/TKO R2 | 6 | 3 |
| 6 Nov 2021 | Zhang Weili vs Rose Namajunas | UFC 268, strawweight title, during the Betcris gap | Rose Namajunas, S-DEC R5 | 6 | 4 |
| 16 Apr 2022 | Chris Barnett vs Martin Buday | technical decision, stopped at 1:38 of round 3 | Martin Buday, U-DEC R3 | 6 | 4 |
| 12 Nov 2022 | Alex Pereira vs Israel Adesanya | UFC 281, middleweight title, late knockout | Alex Pereira, KO/TKO R5 | 7 | 4 |
| 16 Sep 2023 | Alexa Grasso vs Valentina Shevchenko | Noche UFC, flyweight title, split draw | Draw, S-DEC R5 | 7 | 4 |
| 17 Feb 2024 | Ilia Topuria vs Alexander Volkanovski | UFC 298, featherweight title, every prop market | Ilia Topuria, KO/TKO R2 | 7 | 4 |
| 13 Apr 2024 | Max Holloway vs Justin Gaethje | UFC 300, BMF title, last-second knockout | Max Holloway, KO/TKO R5 | 7 | 4 |
| 18 Jan 2025 | Renato Moicano vs Islam Makhachev | UFC 311, lightweight title | Islam Makhachev, SUB R1 | 7 | 0 |
| 25 Oct 2025 | Ciryl Gane vs Tom Aspinall | UFC 321, no contest after an accidental eye poke | No contest, CNC R1 | 7 | 0 |
| 31 Jan 2026 | Yizha vs Kaan Ofli | a fighter known by one name | Kaan Ofli, M-DEC R3 | 7 | 4 |
| 20 Jun 2026 | Kyoji Horiguchi vs Manel Kape | last fight of the file | Manel Kape, KO/TKO R3 | 7 | 4 |

*Books*: out of 7, the books with a closing moneyline on that fight. *Prop markets*: out of 4.

---

## Columns

| Block | Columns | Content |
|---|---:|---|
| Fight | 36 | `Date`, `Event`, `Location`, attendance and pay-per-view buys, card segment and bout order, title, weight class, both fighters with a stable ID and their country, the official result (`Winner`, `Method`, `Method_Detail`, `Round`, `Finish_Time`), knockdowns, significant strikes, takedowns and submission attempts of both fighters, the public betting split |
| Each of the 8 sources | 9 | moneyline of both fighters; total rounds line, over and under — every price in American and decimal odds |
| Props | 120 | total rounds, distance, how the fight ends, method of victory: opening, consensus and best price, number of sportsbooks and their names |

`Betcris_ML_A_US` · `Betcris_ML_A_Dec` · `Opener_Total_Line` · `Bovada_Total_Over_US` · `ML_A_Bet%` · `MOV_Cons_A_KOTKO_US` — William Hill's columns start with `WilliamHill_`.

**`Opener` is the opening line**, the first line published for the fight; **the seven books carry their closing prices**. Prices are American odds as integers (`-150`, and `130` for +130) with the decimal price beside each one. `Fighter_A` is the fighter listed first on the odds page, `Fighter_B` the second (the betting favourite on 70.8% of the fights). An empty cell means no price, never zero.

```python
import pandas as pd

df = pd.read_csv("UFC_Opening_Closing_Odds_2018-2026_SAMPLE.csv", sep=";", encoding="utf-8-sig")

def prob(us):                          # American odds -> implied probability
    return -us / (-us + 100) if us < 0 else 100 / (us + 100)

# Betcris closing probability of fighter A, margin removed
a, b = df["Betcris_ML_A_US"].map(prob), df["Betcris_ML_B_US"].map(prob)
df["betcris_a"] = a / (a + b)

# each book has its own total rounds line
df[[c for c in df.columns if c.endswith("_Total_Line")]].head()
```

---

## Said plainly

- **Odds stop on 20 June 2026.** Later events are not in this edition.
- **One opening line, closing prices for the seven books**: no opening price per book, nothing in between. No round betting, no live odds.
- **Betcris has no price from 24 July 2021 to 20 August 2022. BetAnything starts in September 2021.** On the total rounds, Bovada starts in November 2021 and William Hill is patchy before 2022.
- **Props start on 9 May 2020.**
- **23 fights with no moneyline or total at the source are left out**, listed in the README. No Contender Series, no Road to UFC tournament nights.
- **125 markets whose prices cannot exist or contradict the market were left out, never corrected.** The rules and the counts are in the README.

---

## Verify before you buy

The figures of the listing and of its README — fights year by year, results, prices, coverage of every book year by year, the props, the betting splits, the fights on the listing's images — recomputed from the full file and printed PASS or FAIL: [on Kaggle](https://www.kaggle.com/code/oliviersportsdata/ufc-multi-market-historical-odds-results) · [on GitHub](https://github.com/ovignez-hash/ufc-multi-market-opening-closing-odds/blob/main/UFC_Verify_Before_You_Buy.ipynb) (results shown).

---

## The full dataset

| | Sample | Full |
|---|---|---|
| Fights | 20 | 4,249 |
| Period | 2018 to 2026 | 14 January 2018 to 20 June 2026 |
| Prices | 1,057 | 253,510 |
| Columns | 228 | 228 |
| Files | 1 CSV + README | 1 CSV + README |

→ **[Get the full dataset on Gumroad](https://sportsdataolivier.gumroad.com/l/iiyon?utm_source=github&utm_medium=dataset&utm_campaign=ufc_oc&utm_content=footer)** · also on [Whop](https://whop.com/oliviersportsdata/ufc-opening-closing-odds-7-books-props-fight-stats-2018-2026/?utm_source=github&utm_medium=dataset&utm_campaign=ufc_oc&utm_content=whop_footer)

---

## License

- **Sample**: free to explore and evaluate.
- **Full dataset**: Single commercial user. Use the data as you wish, including the models, predictions and products you sell. Redistribution and resale of the files, or of the raw data in another format, are not permitted.

A question before buying: contact@oliviersportsdata.com

---

*Olivier Sports Data — From Chicken Area 🐔*
