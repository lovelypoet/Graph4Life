# Graph4life Rules

- Preserve evidence: do not invent source facts, metrics, or API behavior.
- Keep changes small, typed, testable, and backward-compatible unless the spec says otherwise.
- Python: 3.12+, 4-space indentation, type hints, `ruff`-compatible style, clear domain names.
- FastAPI: validate at boundaries; return stable schemas; never leak secrets or raw stack traces.
- AI output: require source grounding, deterministic validation, and explicit refusal when evidence is insufficient.
- Reward: passing tests, traceable decisions, minimal diffs, useful docs (+1 each).
- Penalty: untested behavior, hidden state, unsupported claims, secrets, or destructive commands (-2 each).

