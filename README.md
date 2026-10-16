# Yvoo Lab

AI automation engineering — Claude Code power tools, agent pipelines, and the boring-but-critical glue that lets LLMs run unattended in production.

Everything below is extracted from a real multi-machine setup that runs Claude Code daily: scheduled headless agents, cross-machine session handoff, guardrail hooks that have each earned their place by preventing (or surviving) a real incident.

## Claude Code toolbox

| Repo | What it solves |
|---|---|
| [claude-code-cron](https://github.com/yvoolab/claude-code-cron) | Run Claude Code unattended on a schedule — runner script, git-push distributed lock for multi-machine setups, failure alerts, hard-boundary prompt template |
| [claude-code-safety-hooks](https://github.com/yvoolab/claude-code-safety-hooks) | Guardrail hooks: confirmation gate for dangerous commands (`rm -rf`, force-push, `DROP TABLE`, destructive MCP calls), secret-hardcoding blocker, and an ASCII gate that stops CJK bytes from corrupting `.cmd` files |
| [claude-code-session-sharing](https://github.com/yvoolab/claude-code-session-sharing) | Hand off in-progress Claude Code sessions between machines — auto-snapshot on Stop hook, LLM summary, git sync |
| [claude-code-windows-hook](https://github.com/yvoolab/claude-code-windows-hook) | Working Node.js hook template for Claude Code on Windows — bypasses the known bash-hook bugs |
| [claude-code-windows-screenshot-paste](https://github.com/yvoolab/claude-code-windows-screenshot-paste) | 28-line AutoHotkey fix for "No image found in clipboard" when pasting screenshots into Claude Code on Windows ([#68021](https://github.com/anthropics/claude-code/issues/68021)) |
| [claude-code-todo-digest](https://github.com/yvoolab/claude-code-todo-digest) | Every repo's TODO backlog, one nightly email — GitHub Action + zero-LLM summarizer with staleness flags |
| [linux-voice-input-zh](https://github.com/yvoolab/linux-voice-input-zh) | Push-to-talk Chinese voice input for any Linux app — 351 lines of Python, €0 to run (Groq free tier) |

## Working with me

Freelance data scientist & AI engineer — France, remote. Python · TypeScript · Claude API · ML & RAG · agent orchestration · workflow automation. In tech since 2022, data science since 2025, LLM and agent systems since 2026.

Open to missions. Reach out through any repo's issues or the links on this profile.
