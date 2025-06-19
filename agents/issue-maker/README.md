# Issue Maker Agent

## Overview

This agent is designed to act as a senior issue creator and project planner, generating high-quality, actionable GitHub issues for software teams. It is optimized for use with smaller, faster models to encourage more discussion and rapid iteration.

## Usage in Cursor

- **Prompt Location:** Use the `prompt.md` in this directory as the system prompt for your agent.
- **Recommended Model:** Works best with smaller, faster models such as `gemini 2.5 flash` or similar.
- **Access:** When used in Cursor, this agent should be set to **read-only** mode and must not have edit access to the codebase or repository.

## Intended Workflow

- Use this agent to draft, refine, and manage GitHub issues.
- Designed to promote collaborative discussion and iterative refinement of requirements.
- Not intended for code changes—issues only.

## Required MCPs

- **GitHub MCP:** Required for creating and updating issues.
- **GH CLI:** Used for adding issues to project boards and updating status/fields.

## Best Practices

- Use for planning, triage, and requirements gathering.
- Pair with a more capable implementation agent (like the Engineer Agent) for full development workflows.
- Always keep the agent in read-only mode to ensure it cannot make code or documentation changes.

---

For more details, see the full prompt in `prompt.md`.
