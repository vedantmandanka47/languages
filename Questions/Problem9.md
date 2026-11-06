# Problem 9: Tower Defense Simulation

## Part 1 - Problem

Simulate tower defense on a weighted grid with spawn points and a base.
Enemies follow shortest paths. Towers have range, cooldown, damage, armor,
splash damage, or slow effects. Add money, lives, waves, and build rules.

Building or selling a tower may not remove the last valid route to the base.
Use discrete ticks rather than wall-clock timing and recalculate paths only
when the map changes.

## Part 2 - Input and Output

Input contains a map, waves, tower commands, and tick count. Output each tick's
events, enemy positions, health, money, lives, and `WAVE_COMPLETE`, `VICTORY`,
or `DEFEAT`.

## Part 3 - Constraints, Examples, and Requirements

- Reject invalid cells, insufficient money, and route-blocking placements.
- Example: an enemy with armor 3 receiving damage 5 loses 2 health.
- Test simultaneous attacks, death ordering, splash boundaries, path changes,
  and wave completion.
- Implement in Rust and document pathfinding complexity.
