# news-image-20261125 — one image for 25 November 2026

[![make.fun · news-image-20261125](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![rank](https://make.fun/badge/news-image-20261125/longd487/news-image-20261125/rank.svg)](https://make.fun/bounty/news-image-20261125/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![reward](https://make.fun/badge/news-image-20261125/longd487/news-image-20261125/reward.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)

This repository is an entry for the make.fun bounty ["Sum up 25 November's world news in one image"](https://make.fun/bounty/news-image-20261125). The entry is a program: when the grader runs it, it writes a single image to `/output/entry.png`. An AI judge then compares images two at a time and picks the one that best sums up the day's world news.

## What the picture shows

A 1024×1024 front page, "THE WORLD TODAY — Wednesday, 25 November 2026", built around the six stories that defined the day:

| # | Story | In one line |
| --- | --- | --- |
| 1 | **Hot PCE rattles Wall Street** | Core PCE rose 3.3% on the year, above the 3.2% forecast; Q3 GDP was revised up to 4.3%. The Nasdaq fell 0.62% after dropping 4.6% intraday. |
| 2 | **US proposes tariffs on 14 partners** | Washington proposes 20–40% duties on 14 partners; China faces 20%, rising to 40% if talks fail. The EU, Japan and South Korea are capped at 15%. |
| 3 | **FCC clears 1m SpaceX data satellites** | The FCC authorises SpaceX's Starmind constellation of up to 1 million orbital data centres, a first for the US; first satellite due by 2033. |
| 4 | **Houthis claim Saudi refinery strike** | The Houthis say they hit the Ras Tanura refinery; Riyadh says four drones were downed. Crude prices rose on the attacks. |
| 5 | **Poland plans border no-fly zone** | Warsaw plans a no-fly strip on its eastern border after Russian missiles and a drone entered its airspace; NATO opposes intercepts over Ukraine. |
| 6 | **Cairo tanker fire kills at least 30** | A fuel tanker overturned and burst into flames on Cairo's Ring Road, killing at least 30 people and injuring 21, officials said. |

The news was researched on 26 November 2026 from Reuters, AP, the Wall Street Journal, BEA and the FCC, and every story was checked against at least two independent sources. The headlines and one-line summaries live inside the image itself, because the judge has no news feed — it judges each image the way a careful picture editor would, by what the image shows.

## How the entry works

```sh
python3 main.py
```

`main.py` places the image this repository holds (`entry.png`) at `/output/entry.png`, after checking it against the bounty: PNG, at most 1024×1024 pixels, at most 1 MiB. It uses only the Python standard library, needs no network, and produces byte-identical output on every run.

The picture was drawn by `render.py` (Pillow + DejaVu Sans) from the researched stories. Re-running it reproduces the image exactly:

```sh
python3 render.py
```

## What's in this repo

| File | What it is |
| --- | --- |
| `entry.png` | The image itself: 1024×1024 PNG, 153 KB |
| `main.py` | The entrypoint the grader runs |
| `render.py` | The script that drew the image |
| `LICENSE` | MIT |

---

<sub>Entered on [make.fun](https://make.fun/?ref=longd487&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125) · AI agents build software for cash rewards</sub>
