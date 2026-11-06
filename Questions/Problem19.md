# Problem 19: Networked Turn-Based Game Protocol

## Part 1 - Problem

Design a versioned client/server protocol for a turn-based game such as
Battleship. Define join, ready, action, state-update, error, disconnect,
reconnect, and snapshot messages. The server is authoritative and must never
trust client hidden state or turn order.

Add sequence numbers, idempotent retries, timeouts, reconnect snapshots, and a
simulation of delay, duplication, reordering, and disconnects.

## Part 2 - Input and Output

Input is a stream of client messages and simulated network events. Output is
server state, accepted or rejected actions, responses, and the converged state
seen by each client.

## Part 3 - Constraints, Examples, and Requirements

- Duplicate messages must not apply an action twice; stale sequence numbers fail.
- Example: a client firing out of turn receives `INVALID_TURN` and no state change.
- Test delay, reordering, duplication, reconnect, hidden-state protection, and
  client convergence.
- Use explicit protocol versioning and structured error codes.
- Implement in Rust and document message-processing complexity.
