---
title: Trellis
source: https://github.com/mindfold-ai/Trellis
author: mindfold-ai
published:
created: 2026-04-14
description: GitHub repository README snapshot imported for local traceability.
tags:
source_type: repo
bundle_name: 2026-04-14-github-mindfold-ai-trellis
imported_from: GitHub repository homepage README snapshot
---

# mindfold-ai/Trellis

The best agent harness.

## Overview

A multi-platform AI coding framework that rules.

Supports Claude Code, Cursor, OpenCode, iFlow, Codex, Kilo, Kiro, Gemini CLI, Antigravity, Windsurf, Qoder, CodeBuddy, and GitHub Copilot.

Docs:

- https://docs.trytrellis.app
- https://docs.trytrellis.app/quick-start
- https://docs.trytrellis.app/supported-platforms
- https://docs.trytrellis.app/use-cases

## Why Trellis?

- Auto-injected specs: write conventions once in `.trellis/spec/`, then let Trellis inject the relevant context into each session.
- Task-centered workflow: keep PRDs, implementation context, review context, and task status in `.trellis/tasks/`.
- Parallel agent execution: run multiple AI tasks side by side with git worktrees.
- Project memory: journals in `.trellis/workspace/` preserve prior context.
- Team-shared standards: specs live in the repo and can be reviewed like normal project artifacts.
- Multi-platform setup: one Trellis structure can be reused across many AI coding tools.

## Prerequisites

- Node.js >= 18
- Python >= 3.10

## Quick Start

```bash
# 1. Install Trellis
npm install -g @mindfoldhq/trellis@latest

# 2. Initialize in your repo
trellis init -u your-name

# 3. Or initialize with the platforms you actually use
trellis init --cursor --opencode --codex -u your-name
```

Notes:

- `-u your-name` creates `.trellis/workspace/your-name/` for journals and continuity.
- Supported platform flags include `--cursor`, `--opencode`, `--iflow`, `--codex`, `--kilo`, `--kiro`, `--gemini`, `--antigravity`, `--windsurf`, `--qoder`, `--codebuddy`, and `--copilot`.

## Use Cases

- Teach AI your project once by putting coding standards, file structure rules, review habits, and workflow preferences into markdown specs.
- Run multiple AI tasks in parallel with git worktrees and Trellis task structure.
- Turn project history into usable memory with task PRDs, checklists, and workspace journals.
- Keep one workflow across tools when teams use more than one AI coding tool.

## How It Works

Trellis keeps the core workflow in `.trellis/` and generates platform-specific entry points around it.

```text
.trellis/
├── spec/                    # Project standards, patterns, and guides
├── tasks/                   # Task PRDs, context files, and status
├── workspace/               # Journals and developer-specific continuity
├── workflow.md              # Shared workflow rules
└── scripts/                 # Utilities that power the workflow
```

Depending on enabled platforms, Trellis also creates integration files such as `.claude/`, `.cursor/`, `AGENTS.md`, `.agents/`, `.codex/`, `.kilocode/`, `.kiro/`, `.github/copilot/`, and `.github/hooks/`.

High-level workflow:

1. Define standards in specs.
2. Start or refine work from a task PRD.
3. Let Trellis inject the right context for the current task.
4. Use checks, journals, and worktrees to keep quality and continuity intact.

## Spec Templates & Marketplace

- Templates are empty by default and meant to be customized.
- Custom registries are supported, for example:

```bash
trellis init --registry https://github.com/your-org/your-spec-templates
```

## What's New

- v0.3.6: task lifecycle hooks, custom template registries, parent-child subtasks, hook fixes
- v0.3.5: Kilo workflow migration hotfix
- v0.3.4: Qoder support, Kilo workflow migration, record-session task awareness
- v0.3.1: background watch mode for `trellis update`, improved `.gitignore` handling
- v0.3.0: platform support expansion, Windows compatibility, remote spec templates, `/trellis:brainstorm`

## FAQ Highlights

- Trellis differs from plain `CLAUDE.md`, `AGENTS.md`, or `.cursorrules` by adding layered specs, task context, workspace memory, and platform-aware workflow wiring.
- Trellis is not only for Claude Code; it supports multiple AI coding platforms.
- Teams can use it without constant conflicts because personal journals stay separate while shared specs and tasks remain in-repo.
