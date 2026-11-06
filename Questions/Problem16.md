# Problem 16: Dungeon Crawler

## Part 1 - Problem

Generate a connected, seeded dungeon with rooms and corridors. Add field of
view, monsters, items, equipment, doors, traps, turn-based combat, status
effects, experience, an exit, and permadeath. Every action is an event resolved
in deterministic turn order.

Guarantee the exit is reachable and generated levels satisfy minimum room and
item requirements. Save and load using versioned serialization.

## Part 2 - Input and Output

Input contains a seed, map dimensions, generation settings, and commands such as
`MOVE`, `ATTACK`, `PICKUP`, `EQUIP`, and `USE`. Output visible state, events,
health, inventory, and `VICTORY` or `DEATH`.

## Part 3 - Constraints, Examples, and Requirements

- Hidden cells must not appear in the player's output.
- Example: an attack applies damage before a poison tick if that is the declared
  event order; tests must enforce the order.
- Test connectivity, visibility boundaries, combat, status expiration, and
  save/load equivalence.
- Implement in Rust and document generation complexity.
