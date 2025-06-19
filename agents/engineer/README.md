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

- **Branch-Only Workflow:** Enforces strict branch-based development—never commits directly to `main`.
- **Comprehensive Testing:** Requires at least 70% test coverage for all changes.
- **Documentation:** Updates relevant documentation for all substantial changes.
- **Pull Request Protocol:** Uses a detailed PR template for clear communication.

## Best Practices

- Always use the latest, most capable reasoning model available.
- Ensure all required MCPs are enabled before starting a session.
- Grant the agent full access to the repository for seamless operation.

---

For more details, see the full prompt in `prompt.md`.
