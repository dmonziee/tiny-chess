# Tiny Chess

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/dmonziee/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/dmonziee/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A tiny chess engine in 4 KB of Python: 0x88 board, alpha-beta with iterative deepening to a fixed 200,000-node budget, quiescence, null-move pruning, LMR, transposition table, killers, MVV-LVA, piece-square tables and bishop pair. MIT licensed.

The node budget is fixed, never a clock: every move searches exactly 200,000 nodes, so trials replay move-for-move. Local practice Elo 1,364 (6-game trial vs the house gauntlet). `main.py` is the kit-compressed form of `source.py` (kept beside it in the working tree); re-pack it with `node cli/makefun.mjs compress source.py --out main.py` from the kit.
