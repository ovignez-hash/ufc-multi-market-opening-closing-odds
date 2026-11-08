# UFC Opening & Closing Odds — free 20-fight sample

`UFC_Opening_Closing_Odds_2018-2026_SAMPLE.csv` holds 20 fights of the full product: the same 228 columns and the same
format, the rows copied byte for byte from the full file. Read it with
`pd.read_csv("UFC_Opening_Closing_Odds_2018-2026_SAMPLE.csv", sep=";", encoding="utf-8-sig")`.

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

Below, unchanged, the README shipped with the full product (4,249 fights).

---

# UFC Multi-Market — Opening & Closing Odds, Props & Results (2018–2026)

One row per fight. 4,249 fights of 354 UFC events, from 14 January 2018 to 20 June 2026: numbered events, Fight Nights, The Ultimate Fighter finales and Noche UFC. No Dana White's Contender Series, no Road to UFC tournament nights (the three Road to UFC finals fought on the UFC 325 card are in).

For each fight, when the source has them: the opening line and the closing prices of seven sportsbooks on the moneyline and the total rounds, each book with its own total line; the public betting split on both markets; from 9 May 2020, four prop markets across the US sportsbooks; and the official result, with the method, the round, the time and the fight stats of both fighters.

| | |
|---|---|
| Fights | 4,249 |
| Events | 354 |
| Period | 14 January 2018 to 20 June 2026 |
| Fighters | 1,450, each with a stable ID |
| Sportsbooks, closing prices | Betcris · Heritage · BetOnline · Bovada · BetAnything · William Hill · Everygame |
| Opening line | `Opener`, the first line published for the fight |
| Core markets | Moneyline · Total rounds, with each book's own line |
| Prop markets, from 9 May 2020 | Total rounds · Will the fight go the distance · How will the fight end · Method of victory: opening, consensus and best price, the number of sportsbooks and their names |
| Public betting split | % of bets on each side, moneyline and total rounds |
| Results | winner, method, round, finish time, judges' scorecards; knockdowns, significant strikes, takedowns and submission attempts of both fighters |
| Prices | 253,510, each in American and decimal odds |
| Columns | 228 |
| File | `UFC_Opening_Closing_Odds_2018-2026.csv`: UTF-8 with BOM, semicolon-separated, dot as decimal mark |

```python
import pandas as pd
df = pd.read_csv("UFC_Opening_Closing_Odds_2018-2026.csv", sep=";", encoding="utf-8-sig")
```

## Fights

| Year | Events | Fights |
|---|---:|---:|
| 2018 | 39 | 460 |
| 2019 | 42 | 510 |
| 2020 | 41 | 456 |
| 2021 | 43 | 508 |
| 2022 | 42 | 511 |
| 2023 | 43 | 519 |
| 2024 | 42 | 517 |
| 2025 | 42 | 520 |
| 2026 | 20 | 248 |

2026 stops on 20 June 2026. Every fight of these events that took place is in the file, with 23 exceptions: fights with no moneyline or total at the source (see *Known limitations*). Cancelled bouts are not in the file. 720 women's fights; 158 fights marked as title fights and 5 as BMF title fights (the two title fights of UFC 292, whose event card is missing, are not marked).

## Columns

**Fight — 36 columns**

| Column | Content |
|---|---|
| `Fight_ID` | 1 to 4,249, in date order |
| `Date` | event date, `YYYY-MM-DD`, as in the official statistics |
| `Event`, `Location` | event name and city, as in the official statistics (`UFC 229: Khabib vs. McGregor`) |
| `Attendance`, `PPV_Sales` | spectators and pay-per-view buys, as published on the event card; empty when not published (attendance on 202 events, pay-per-view buys on 40) |
| `Card_Segment` | `Main Event`, `Co-Main Event`, `Main Card`, `Prelims`, `Early Prelims`. The main event is the last bout of the card, the co-main event the one before |
| `Bout_Order` | position on the card, `1` for the first fight of the night |
| `Title` | `Championship` for a UFC title fight, `BMF` for the BMF title, empty otherwise and on the 49 fights without an event card |
| `Weight_Class` | as in the official statistics: 13 classes, `Catch Weight` included |
| `Gender` | `Men` or `Women`. At catchweight the fighters tell: 7 women's fights are catchweight bouts |
| `Fighter_A`, `Fighter_B` | names as in the official statistics. `Fighter_A` is the fighter listed first on the odds page, `Fighter_B` the second; `Fighter_B` is the betting favourite on 70.8% of the fights |
| `Fighter_A_ID`, `Fighter_B_ID` | one ID per fighter, the same on all his or her fights: 1,450 fighters. The two UFC fighters named Bruno Silva have their own ID |
| `Fighter_A_Country`, `Fighter_B_Country` | country shown on the event card (99 countries) |
| `Fighter_A_Result`, `Fighter_B_Result` | `Win`, `Loss`, `Draw` or `No Contest` |
| `Winner` | name of the winner; empty for draws and no contests |
| `Method` | as in the official statistics: `KO/TKO`, `SUB`, `U-DEC`, `S-DEC`, `M-DEC` (unanimous, split, majority decision), `DQ`, `CNC` (no contest, the fight could not continue), `Overturned` (result changed after the event: to a no contest, once to a draw) |
| `Method_Detail` | finishing technique, from the official statistics (`Punches`, `Rear Naked Choke`…); for decisions, the three judges' scores from the event card, as written there (`29-28, 28-29, 29-28`): the winner's score first, except on 15 cards that give the loser's first. Empty on 29 decisions (see Results and fight data) |
| `Round`, `Finish_Time` | round in which the fight ended and time in that round (`m:ss`); `5:00` for decisions, except 6 technical decisions |
| `Fighter_A_Knockdowns`, `Fighter_B_Knockdowns` | knockdowns scored by each fighter |
| `Fighter_A_Sig_Strikes`, `Fighter_B_Sig_Strikes` | significant strikes landed |
| `Fighter_A_Takedowns`, `Fighter_B_Takedowns` | takedowns landed |
| `Fighter_A_Sub_Attempts`, `Fighter_B_Sub_Attempts` | submission attempts |
| `ML_A_Bet%`, `ML_B_Bet%` | public betting split on the moneyline: % of bets on each fighter |
| `Total_Over_Bet%`, `Total_Under_Bet%` | the same on the total rounds |

**Core markets — 9 columns per source**, for the 8 sources `Opener`, `Betcris`, `Heritage`, `BetOnline`, `Bovada`, `BetAnything`, `WilliamHill`, `Everygame`. The columns are grouped by market: the moneylines of the 8 sources, then their totals.

```
{Src}_ML_A_US      {Src}_ML_A_Dec        {Src}_ML_B_US        {Src}_ML_B_Dec
{Src}_Total_Line   {Src}_Total_Over_US   {Src}_Total_Over_Dec   {Src}_Total_Under_US   {Src}_Total_Under_Dec
```

**Props — 120 columns, from 9 May 2020**

| Prefix | Market | Outcomes |
|---|---|---|
| `TR_` | Total rounds | over and under, with the line |
| `Dist_` | Will the fight go the distance | `Yes`, `No` |
| `End_` | How will the fight end | `KOTKO`, `KOTKODQ`, `SUB`, `DEC`, `Draw` |
| `MOV_` | Method of victory | `A_KOTKO`, `A_KOTKODQ`, `A_SUB`, `A_DEC`, the same for B, `Draw` |

```
TR_Open_Line   TR_Open_Over_US   TR_Open_Over_Dec   TR_Open_Under_US   TR_Open_Under_Dec   (the same with Cons)
TR_Best_Over_Line   TR_Best_Over_US   TR_Best_Over_Dec   TR_Best_Under_Line   TR_Best_Under_US   TR_Best_Under_Dec
Dist_Open_Yes_US   Dist_Open_Yes_Dec   Dist_Open_No_US   Dist_Open_No_Dec        (the same with Cons and Best)
End_Cons_KOTKO_US   End_Cons_KOTKO_Dec   …   MOV_Best_B_SUB_US   MOV_Best_Draw_Dec
TR_NBooks   TR_Books   Dist_NBooks   Dist_Books   End_NBooks   End_Books   MOV_NBooks   MOV_Books
```

`Open` is the opening price shown by the odds-comparison page, `Cons` its consensus price and `Best` the best price among the sportsbooks, both at the close. `NBooks` is the number of sportsbooks quoting the market (one side or more), `Books` their names; when no sportsbook quotes it at the close, only the opening price is there and `NBooks` is `0` (6 markets). When a fight is listed twice on a prop page, the listing with the most sportsbooks is kept. `Books` follows the order of the comparison page. On the total rounds the best over and the best under can come from lines that differ (528 fights): `TR_Best_Over_Line` and `TR_Best_Under_Line` give the line of each.

### How to read it

**`Opener` is the opening line**, the first line published for the fight, with its prices. **The seven books carry their closing prices**, the last ones before the fight. There is no opening price per book and nothing in between.

**Prices are American odds, as integers**: `-150`, and `130` for +130; even money is `100`. The decimal price is beside each one, to two decimals.

**Each book has its own total line.** On 1,380 fights the books did not all post the same line. The over and the under of a book are always on the same line. A total of `1.5` rounds is reached at 2:30 of the second round.

**The public betting split** is the share of bets on each side, as published with the odds. The two sides of a market add up to 100.

**In the props**, some books quote KO/TKO and others KO/TKO/DQ: both are kept as published, in their own columns. `DEC` is the decision ("points" on the page).

**An empty cell means no price**, never zero and never estimated. A market is either complete for a source, both sides with the line, or empty.

## How the prices were checked

Every price was read from the source pages for this edition. Prices that cannot exist, or that contradict the rest of the market, were left out rather than corrected: 125 markets (one source's moneyline or total on one fight) out of 58,804.

| Left out | Markets |
|---|---:|
| One side of the market missing | 42 |
| Closing moneyline far from the other books on the same fight: more than 15 points of probability from their median, margin removed | 40 |
| Total price without a line (Bovada, 14 January 2018) | 11 |
| Prices that cannot exist: a margin outside 1.5–25% on the moneyline, 0–15% on the total | 11 |
| Fight listed twice on the page with different prices (Maria Oliveira – Tabatha Ricci, 23 October 2021): the sources whose two listings differ or that price one listing only | 10 |
| Total line outside 0.5–4.5 rounds | 4 |
| Placeholder prices (±10000 and beyond) | 4 |
| Over and under quoted on different lines | 3 |

In the props, 47 opening or consensus pairs (total rounds, distance) with a margin outside 0–25% are left out, and so is one total-rounds market quoted on the under only (Claudia Gadelha – Yan Xiaonan, 7 November 2020). 14 public betting splits recorded 0% / 0% are left empty, and so are the splits of Maria Oliveira – Tabatha Ricci, whose two listings give different ones. No rule bears on the height of a total line: a book may post its own line, far from the others', and keeps it (BetOnline at 2.5 rounds on Stipe Miocic – Daniel Cormier, UFC 241, the other books at 4.5).

Also checked across the whole file: every fight is unique and matched to the official statistics by date and fighters; `Winner` agrees with the results on every row; every American price matches its decimal price; no book's prices run against the other books' over a season (correlation of the probabilities above 0.9 for every book and year).

## Coverage

Fights with a price, source by source:

| Source | Moneyline | Total rounds |
|---|---:|---:|
| Opener (opening line) | 4,209 (99.1%) | 4,200 (98.8%) |
| Betcris | 3,662 (86.2%) | 3,521 (82.9%) |
| Heritage | 4,184 (98.5%) | 4,211 (99.1%) |
| BetOnline | 4,218 (99.3%) | 4,203 (98.9%) |
| Bovada | 4,202 (98.9%) | 2,299 (54.1%) |
| BetAnything | 2,472 (58.2%) | 2,470 (58.1%) |
| William Hill | 4,224 (99.4%) | 2,216 (52.2%) |
| Everygame | 4,201 (98.9%) | 4,187 (98.5%) |

Moneyline coverage, year by year (% of the year's fights):

| Source | 2018 | 2019 | 2020 | 2021 | 2022 | 2023 | 2024 | 2025 | 2026 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Opener | 98% | 99% | 97% | 98% | 100% | 100% | 100% | 100% | 100% |
| Betcris | 100% | 100% | 99% | 55% | 31% | 100% | 100% | 100% | 100% |
| Heritage | 99% | 99% | 95% | 97% | 100% | 100% | 99% | 99% | 99% |
| BetOnline | 100% | 100% | 97% | 98% | 100% | 100% | 100% | 100% | 100% |
| Bovada | 99% | 98% | 97% | 96% | 100% | 100% | 100% | 100% | 100% |
| BetAnything | 0% | 0% | 0% | 31% | 100% | 100% | 100% | 100% | 100% |
| William Hill | 99% | 99% | 99% | 99% | 100% | 100% | 100% | 100% | 99% |
| Everygame | 99% | 99% | 99% | 97% | 96% | 100% | 100% | 100% | 100% |

Total rounds coverage, year by year:

| Source | 2018 | 2019 | 2020 | 2021 | 2022 | 2023 | 2024 | 2025 | 2026 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Opener | 99% | 97% | 97% | 97% | 100% | 100% | 100% | 100% | 100% |
| Betcris | 100% | 100% | 100% | 55% | 31% | 100% | 100% | 100% | 42% |
| Heritage | 98% | 99% | 99% | 97% | 100% | 100% | 99% | 99% | 100% |
| BetOnline | 99% | 97% | 97% | 97% | 100% | 100% | 100% | 100% | 100% |
| Bovada | 0% | 0% | 0% | 7% | 100% | 100% | 99% | 100% | 80% |
| BetAnything | 0% | 0% | 0% | 31% | 100% | 99% | 100% | 100% | 100% |
| William Hill | 35% | 0% | 0% | 5% | 98% | 99% | 100% | 60% | 73% |
| Everygame | 98% | 99% | 100% | 98% | 93% | 100% | 100% | 100% | 100% |

Public betting split: 4,234 fights on the moneyline, 4,177 on the total rounds.

Props, from 9 May 2020 (3,184 fights since that date):

| Market | Fights | Share | Most books on one fight |
|---|---:|---:|---:|
| Total rounds | 2,999 | 94.2% | 10 |
| Will the fight go the distance | 2,959 | 92.9% | 14 |
| How will the fight end | 2,640 | 82.9% | 5 |
| Method of victory | 2,958 | 92.9% | 8 |

Sportsbooks in the props, by number of markets quoted: FanDuel, DraftKings, BetRivers, SugarHouse, BetMGM, Caesars, PartyCasino, Fanatics, theScore Bet, Novig, Hard Rock, Fliff, ProphetX, Kalshi.

## Results and fight data

- 4,173 wins, 33 draws, 43 no contests. Results, methods, rounds, finish times, weight classes, events, locations and fight stats are those of the official UFC statistics.
- `Overturned`: 24 results changed after the event (a failed drug test, a commission review): 23 to a no contest, 1 to a draw (Mansur Abdul-Malik – Cody Brundage, 14 June 2025). The file gives the result as it stands, not the one announced on fight night.
- `CNC`: 20 fights stopped by an accidental foul and declared no contests.
- 6 technical decisions end before 5:00 of the third round: the fight was stopped and went to the scorecards.
- Judges' scores: on 2,093 of the 2,122 decisions. 14 event cards give none. On 15 others the card's scores do not fit the official result (a split card on a unanimous decision, a `30-37`): they are left out, not corrected. The card's own label ("Unanimous", "Split"…) is not kept, since it sometimes contradicts the official method; `Method` gives it.
- Card segment, bout order and title come from the event cards. They are missing on 49 fights, most of them from the cards of 12 and 19 August 2023 (UFC Fight Night: Luque vs. Dos Anjos, UFC 292) and the three Road to UFC finals of UFC 325. Countries, also from the event cards, are missing on 28 fights.

## Known limitations

- **Odds stop on 20 June 2026.** Later events are not in this edition.
- **One opening line, closing prices for the seven books**: no opening price per book, nothing in between. No round betting, no live odds.
- **Betcris has no price from 24 July 2021 to 20 August 2022**, and no total rounds after 21 March 2026. **BetAnything starts in September 2021.** On the total rounds, **Bovada starts in November 2021** and **William Hill** is patchy before 2022 (see the tables above).
- **Props start on 9 May 2020.** The 1,065 fights before that date have no prop prices.
- **Method of victory**: a fight takes its prices from a block of the comparison page that names both fighters (the block of the page dated like the fight, a block of that fight alone first, else the one with the most prices, and on a tie the first of the page); only when no block does, each fighter keeps his own from a block that names him, chosen the same way. When a block lists several fights, its draw price cannot be tied to one fight and is left out. When a fighter's outcome is quoted twice in a block with two different prices (two labels for the same fighter), that price is left out (19 fights). On some 2025–2026 pages the KO/TKO outcome of a fighter carries his name only: it is read as KO/TKO when the same fighter's submission and decision prices are in the block and no other knockout outcome; any other name-only label is left out. From 28 March 2026 the pages add a KO/TKO/DQ/submission outcome (the fighter wins inside the distance), and one block (Vince Morales – Chris Gutierrez, 30 May 2020) quotes combined outcomes (submission or draw, KO/TKO/DQ or draw, draw or decision): none of these is in the file.
- **Justin Ledet**: on his 4 fights his row is blank on the odds page (no name, no price). The moneyline is left out, the total rounds are kept.
- **Marked cancelled on the odds page**: 22 fights of the file: 20 no contests (16 CNC, 4 overturned after the event) and 2 fights that ended with a winner: Vinicius Moreira – Alonzo Menifield, 19 January 2019; Justin Tafa – Karl Williams, 23 March 2024. All keep their prices and their official result.
- **Fights missing at the source** (23): no moneyline or total on the source pages, left out of the file. 3 of them have prop prices on the comparison pages (Luana Carolina – Loopy Godinez, 16 October 2021; CJ Vergara – Daniel Lacerda, 25 March 2023; Kai Kamaka III – Dakota Hope, 4 April 2026): without a moneyline or a total, they are not in the file either.

| Event | Date | Fights |
|---|---|---|
| UFC Fight Night: Cowboy vs. Edwards | 23 June 2018 | Petr Yan – Teruto Ishihara; Yan Xiaonan – Viviane Pereira; Ji Yeon Kim – Melinda Fabian |
| The Ultimate Fighter: Undefeated Finale | 6 July 2018 | Michael Trizano – Joe Giannetti; Brad Katona – Jay Cucciniello; Luis Pena – Richie Smullen; John Gunther – Allan Zuniga; Bryce Mitchell – Tyler Diamond |
| UFC 226: Miocic vs. Cormier | 7 July 2018 | Daniel Cormier – Stipe Miocic |
| UFC 230: Cormier vs. Lewis | 3 November 2018 | Lyman Good – Ben Saunders |
| The Ultimate Fighter: Heavy Hitters Finale | 30 November 2018 | Juan Espino – Justin Frazier; Macy Chiasson – Pannie Kianzad; Maurice Greene – Michel Batista; Leah Letson – Julija Stoliarenko |
| UFC Fight Night: Assuncao vs. Moraes 2 | 2 February 2019 | Geraldo de Freitas – Felipe Colares |
| UFC Fight Night: Barboza vs. Gaethje | 30 March 2019 | Casey Kenney – Ray Borg |
| UFC Fight Night: Jacare vs. Hermansson | 27 April 2019 | Carla Esparza – Virna Jandiroba; Gilbert Burns – Mike Davis; Angela Hill – Jodie Esquibel |
| UFC Fight Night: Joanna vs. Waterson | 12 October 2019 | Mike Davis – Thomas Gifford |
| UFC Fight Night: Ladd vs. Dumont | 16 October 2021 | Luana Carolina – Loopy Godinez |
| UFC Fight Night: Vera vs. Sandhagen | 25 March 2023 | CJ Vergara – Daniel Lacerda |
| UFC Fight Night: Moicano vs. Duncan | 4 April 2026 | Kai Kamaka III – Dakota Hope |

  Lyman Good – Ben Saunders (UFC 230) is among them: the odds page lists the original matchup, Sultan Aliev – Lyman Good, not the fight that took place.

## Changes from the previous edition

- **BookMaker and Ozoon are gone**: on this source they repeat Betcris and Bovada price for price.
- **Results from the official UFC statistics**: winner, method, round, finish time, weight class, event name and location. **New: the fight stats of both fighters** (knockdowns, significant strikes, takedowns, submission attempts).
- **Each book now has its own total line.** The previous edition had a single `Total_Line` for all books; the books did not post the same line on 1,380 fights.
- **Fighter order**: the order of the odds page. The previous edition used the order of the event card.
- **Fighter IDs**: one stable ID per fighter, on every fight. `Fighter_X_Rank` is removed: it held numbers shown on the event pages when they were collected in 2026, not the ranking at the time of the fight.
- **Props**: opening, consensus and best price for the outcomes of the four markets (the KO/TKO/DQ/submission outcome of 2026 aside), in American and decimal odds, with the number of sportsbooks and their names. KO/TKO and KO/TKO/DQ kept apart in *How will the fight end*.
- **Fight list rebuilt from the official statistics**: 22 Road to UFC bouts filed in the previous edition under UFC 292, UFC Fight Night of 12 August 2023 and Road to UFC Shanghai are gone, and the 25 real fights of those two August 2023 cards are in. The 23 fights without a moneyline or total at the source are left out; the previous edition kept them, most without any price, 3 with props only, and gave Lyman Good – Ben Saunders the prices of the cancelled matchup.
- **Formats**: dates `YYYY-MM-DD` (the previous file wrote DD/MM/YYYY), whole numbers without decimals, attendance and pay-per-view buys as plain numbers.

## License

Single commercial user. Use the data as you wish, including the models, predictions and products you sell. Redistribution and resale of the files, or of the raw data in another format, are not permitted.

A question before buying: contact@oliviersportsdata.com

*Olivier Sports Data — From Chicken Area 🐔*
