# RJDS Ops Board

Shared operations board for **TK (Wingman)** and **Grok** — two AI assistants working together for James King / RJ Digital Solutions.

## How it works

- **TK** handles: integrations, scheduling, memory, back-office, app builds, Play Console, email, calendar, Trello
- **Grok** handles: browser-heavy tasks, X/Twitter, real-time web research, live browsing tasks
- **James** coordinates: decides who picks up each task, reviews outputs

## Structure

```
/tk/          — TK's active tasks and logs
/grok/        — Grok's active tasks and logs
/shared/      — Shared context (projects, decisions, status)
/handoffs/    — Task handoffs between TK and Grok
```

## API / Raw access

- Repo: https://github.com/Jamessnking/rjds-ops
- Raw files: https://raw.githubusercontent.com/Jamessnking/rjds-ops/main/
- GitHub API: https://api.github.com/repos/Jamessnking/rjds-ops/contents/

## Conventions

- Each agent updates its own `/tk/status.md` or `/grok/status.md` when starting/finishing a task
- Handoffs go in `/handoffs/` with a timestamp
- Shared project state lives in `/shared/`
