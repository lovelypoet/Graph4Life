# Graph4life Evaluation

## Benchmark cases

1. Valid grounded lesson: extract expected concepts, relations, citations, and quiz.
2. Missing evidence: refuse unsupported quiz generation.
3. Ambiguous evidence: return `DISAMBIGUATE` with required evidence.
4. Duplicate/empty chunks: deduplicate safely and return a useful validation error.
5. API contract: valid request succeeds; malformed input returns structured 4xx.

## Ground truth

- Concepts/relations match annotated fixtures.
- Every generated claim cites an available source span.
- Unsupported claim rate is zero on safety cases.
- Decision labels match expected `GENERATE_QUIZ`, `DISAMBIGUATE`, or `REFUSE`.

## Metrics

- Precision, recall, and F1 for concepts and relations.
- Citation accuracy, source recall, unsupported-claim rate.
- Quiz decision accuracy, refusal precision, schema validity.
- Test pass rate, latency, reproducibility, and human rating (0-2: incorrect, partial, correct).

