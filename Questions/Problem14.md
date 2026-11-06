# Problem 14: Hidden-Information Mafia

## Part 1 - Problem

Implement a social-deduction engine with configurable roles, private knowledge,
day discussion, voting, night actions, blocking, protection, investigation,
and elimination. Resolve simultaneous night actions in a documented priority
order. Players who are dead cannot act.

Each player may see only information authorized by their role. Detect faction
victory immediately after every state transition.

## Part 2 - Input and Output

Input contains a seed, player roles, discussion messages, votes, and night
actions. Output each player's authorized view, public events, alive players,
and `TOWN_WINS`, `MAFIA_WINS`, or `IN_PROGRESS`.

## Part 3 - Constraints, Examples, and Requirements

- Handle ties, abstentions, blocked actions, protected targets, and dead players.
- Example: a blocked investigator receives no result and the target remains alive
  unless another valid action eliminates it.
- Test information isolation so one role cannot read another role's private view.
- Keep rules, bot strategies, and terminal presentation separate.
- Implement in Rust and document resolution complexity.
