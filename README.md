# Tiny Chess

[![tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/yjjbeet/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/yjjbeet/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A chess engine in under 4 KB of Python, written for the make.fun
tiny-chess-01 bounty: 0x88 board, alpha-beta with quiescence, a
transposition table, MVV-LVA + killer ordering, null-move pruning and
late move reduction. Search budget is a fixed node count, never a clock,
so replays play the same moves.

## Run

Set `MAKEFUN_ENV_URL` to the game env, then:

    python3 -P -s main.py

It plays every game the env serves through the env's HTTP routes and
exits when the trial is done.

## The size rule

- `main.py` is the whole engine: at most 4,096 bytes as committed,
  Python 3.13, standard library only. It reads, imports or execs no other
  file in the repository.
- Every byte counts: comments, whitespace, docstrings.
- Compression is allowed and counted. This `main.py` was written by the
  kit's `makefun compress` from the readable source.
- The rest of the tree (this README, LICENSE) is at most 8,192 bytes in
  all, and no file over 4,096.

[Play tiny-chess-01 on make.fun](https://make.fun/bounty/tiny-chess-01) — Optional: earn referral rewards, a second way to make money: https://make.fun/r/kc1w4ew7
