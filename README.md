# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Kurenai193/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Kurenai193/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A deterministic chess engine that fits in 4 KB of Python. Negamax search with alpha-beta pruning, principal-variation search, late-move reductions, null-move pruning, check extensions, a transposition table and quiescence search, with a tapered material + piece-square evaluation and repetition detection. It searches a fixed 160,000 nodes per move — never a clock — so every game replays identically. Local practice with the official kit (18 games against the house ladder): mean Elo 1586.

The packed `main.py` is 4,082 bytes. A fuller-featured build of the same engine (with pawn-structure terms and history/killer move ordering) measured mean Elo 1733 in the same 18 games but packs to over 7 KB, so this entry trades those features for the size cap; the search core is unchanged.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:PORT python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
