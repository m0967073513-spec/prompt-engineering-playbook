# Design Decisions

- Prompts are treated as versioned assets.
- Deterministic formats (JSON-only) are prioritized for automation.
- Chains make behavior reliable: generate → validate → repair.
- Evaluation uses a small golden set to catch regressions early.
- Safety constraints are explicit to prevent scope creep.

