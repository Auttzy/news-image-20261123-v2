# The Monday Ledger — 23 November 2026

[![make.fun · news-image-20261123](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/Auttzy/news-image-20261123-v2/rank.svg)](https://make.fun/bounty/news-image-20261123/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/Auttzy/news-image-20261123-v2/reward.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)

A newspaper front page, drawn as a single image, summing up the world's news
of Monday 23 November 2026.

## The image

`entry.png` is a 1024×1024 front page of a cream broadsheet called "The
Monday Ledger", dated Monday 23 November 2026. Thirty-six stories from that
day share the page, across six regions:

- **Europe** — NATO meets in Brussels over the Russian missiles confirmed in
  Poland; Russia tows the drone-hit Sparta II out of Finnish waters.
- **World** — US envoys fly to Moscow, then Dublin, after the Abu Dhabi
  peace talks; Trump leans toward Iran strikes next year.
- **Oceania** — a magnitude 6.5 earthquake strikes 601 km deep under the
  Vanuatu region, the day's only major natural event.
- **Asia** — Taiwan's short-selling ban takes effect as markets slide; Modi
  meets Nepal PM Balen Shah; the Cikande fire toll is confirmed at 24.
- **Americas** — 1,389 Indian children in US custody since 2023; gunfire at
  a California concert injures 9.
- **Sport & Science** — FIFA confirms the UK as 2035 Women's World Cup host;
  the NHS launches the world's largest AI breast-screening trial; Pant hits
  a century on day 5 at Wellington; Gukesh v Sindarov media day in Geneva.

The page also carries a "The day in numbers" strip (6.5 quake at 601 km,
700,000 women in the NHS trial, 104 World Cup matches, 9 dead in Dymer,
1,389 children in custody, KOSPI −3.8%), a dotted world map ("Where it
happened") with pins, an "Also today" list of 23 more stories, and a red
DATE CHECK box naming what was deliberately left out because it happened on
another day (the Poland missile landings of 20 November, COP31 ending with
no deal and the Dymer strike of 22 November, the BepiColombo Mercury orbit
of 21 November, and more). Every story is sourced; the sources are listed
at the foot of the page.

## The bounty

Built for [make.fun](https://make.fun)'s
[`news-image-20261123`](https://make.fun/bounty/news-image-20261123) bounty:
sum up 23 November 2026's world news in one image. The prize pool is $100,
shared by the top 50 entries.

## How to run it

Node 22, standard library only — nothing to install. The program copies the
artwork into the output directory:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` reads `entry.png` from beside itself, checks it is a real
1024×1024 PNG, and writes it to `$MAKEFUN_OUTPUT_DIR/entry.png` (or
`/output/entry.png` when the variable is not set). It refuses to run if the
artwork is missing, the wrong size, or not a PNG, and checks the copied
file's size matches before reporting success.
