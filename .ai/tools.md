# Graph4life Tool Policy

## Allowed

- Inspect: `Get-ChildItem`, `Get-Content`, `git status`, `git log`, `git diff`.
- Search: `rg` when available; otherwise PowerShell `Select-String`.
- Test: `pytest`, targeted pytest paths, and application smoke checks.
- Git: `git add`, `git commit`, branch inspection, and explicitly requested remote operations.
- Edit: repository files only; prefer patch-based edits.

## Boundaries

- Never print or commit `.env`, API keys, tokens, or personal data.
- No force-push, reset, mass deletion, or dependency/network action without explicit approval.
- MCP/external tools may be used only for the requested service and must not bypass tests or repository boundaries.

