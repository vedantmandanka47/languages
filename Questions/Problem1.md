# Problem 1: Connect Four AI

## Part 1 - Problem

Implement Connect Four on an `R x C` board. Players alternate dropping discs
into columns; a disc falls to the lowest empty row. The first player to create
`K` consecutive discs horizontally, vertically, or diagonally wins. If the
board fills without a winner, the game is a draw.

Support human-vs-human and human-vs-computer modes. The computer must choose a
move with minimax, alpha-beta pruning, a depth limit, and a heuristic. Use a
transposition table to avoid evaluating repeated positions.

## Part 2 - Input and Output

Input contains `R C K`, a mode, and a sequence of column choices. Output every
board state, reject full or out-of-range columns, and print `WINNER player`,
`DRAW`, or `IN_PROGRESS`. In computer mode also print the selected column.

## Part 3 - Constraints, Examples, and Requirements

- `4 <= R,C <= 10`, `3 <= K <= 5`; the default is `7 6 4`.
- Run the default computer move within 2 seconds.
- Example: `R=4,C=4,K=3`, moves `0,1,0,1,0` produces `WINNER 1`.
- Add tests for all four directions, invalid moves, draws, and deterministic AI.
- Document time and space complexity and implement in Rust first.
