---
type: project
name: Bloom Early Learning Center
status: active
area: client
priority: high
started: 2026-09-23
---

# Bloom Early Learning Center

## Goal
Website (plus possible app) for Bloom, a commercial daycare in Lenexa, KS (ages
6 weeks–6 years); alongside it, consulting/fractional COO-CFO work. Manual pilot
of Maiztro's new ingestion process — friction notes feed Focus 3.

## Current state
Director plan v1 + Cursor build brief approved 2026-09-23. Hosting: Vercel.
Asset pack (logo, Blossom mascot, tuition table, building photo, copy docs,
brief) zipped and handed to James; dispatched to Cursor. Awaiting the build,
then James's sign-off gate before deploy.

## Open tasks

```dataview
TABLE status AS Status, due AS Due, priority AS Priority
FROM "Tasks"
WHERE type = "task" AND contains(string(project), "Bloom Early Learning Center") AND status != "done"
SORT due ASC
```

## Log
- 2026-09-23: director plan + build brief approved; asset pack delivered; build dispatched to Cursor
