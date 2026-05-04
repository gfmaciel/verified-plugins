# one-page-creator

This plugin helps teams create a concise one-pager to get manager buy-in for adopting Claude Code automation.

## When to use

Invoke `/one-page-creator` when a developer or team lead wants to pitch Claude Code automation to a manager or decision-maker who controls budget, time, or headcount approvals.

## How it works

The skill asks 3–4 targeted questions to understand the team's context, then generates a filled one-pager ready to send or print.

**Questions asked:**
1. Team size and main role (devs, QA, data, etc.)
2. Top 2–3 pain points (repetitive tasks, slow reviews, manual docs, etc.)
3. Manager's known priorities (shipping faster, reducing bugs, cutting costs, etc.)
4. Any deadline or timeline pressure

**Output:** A complete one-pager in markdown covering the problem, the solution, expected ROI, a low-risk pilot proposal, and the specific ask.

## Usage

```
/one-page-creator
```

No arguments required. The skill will prompt for the information it needs.

## Output format

The generated one-pager follows this structure:

- **The Problem** — what the team is struggling with today
- **The Solution** — what Claude Code automates and how
- **Expected ROI** — time saved per week, estimated
- **Low-Risk Pilot** — a concrete 2-week trial with a success metric
- **The Ask** — exactly what is needed from the manager (usually just time, no budget)
