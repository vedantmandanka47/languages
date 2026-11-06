# Problem 10: 2048 AI

## Part 1 - Problem

Implement 2048 for an even board size. A move compresses tiles, merges equal
adjacent tiles once per move from the movement side, updates the score, and
spawns a new tile if the board changed. Detect reaching 2048 and no legal moves.

Add an expectimax AI with a tunable depth and heuristic for empty cells,
monotonicity, smoothness, and maximum tile placement.

## Part 2 - Input and Output

Input contains board size, seed, and moves `UP`, `DOWN`, `LEFT`, or `RIGHT`.
Output the board, score, highest tile, and `WIN`, `GAME_OVER`, or `PLAYING`.

## Part 3 - Constraints, Examples, and Requirements

- Support sizes `4, 6, or 8`; seeded runs must be reproducible.
- Example: `[2,2,2,2]` moved left becomes `[4,4,0,0]`, not `[8,0,0,0]`.
- Test all directions, unchanged moves, spawn behavior, win, and game over.
- Measure average score and highest tile over 100 seeded games.
- Implement in Rust and document AI complexity.
