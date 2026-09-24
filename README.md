> **What this is:** maiztro-ops as an Obsidian vault — a high-level project tracker plus a task tracker, plain markdown throughout · **Created:** 2026-09-23 · **Status:** ready to open

# maiztro-ops (Obsidian vault)

Fresh start, deliberately basic: one note per project, one note per task, one
note per idea, and a `Home.md` dashboard that rolls them up. No build step, no
server — open the folder in Obsidian and it works. Same markdown format Holocron
is specced to use, so the two can share one vault later if you want.

## Setup (3 steps, ~2 minutes)

1. Unzip and open this folder as a vault in Obsidian (`Open folder as vault`).
2. Install + enable the **Dataview** community plugin (Settings → Community
   plugins). This is the only community plugin the dashboards need.
3. Point the core **Templates** plugin at the `Templates` folder
   (Settings → Templates → Template folder location).

Then open `Home.md` and pin it. That's the dashboard.

## Conventions

- **Projects/** — one note per project. Frontmatter: `status` is
  `active`, `paused`, or `done`.
- **Tasks/** — one note per task. Frontmatter: `status` is `todo`, `doing`,
  or `done`; `project` links back to its project note; `due` is a date or blank.
- **Ideas/** — the drop zone. Half-formed thoughts, feature sparks, whole new
  projects — don't polish them. Frontmatter: `status` is `inbox`, `someday`,
  `promoted`, or `dropped`; `project` links to a project if the idea belongs to
  one, blank if it's free-floating. When an idea grows up, make the project or
  task note, link it under "Promoted to", and flip the idea to `promoted`. It
  drops off the Home dashboard automatically, same as done tasks.
- New project / new task / new idea: `Ctrl/Cmd+P` → "Templates: Insert template" → pick
  the template. Fill in the frontmatter, done.
- Archive: set a project or task to `done`. It drops off the active dashboards
  automatically and shows under "Done recently" on Home.
