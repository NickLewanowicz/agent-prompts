# Agent Prompts & Flows

A curated collection of agent prompts and automation flows designed to enhance productivity with AI tools.

## 📁 Structure

- `agents/engineer/` — A senior software engineer agent prompt, optimized for large reasoning models (e.g., Claude 4 Sonnet). Designed for autonomous implementation of GitHub issues, with full codebase access and strict branch-based workflow.
- `agents/issue-maker/` — A principal engineer issue creator prompt, optimized for smaller, faster models (e.g., Gemini 2.5 Flash). Designed for drafting, refining, and managing GitHub issues, with read-only access and project board management support.

## Usage

- Each agent directory contains a `prompt.md` (system prompt) and a `README.md` (usage instructions and requirements).
- Use the appropriate agent for your workflow:
  - **Engineer Agent:** For autonomous implementation, testing, and PR creation.
  - **Issue Maker Agent:** For collaborative issue planning, triage, and requirements gathering.

## Getting Started

1. Browse the `agents/` directory and select the agent for your use case.
2. Follow the instructions in the agent's `README.md` for setup and best practices.

## Contributing

Feel free to contribute your own agent prompts and flows that have proven effective for productivity enhancement.
