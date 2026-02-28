---
name: simple-brainstorm
description: "Invoke before any creative or architectural work — feature design, component creation, or behavioral changes. A streamlined brainstorming process optimized for fast, focused decision-making."
---

# Simple Brainstorm

A structured yet lightweight brainstorming skill designed to move from idea to actionable direction quickly. It preserves the rigor of collaborative design — exploring intent, evaluating trade-offs, and validating decisions — while eliminating process overhead that doesn't scale to small and medium tasks.

## Gate

Do NOT write any code, scaffold any files, or take any implementation action until the user has explicitly approved a direction.

## Process

1. **Discover** — Assess project context (codebase, conventions, existing patterns). Ask up to 3 targeted questions to clarify intent, constraints, and success criteria. Prefer multiple-choice where possible. Batch related questions into a single message.

2. **Propose** — Present 2 distinct approaches with concrete trade-offs. Lead with your recommendation and state why. Keep each option to 2–3 sentences — enough to inform, not enough to overwhelm.

3. **Converge** — Obtain explicit user approval on an approach. If rejected, offer revised alternatives. Limit to two proposal rounds — if alignment isn't reached, ask the user to state their preferred direction directly.

4. **Capture** — Record the chosen approach (what, why, key decisions) as a brief inline comment in the first implementation file, or surface it in chat. No separate design document unless the user requests one.

## Principles

- **Speed over ceremony** — Minimize overhead. Reserve formal design artifacts for work that genuinely warrants them.
- **YAGNI** — Design only for current requirements. Resist speculative abstractions.
- **Bias toward action** — When options are comparably viable, commit to one and proceed. Indecision costs more than imperfection.
- **Batched discovery** — Consolidate clarifying questions into a single round. Avoid drawn-out back-and-forth.
- **Proportional depth** — Scale the process to the task. Trivial changes can complete steps 1–2 in a single message; larger efforts merit fuller exploration in step 2.
