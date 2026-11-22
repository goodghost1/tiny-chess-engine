# tiny-chess-engine

A 4 KB Python chess engine for make.fun tiny-chess-01: 0x88 board,
negamax + alpha-beta, quiescence search, iterative deepening under a
fixed node budget, transposition table, MVV-LVA + killer + history
ordering, material + piece-square evaluation.

`main.py` is the whole engine (lzma-packed by `makefun compress` from
`engine.py`, which is not committed). It talks to the env only, searches
to a fixed node budget (never a clock), so every trial replays the same
moves.
