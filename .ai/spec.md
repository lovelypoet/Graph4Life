# Graph4life Implementation Spec

## Checklist

- [ ] Define user-visible behavior and acceptance examples.
- [ ] Define request/response schemas and failure states.
- [ ] Implement domain logic with source evidence.
- [ ] Add unit and integration tests.
- [ ] Add or update golden/evaluation cases.
- [ ] Run `pytest`; record result and known warnings.
- [ ] Update README and `.ai/memories.md`.

## Edge cases

- Empty, malformed, duplicate, or oversized input.
- Missing, conflicting, or low-confidence source evidence.
- Unsupported quiz claims; return refusal or disambiguation.
- Duplicate concepts, cyclic relations, missing IDs, and partial uploads.
- Network/model timeout, unavailable dependency, and concurrent writes.

