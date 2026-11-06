# Problem 2: Minesweeper Solver

## Part 1 - Problem

Create Minesweeper on a `W x H` board containing exactly `M` mines. The first
revealed cell and its neighbors must be safe. Revealing an empty cell
flood-fills adjacent empty cells; numbered cells show adjacent mine counts.
Players may reveal, flag, and unflag cells.

Add a solver that repeatedly identifies guaranteed safe cells and guaranteed
mines from visible constraints. When deduction stops, it may choose the cell
with the lowest estimated mine probability.

## Part 2 - Input and Output

Input contains `W H M seed` followed by commands `REVEAL x y`, `FLAG x y`, and
`UNFLAG x y`. Output the visible board after each valid command and
`WIN`, `LOSS`, or `IN_PROGRESS`.

## Part 3 - Constraints, Examples, and Requirements

- `1 <= W,H <= 30`, `0 < M < W*H`; use exactly `M` mines.
- Identical seeds and commands must produce identical games.
- Example: revealing an empty region prints all reachable zero and boundary
  cells; revealing a mine prints `LOSS`.
- Test first-click safety, flood-fill, duplicate flags, bounds, and solver guesses.
- Implement in Rust and state solver complexity.
