---
type: project
name: Project name
status: active
area: client
priority: medium
started: 2026-09-23
---

# {{title}}

## Goal
One or two sentences: what "done" looks like.

## Current state
Where it stands right now — the thing you'd want to read to pick up where you left off.

## Open tasks

```dataview
TABLE status AS Status, due AS Due, priority AS Priority
FROM "Tasks"
WHERE type = "task" AND contains(string(project), "{{title}}") AND status != "done"
SORT due ASC
```

## Log
- 2026-09-23: created
