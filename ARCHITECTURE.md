# Architecture Overview

## Components

### Claude (Orchestrator)
- Platform: claude.ai or Claude Desktop
- Role: Receives user requests, creates GitHub issues, reviews PRs
- Tools: GitHub MCP connector, Filesystem MCP (Desktop only)

### GitHub (Message Bus)
- Issues = task definitions with acceptance criteria
- PRs = code changes ready for review
- Single source of truth for all tasks

### GitHub Copilot Agent (Executor)
- Reads GitHub issues, writes code, opens PRs
- Assigned directly to issues by Claude

### Local LLM Stack (Optional)
- **LM Studio** (port 1234): runs local models (Qwen, etc.)
- **pattern_system proxy** (port 1235): routes OpenCode → Gemini/Groq/Cerebras/LMStudio
- **stack-rag** (port 8000): FastMCP SSE semantic search over Python functions

## Design Principles

1. **GitHub as single source of truth** — all tasks live as issues
2. **Small atomic changes** — one issue = one PR = one concern
3. **Human in the loop** — PRs always reviewed before merge
4. **Local-first** — prefer local models over cloud
5. **Transparency** — all AI actions traceable via GitHub history
