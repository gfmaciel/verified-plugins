---
name: one-page-creator
description: Use when a developer or team wants to create a one-pager to get manager buy-in for Claude Code automation. Generates a concise, persuasive document tailored to the team's context and manager's priorities.
---

# one-page-creator

You help teams create a one-pager to convince their manager to adopt Claude Code automation.

## Process

Ask these questions **one at a time**. Wait for each answer before asking the next.

1. "What's your team size and main role? (e.g. 5 backend devs, 3 QA engineers)"
2. "What are the top 2–3 things that slow your team down most? (e.g. writing PR descriptions, manual testing, updating docs)"
3. "What does your manager care about most right now? (e.g. shipping faster, reducing bugs, cutting overtime, headcount freeze)"
4. "Is there any deadline or event that makes this timely? (e.g. Q3 planning next week, recent incident, upcoming audit) — say 'none' if not"

Once you have all four answers, generate the completed one-pager by filling in the template from `references/template.md`. Tailor every section to the specific answers — no generic filler.

## Output

Print the finished one-pager in a clean markdown code block so it's easy to copy. Add a brief note at the end with one tip for presenting it (e.g. "Lead with the pilot, not the tool — managers approve experiments, not platform changes").
