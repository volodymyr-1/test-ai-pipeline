# Copilot Instructions — test-ai-pipeline

## Project Purpose
Automated AI development pipeline: Claude creates GitHub Issues → Copilot Agent writes code → Pull Request opened → Human reviews & merges.

## Pipeline Flow
```
Claude (claude.ai) → GitHub Issue → Copilot Agent → Pull Request → Review & Merge
```

## Key Conventions

### When creating files
- Always place source code in `src/`
- Tests go in `tests/`
- Documentation in root or `docs/`

### Branch naming
- `feature/short-description`
- `fix/short-description`
- `docs/short-description`

### Commit messages
- `feat:` new feature
- `fix:` bug fix
- `docs:` documentation update
- `chore:` maintenance

### Pull Requests
- Title must match the issue title
- Body must reference the issue: `Closes #<issue_number>`
- Keep PRs small and focused — one issue = one PR

## Local Stack Context
- LM Studio runs at localhost:1234 (local LLM server)
- pattern_system proxy at localhost:1235 (routes to Gemini/Groq/LMStudio)
- stack-rag at localhost:8000 (semantic search over Python functions)

## Important
- Every task starts as a GitHub Issue
- Acceptance criteria must be checked before closing issue
- Human review is required before merging any PR
