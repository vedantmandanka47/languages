# Problem 6: Battleship with Probability Targeting

## Part 1 - Problem

Create Battleship for a configurable rectangular board. Players place ships
horizontally or vertically, then alternate firing at cells. A shot is a hit or
miss; a ship is sunk only when all its cells are hit. The game ends when one
fleet is sunk.

The computer must use probability-density targeting, updating possible ship
placements after every result. It may never fire at a resolved cell.

## Part 2 - Input and Output

Input contains board dimensions, a seed, fleet definitions, placements, and
shot coordinates. Output legal placement results, `HIT`, `MISS`, `SUNK name`,
remaining ships, and the final winner.

## Part 3 - Constraints, Examples, and Requirements

- Reject overlap, out-of-bounds placement, and touching when that option is on.
- Identical seeds must produce identical computer fleets and choices.
- Example: hitting the last cell of Cruiser prints `SUNK Cruiser`.
- Test repeated shots, invalid placements, final sinking, and hidden information.
- Implement in Rust and state targeting complexity.
