---
type: project
name: Vanyshr Page Conversions
status: active
area: product
priority: medium
started: 2026-09-17
---

# Vanyshr Page Conversions

## Goal
Convert app pages to the integrated design bible (Konsta chrome + shadcn
content, token-only styling) now that the pilot loop is closed.

## Current state
Pilot loop closed; pages can convert. Queued: ~50 `text-[var(--text-primary)]`
call sites (migrate to `text-text-primary`) and the 6 hex-hook debt flags.
vanyshrdesignsys is now the whole-brand hub (public, branch protection live).

## Open tasks

```dataview
TABLE status AS Status, due AS Due, priority AS Priority
FROM "Tasks"
WHERE type = "task" AND contains(string(project), "Vanyshr Page Conversions") AND status != "done"
SORT due ASC
```

## Log
- 2026-09-17/18: bible integrated; pilot loop closed — conversions next
