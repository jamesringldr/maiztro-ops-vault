# Maiztro Ops

## Active projects

```dataview
TABLE status AS Status, priority AS Priority, area AS Area, started AS Started
FROM "Projects"
WHERE type = "project" AND status = "active"
SORT priority DESC
```

## Paused projects

```dataview
TABLE priority AS Priority, area AS Area
FROM "Projects"
WHERE type = "project" AND status = "paused"
SORT priority DESC
```

## Tasks — up next

```dataview
TABLE project AS Project, status AS Status, due AS Due, priority AS Priority
FROM "Tasks"
WHERE type = "task" AND status != "done"
SORT due ASC
```

## Done recently

```dataview
TABLE project AS Project
FROM "Tasks"
WHERE type = "task" AND status = "done"
SORT file.mtime DESC
LIMIT 10
```
