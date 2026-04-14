# quarry

All work is just different sized rocks. Break them. Move them.

Quarry is a Claude Code plugin that injects a structured task management workflow — capture rough ideas, refine and score them, then execute one rock at a time until the backlog is clear.

## Installation

Add the jehoshua02 marketplace and install the plugin using the `/plugin` command in Claude Code:

```
/plugin add-marketplace jehoshua02
/plugin install quarry
```

## What it does

Injects project management workflow rules into Claude's context via `SessionStart` hook:

- **Capture** — drop rough ideas into `project/0-inbox/` before they vanish
- **Refine** — Q&A loop to score each task on Value, Momentum, Effort, and Risk
- **Prioritize** — formula-based scoring, lower is higher priority
- **Execute** — structured pipeline: inbox → todo → doing → done
