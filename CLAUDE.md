# CLAUDE.md — Context for Claude AI Projects

> Load this file at the start of every session to restore full project context.
> In NotebookLM add as source: https://raw.githubusercontent.com/volodymyr-1/test-ai-pipeline/main/CLAUDE.md

## Project Overview

**Name:** test-ai-pipeline  
**Repo:** https://github.com/volodymyr-1/test-ai-pipeline  
**Purpose:** Automated pipeline — Claude creates issues → Copilot writes code → PR opened  
**Status:** 🚧 Active testing

## Pipeline Architecture

```
Claude (claude.ai)
  └─ Creates GitHub Issue (via MCP GitHub connector)
        └─ GitHub Copilot Agent reads issue
              └─ Writes code / files
                    └─ Opens Pull Request
                          └─ Review & Merge
```

## Key Conventions

- Issues: clear title + acceptance criteria + label + assignee: volodymyr-1
- Branches: feature/ fix/ docs/
- Commits: feat: / fix: / docs: / chore:

## Local Stack

| Service | URL | Notes |
|---|---|---|
| LM Studio | localhost:1234 | Local LLM server |
| pattern_system proxy | localhost:1235 | OpenAI proxy → Gemini/Groq/LMStudio |
| stack-rag | localhost:8000 | FastMCP SSE semantic search |

## Notes for Claude

- Always create issues via GitHub MCP tool
- One issue = one PR = one concern
- Each issue must have clear acceptance criteria
