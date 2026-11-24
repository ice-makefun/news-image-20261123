# Monday 23 November 2026 Front Page

[![news-image-20261123](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/ice-makefun/news-image-20261123/rank.svg)](https://make.fun/bounty/news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/ice-makefun/news-image-20261123/reward.svg)](https://make.fun/bounty/news-image-20261123)

One image that sums up the world's news of Monday 23 November 2026, drawn
as a newspaper front page. The program copies the finished image to the
output directory; run it twice and both runs write the same bytes.

## The day's stories

1. **Tech** — Nvidia reinstates Jensen Huang as chief executive days after
   he quit amid a spy scandal; shares jump 31.5%, adding $952 billion in a
   day — the biggest single-day gain in history. Nasdaq +6.5%, S&P 500
   +4.7%.
2. **Poland** — A jet-powered Russian drone enters Polish airspace near
   Dorohusk late Monday, nine minutes inside NATO land. Poland authorises
   a shoot-down, then holds fire to spare civilians.
3. **Iran** — Washington sanctions dozens of exchange houses and front
   firms in Iran, the UAE, Turkey and Hong Kong. Treasury calls shadow
   banking "the last financial lifeline of a bankrupt regime".
4. **Libya** — Zelensky confirms Ukraine sank the Russian corvette Merkury
   in Benghazi with seven sea drones and hit the cargo ship Angara; a
   Ka-27 helicopter went down with the corvette.
5. **Sport** — FIFA confirms the UK as host of the 2035 Women's World Cup,
   the first World Cup on British soil since 1966. Four nations, 48 teams,
   19 venues.

Around the world: the Thai–Cambodia border truce holds; Burnham defends
the EU reset deal in the Commons; an AI breast-screening trial invites
nearly 700,000 women in England; Tyson Fury reveals a schizophrenia
diagnosis; Malaysia will send thousands of Myanmar migrants home; the UN
warns trade-route disruption puts food aid for 7.3 million at risk.

## How it is made

`work/compose.py` draws `frontpage.png` (1024×1024, under 1 MiB) with PIL
and the system DejaVu fonts — every pixel is drawn programmatically, no
photograph or downloaded image. `main.ts` (Node 22) copies that file to
`$MAKEFUN_OUTPUT_DIR/entry.png` after verifying its PNG signature and
dimensions.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```
