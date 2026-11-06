# Problem 7: Tetris Engine

## Part 1 - Problem

Implement a deterministic Tetris engine with the seven tetrominoes. Support
movement, rotation, collision detection, soft drop, hard drop, line clearing,
scoring, levels, hold, preview, and game over. Use a seven-bag generator.

Rotations must use wall kicks and preserve the board when no rotated position
is legal. Every state transition must be replayable from a seed and event log.

## Part 2 - Input and Output

Input contains board dimensions, seed, and commands `LEFT`, `RIGHT`, `ROTATE`,
`SOFT_DROP`, `HARD_DROP`, `HOLD`, and `TICK`. Output the board, score, level,
cleared lines, next pieces, and `GAME_OVER` when applicable.

## Part 3 - Constraints, Examples, and Requirements

- Test every piece near every wall and against uneven stacks.
- Example: a hard drop followed by a completed row removes exactly that row.
- A piece may be held only once until the next piece locks.
- Test seven-bag distribution, rotation failure, scoring, and replay identity.
- Implement in Rust and document transition complexity.
