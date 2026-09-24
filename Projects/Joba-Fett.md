---
type: project
name: Joba-Fett
status: active
area: product
priority: high
started: 2026-09-23
---

# Joba-Fett

## Goal
Job-application pipeline: Rover sweeps external boards → internal job board →
James hand-selects → per-job config (Aggression, Industry, Persona, Personal
Connection) → Scout vs Direct fork → Bundle → Applier → follow-up. Grok bots do
research/speccing, Cursor builds, James holds the sign-off gates.

## Current state
Pipeline v2 spec written (JobHuntr/Project Docs/) but the token 403s on
`joba-fett`, so the spec was handed to James directly. Awaiting his word:
kick off grok-bot research briefs or a Cursor Phase 0 brief.

## Open tasks

```dataview
TABLE status AS Status, due AS Due, priority AS Priority
FROM "Tasks"
WHERE type = "task" AND contains(string(project), "Joba-Fett") AND status != "done"
SORT due ASC
```

## Log
- 2026-09-23: pipeline v2 spec completed; handed to James directly (repo write 403)
