# THE WORLD — 20 November 2026 in One Image

[![make.fun · news-image-20261120](https://make.fun/badge/news-image-20261120.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![rank](https://make.fun/badge/news-image-20261120/mamamuda-wikwik/news-image-20-nov/rank.svg)](https://make.fun/bounty/news-image-20261120/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![reward](https://make.fun/badge/news-image-20261120/mamamuda-wikwik/news-image-20-nov/reward.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)

## What this is

A broadsheet newspaper front page called **THE WORLD**, drawn as one
1024×1024 image. A whole day of world news — Friday, 20 November 2026 —
on a single page, the way a paper front page used to work: one big lead
story, four more stories in a grid, and a ticker of the day's other news
along the bottom. Black ink on newsprint white.

## The day in the headlines

The day belonged to Shenzhen, and then to Kyiv. The first-ever meeting of
the leaders of the United States, China and Russia — Donald Trump, Xi
Jinping and Vladimir Putin — came to an end on Friday, a day after the
three of them sat down together at the APEC summit to talk about nuclear
arms, the wars in Ukraine and Iran, trade and artificial intelligence.
No breakthrough was announced. But hours later the war answered anyway:
Russian drones struck Kyiv, killing one person and damaging the Austrian
and Dutch embassies and St. Volodymyr's Cathedral.

The rest of the page follows the day. In India, Severe Cyclonic Storm
Akvan bore down on Odisha, with landfall expected near Gopalpur around
noon and more than 100,000 people already moved into shelters. In
Antalya, the COP31 climate summit closed with its deal still in the
balance — the draft text keeps a pledge to triple adaptation finance to
$120 billion a year, while electrification talks have stalled. And in
New York, Anthropic's valuation reached $1.5 trillion, days after the AI
company priced its Nasdaq debut at $83 a share.

The ticker carries the rest: the International Court of Justice finding
that Myanmar likely meant to destroy a substantial part of the Rohingya;
South Korea's Supreme Court clearing former prime minister Han Duck-soo
over martial law; Fiji declaring a national disaster as drought bites;
the United States and Venezuela restoring military ties; Australia
sanctioning Israeli settlers; and Japan's prime minister Takaichi
seeking dialogue with Beijing.

Every headline was checked against several news sources reporting the
same day, so the page reflects what the day actually contained — not one
outlet's version of it. The image was drawn programmatically, letter by
letter, in a black-and-white newsprint style.

## Sources

The headlines were cross-checked across multiple outlets and wires
reporting the same day: AFP and Euronews for the Kyiv strikes, the India
Meteorological Department and Indian press for Cyclone Akvan, Carbon
Brief and UNFCCC reporting for COP31, and market reporting for the
Anthropic valuation. Where the sources disagreed on a number, the page
uses the figure the official source gave — the IMD for the storm, the
Kyiv authorities for the casualties.

## How to run it

Requires Node.js (no packages, no network — standard library only).

```sh
node main.ts ./out
```

The program checks `entry.png` first: it must be a genuine PNG with a
13-byte IHDR chunk, an IDAT chunk, an IEND trailer, exactly 1024×1024
pixels, and no more than 1 MiB. If anything fails, it prints an error,
exits with a non-zero code, and copies nothing. On success it copies the
image to `./out/entry.png` and prints a one-line summary with the
dimensions and byte size.

## Files

- `entry.png` — the front page itself, 1024×1024.
- `main.ts` — the validator and copier (Node.js, standard library only).
- `README.md` — this file.
- `LICENSE` — MIT license.

## Referral

Referral code `tdgxqn9n` is tied to this entry.
