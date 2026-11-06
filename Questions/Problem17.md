# Problem 17: Real-Time Strategy Economy

## Part 1 - Problem

Simulate an RTS economy using discrete ticks. Model workers, resources,
buildings, production queues, technology upgrades, prerequisites, construction,
and supply limits. Jobs reserve resources atomically so concurrent actions
cannot spend the same resource.

Support pause, resume, cancellation, refunds, and event logging. Detect
deadlocks caused by mutually dependent queued actions.

## Part 2 - Input and Output

Input contains initial entities and tick-indexed commands such as `BUILD`,
`TRAIN`, `RESEARCH`, `CANCEL`, `PAUSE`, and `RESUME`. Output every tick's
resources, queues, completed actions, and errors.

## Part 3 - Constraints, Examples, and Requirements

- A queued action must satisfy prerequisites and available supply.
- Example: two builds requiring 50 minerals cannot both reserve an initial 60.
- Test simultaneous completion, cancellation refunds, queue limits, and deadlocks.
- Event logs must reproduce identical state from the same input.
- Implement in Rust and document per-tick scheduling complexity.
