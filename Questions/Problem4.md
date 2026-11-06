# Problem 4: Chess Move Validator

## Part 1 - Problem

Implement legal chess move generation for both sides. Support pieces, captures,
promotion, castling, en passant, check, checkmate, and stalemate. A move is
illegal if it leaves the moving player's king in check.

Also detect threefold repetition and the fifty-move rule. Keep board mutation
reversible so legal-move testing does not corrupt state.

## Part 2 - Input and Output

Input is a FEN position followed by coordinate moves such as `e2 e4`.
Output every legal move result and the terminal status: `CHECK`,
`CHECKMATE`, `STALEMATE`, `DRAW_REPETITION`, or `DRAW_50_MOVE`.

## Part 3 - Constraints, Examples, and Requirements

- Validate coordinates, turn ownership, path blocking, and special-move rights.
- Example: from the initial position, `e2 e4` is legal; `e2 e5` is rejected.
- Add perft tests for known positions and promotion/castling/en-passant tests.
- No illegal move may alter the board.
- Implement in Rust and state move-generation complexity.
