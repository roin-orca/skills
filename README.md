# skills

Simplified Claude Code skills for faster work and decision making.

## simple-brainstorm

A streamlined version of [obra's brainstorming skill](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md), built for speed and short sessions.

Obra's original skill is thorough — it walks through a multi-step discovery process, asks one question at a time, produces a full design document, and commits it to `docs/plans/`. That's great for large, ambiguous projects where upfront design pays off.

But in practice, I found that for many real-world tasks, the ceremony slowed things down more than it helped. So I built `simple-brainstorm` — a stripped-down version that keeps the good parts (structured thinking, exploring alternatives, getting approval before coding) and drops the overhead (sequential single-question discovery, mandatory design docs, rigid multi-phase flow).

### Where simple-brainstorm performed better for me

After testing both skills across multiple sessions, `simple-brainstorm` consistently outperformed the original for:

- **Quick feature additions** — Adding a new endpoint, UI component, or config option where the scope is already mostly clear. The original skill's one-question-at-a-time flow added 5-10 extra back-and-forth messages before any real decision was made.
- **Bug fix planning** — When you already know the bug and need to decide between 2-3 fix strategies. The full brainstorming process felt like overkill when the problem space was already well-understood.
- **Short coding sessions (< 30 min)** — When you have limited time, spending half of it on structured discovery and design docs leaves little room for actual implementation. Simple-brainstorm gets to a decision in 1-2 messages.
- **Refactoring decisions** — Choosing between refactoring approaches (extract function vs. inline, rename vs. restructure) where the trade-offs are straightforward and a brief comparison is all you need.

### When to use obra's original instead

For large greenfield projects, complex architectural decisions, or work that multiple people need to review — the full brainstorming skill with its design docs and thorough discovery process is still the better choice.

## Installation

Copy the `skills/simple-brainstorm` directory into your project's `.claude/skills/` folder, or reference it directly.
