# Graph4life Architecture

## Map

- `main.py`, `annotation_api.py`: FastAPI entrypoints and review API.
- `ai/`: ingestion, extraction, graph, grounding, quiz, evaluation logic.
- `adaptive_learning/`: adaptive-learning API and domain flow.
- `tests/`, `evals/`: software tests, golden cases, and AI evaluation reports.
- `fe/`, `index.html`: browser UI.
- `data/`, `uploads/`: local inputs and generated assets; never commit secrets.

## Flow

`document/slide/video -> chunks -> concepts/relations -> grounded graph -> quiz/learning response -> review/evaluation`

## Boundaries

- API validates input and delegates to domain modules.
- Domain modules own schemas and decisions; UI does not implement AI policy.
- Retrieval/grounding must expose source metadata.
- Evaluation is read-only against fixtures; production data is isolated.

