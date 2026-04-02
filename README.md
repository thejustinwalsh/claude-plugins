# Claude Code Plugins — @thejustinwalsh

A marketplace of Claude Code plugins by Justin Walsh.

## Install

```bash
/plugin marketplace add thejustinwalsh/claude-plugins
```

Then install any plugin:

```bash
/plugin install restruct@thejustinwalsh
/plugin install ghostty-notify@thejustinwalsh
```

## Plugins

### restruct

Meta-prompt refinement via local LLM. Intercepts every prompt, runs it through a local Ollama model (qwen2.5-coder:14b) that classifies your request against your project's CLAUDE.md rules, and injects structured context that keeps Claude on-task.

- Local-only — no data leaves your machine
- Bootstraps project context at session start
- Real-time dashboard for monitoring refinements, tool decisions, and verifications
- Retrieval-augmented rule selection from multiple CLAUDE.md files

**Requires:** [Ollama](https://ollama.com) running locally.

```bash
/plugin install restruct@thejustinwalsh
/restruct:setup
```

### ghostty-notify

Native macOS notifications for Claude Code when running in the Ghostty terminal. Get notified when long-running tasks complete, with automatic tab focusing.

```bash
/plugin install ghostty-notify@thejustinwalsh
```
