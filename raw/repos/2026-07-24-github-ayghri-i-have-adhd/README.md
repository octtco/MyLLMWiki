<p align="center">
  <strong>ADHD-friendly outputs. No ADHD diagnosis needed!</strong>
</p>

## Install

### Claude Code

```bash
claude plugin marketplace add ayghri/i-have-adhd
claude plugin install i-have-adhd@i-have-adhd
```

Then type `/i-have-adhd`. To apply it on every session, create
`~/.claude/.i-have-adhd-always`.

### Codex

```bash
codex plugin marketplace add ayghri/i-have-adhd --ref main
codex plugin add i-have-adhd@i-have-adhd
```

Then type `$i-have-adhd` to apply the output style explicitly. The skill can
also be invoked implicitly when Codex sees a task that benefits from it.

## What it does

A skill for coding assistants that stops them from burying the answer. Action
first. Steps numbered. No preamble or closing filler.

## The rules

1. Lead with the next action.
2. Number multi-step tasks.
3. End with one concrete next step.
4. Suppress tangents.
5. Restate state every turn.
6. Give specific time estimates in minutes.
7. Make wins visible.
8. State errors matter-of-factly.
9. Cap lists at 5 items.
10. Remove preambles, recaps, and closers.

## Tune it

Fork the repository, edit `skills/i-have-adhd/SKILL.md`, then install the fork
as the marketplace source. The project is intended to be adapted to a user's
preferred coding-agent host and output style.

## Credits

Loosely based on *The Adult ADHD Tool Kit* by J. Russell Ramsay and Anthony L.
Rostain. It is adapted for how an LLM should respond, not how a human should
organize their day.

## License

MIT.
