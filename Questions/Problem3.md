# Problem 3: Sudoku Battle

## Part 1 - Problem

Generate a valid Sudoku puzzle with one solution and let two players race on
independent copies. A move places a digit in an empty cell. Reject a move if it
violates its row, column, or subgrid. Track time, mistakes, hints, and solved
cells. The player who completes the puzzle first wins.

Implement a solver using constraint propagation, minimum-remaining-values
selection, and backtracking. The generator must verify uniqueness.

## Part 2 - Input and Output

Input contains a difficulty, seed, player actions `(player,row,column,digit)`,
and optional `HINT player` commands. Output the board, updated scores, rejected
actions, and `WINNER`, `DRAW`, or `IN_PROGRESS`.

## Part 3 - Constraints, Examples, and Requirements

- Use a `9 x 9` board with digits `1..=9`; clues cannot be edited.
- A generated puzzle must have exactly one solution.
- Example: placing `5` in a row containing `5` returns `INVALID_MOVE` and leaves
  the board unchanged.
- Test uniqueness, conflicting moves, hints, simultaneous completion, and seeds.
- Implement in Rust and document solver complexity.
