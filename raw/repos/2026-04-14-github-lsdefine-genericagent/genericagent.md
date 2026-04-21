---
title: GenericAgent
source: https://github.com/lsdefine/GenericAgent
author: lsdefine
published:
created: 2026-04-14
description: GitHub repository README snapshot imported for local traceability.
tags:
source_type: repo
bundle_name: 2026-04-14-github-lsdefine-genericagent
imported_from: GitHub repository homepage README snapshot
---

English | 中文

## Overview

GenericAgent is a minimal, self-evolving autonomous agent framework. Its core is just ~3K lines of code. Through 9 atomic tools + a ~100-line Agent Loop, it grants any LLM system-level control over a local computer — covering browser, terminal, filesystem, keyboard/mouse input, screen vision, and mobile devices (ADB).

Its design philosophy: don't preload skills — evolve them.
Every time GenericAgent solves a new task, it automatically crystallizes the execution path into an skill for direct reuse later. The longer you use it, the more skills accumulate — forming a skill tree that belongs entirely to you, grown from 3K lines of seed code.

> Self-Bootstrap Proof — Everything in this repository, from installing Git and running `git init` to every commit message, was completed autonomously by GenericAgent. The author never opened a terminal once.

## Core Features

- Self-Evolving: Automatically crystallizes each task into an skill. Capabilities grow with every use, forming your personal skill tree.
- Minimal Architecture: ~3K lines of core code. Agent Loop is ~100 lines. No complex dependencies, zero deployment overhead.
- Strong Execution: Injects into a real browser (preserving login sessions). 9 atomic tools take direct control of the system.
- High Compatibility: Supports Claude / Gemini / Kimi / MiniMax and other major models. Cross-platform.

## Latest News

- 2026-04-11: Introduced L4 session archive memory and scheduler cron integration
- 2026-03-23: Support personal WeChat as a bot frontend
- 2026-03-10: Released million-scale Skill Library
- 2026-03-08: Released "Dintal Claw" — a GenericAgent-powered government affairs bot
- 2026-03-01: GenericAgent featured by Jiqizhixin (机器之心)
- 2026-01-11: GenericAgent V1.0 public release

## Quick Start

```bash
# 1. Clone the repo
git clone https://github.com/lsdefine/GenericAgent.git
cd GenericAgent

# 2. Install minimal dependencies
pip install streamlit pywebview

# 3. Configure API Key
cp mykey_template.py mykey.py
# Edit mykey.py and fill in your LLM API Key

# 4. Launch
python launch.pyw
```

Full guide: GETTING_STARTED.md

## Comparison with Similar Tools

| Feature | GenericAgent | OpenClaw | Claude Code |
| --- | --- | --- | --- |
| Codebase | ~3K lines | ~530,000 lines | Open-sourced (large) |
| Deployment | `pip install` + API Key | Multi-service orchestration | CLI + subscription |
| Browser Control | Real browser (session preserved) | Sandbox / headless browser | Via MCP plugin |
| OS Control | Mouse/kbd, vision, ADB | Multi-agent delegation | File + terminal |
| Self-Evolution | Autonomous skill growth | Plugin ecosystem | Stateless between sessions |
| Out of the Box | A few core files + starter skills | Hundreds of modules | Rich CLI toolset |

## How It Works

GenericAgent accomplishes complex tasks through Layered Memory × Minimal Toolset × Autonomous Execution Loop, continuously accumulating experience during execution.

### 1. Layered Memory System

- L0 — Meta Rules: Core behavioral rules and system constraints of the agent
- L1 — Insight Index: Minimal memory index for fast routing and recall
- L2 — Global Facts: Stable knowledge accumulated over long-term operation
- L3 — Task Skills / SOPs: Reusable workflows for completing specific task types
- L4 — Session Archive: Archived task records distilled from finished sessions for long-horizon recall

### 2. Autonomous Execution Loop

Perceive environment state → Task reasoning → Execute tools → Write experience to memory → Loop

The entire core loop is just ~100 lines of code (`agent_loop.py`).

### 3. Minimal Toolset

GenericAgent provides only 9 atomic tools, forming the foundational capabilities for interacting with the outside world.

- `code_run` Execute arbitrary code
- `file_read` Read files
- `file_write` Write files
- `file_patch` Patch / modify files
- `web_scan` Perceive web content
- `web_execute_js` Control browser behavior
- `ask_user` Human-in-the-loop confirmation
- `update_working_checkpoint` Memory persistence
- `start_long_term_update` Long-term memory accumulation
