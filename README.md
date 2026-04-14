# claude-plugin-quarry

Quarry is a Claude Code plugin that injects a structured task management workflow into Claude's context. Capture, break, refine, prioritize, and execute — from raw ideas to shipped work.

The name comes from the analogy: a quarry extracts raw material. You capture rough ideas, break them into rocks, refine them, and ship them.

## What it does

Injects `quarry.md` into `~/.claude/rules/` via a `SessionStart` hook. Claude picks up the workflow rules automatically on session start.

## What it includes

- Prioritization formula (Value, Momentum, Effort, Risk)
- Four-stage pipeline: inbox → todo → doing → done
- Workflow steps: capture, refine, pick up, complete
- Task file template

## What it doesn't include

Folder setup. Each project manages its own `project/0-inbox/`, `project/1-todo/`, `project/2-doing/`, `project/3-done/` directories.

## Installation

Install via `claude-marketplace` or manually:

```bash
cp rules/quarry.md ~/.claude/rules/quarry.md
```

Or register the plugin so the `SessionStart` hook runs automatically.
