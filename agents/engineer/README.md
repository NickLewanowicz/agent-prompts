# Engineer Agent

## Overview

This agent is designed to act as a senior software engineer, autonomously handling GitHub issues, implementing solutions, and preparing code for review. It is optimized for use in Cursor and similar AI development environments.

## Usage in Cursor

- **Prompt Location:** Use the `prompt.md` in this directory as the system prompt for your agent.
- **Recommended Model:** Works best with a large reasoning model such as `claude-4-sonnet` or equivalent.
- **Access:** Grant the agent auto access to all files, code, and tools for maximum productivity.

## Required MCPs

- **GitHub MCP:** The agent requires the GitHub MCP for all standard Git and GitHub operations (branching, committing, PRs, etc.).
- **Other MCPs:** Any additional MCPs needed for your workflow (e.g., file system, shell, or project management MCPs) can be enabled as required.

## Key Features

- **Worktree-Based Workflow:** Enforces worktree usage for all feature development to enable parallel work streams.
- **Branch-Only Development:** Strict branch-based workflow—never commits directly to `main`.
- **Comprehensive Testing:** Requires at least 80% test coverage for all changes.
- **6-Step Opinionated Process:** Branch/worktree setup → Implementation → Testing → Validation → Commit/Push → PR creation.
- **Pull Request Protocol:** Uses a detailed PR template with testing instructions and checklist.

## Workflow Summary

1. **Branch & Worktree Management** - Verify git status and create worktree with new branch
2. **Implementation** - Minimal changes, clear naming, no comments
3. **Write Tests** - 80% coverage with clear describe blocks
4. **Validate** - Run tests and linting
5. **Commit & Push** - Conventional commits
6. **Create PR** - Comprehensive PR description

## Best Practices

- Always use the latest, most capable reasoning model available.
- Ensure all required MCPs are enabled before starting a session.
- Grant the agent full access to the repository for seamless operation.
- The agent will create worktrees by default—this is the expected workflow.

---

For more details, see the full prompt in `prompt.md`.
