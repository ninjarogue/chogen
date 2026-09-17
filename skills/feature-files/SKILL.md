---
name: feature-files
description: Use when adding or updating a behavior inventory so agents can open one piece at a time; one file per area; answer the four questions; keep checks fresh.
---

# Feature files

Pretty folders are not enough. The repo is agent memory — keep a scoped behavior inventory agents can open narrowly.

One feature file per area (sits with the folder layout from `feature-folders`). Prefer opening the one file for the change under test, not the whole corpus.

## Four questions

Each feature file answers:

1. **What exists?** — the capability and its pieces.
2. **How do you reach it?** — entry points, routes, doors.
3. **How do you drive it?** — the checks or driver that exercise it.
4. **What usually lies?** — stale paths, false greens, traps that waste runs.

## Drift

When behavior or UI shifts, update that feature file in the same change — or run a maintain pass soon after. Stale inventory is worse than none.

## Pointers

- Folder layout → `feature-folders` (don't merge folder rules here).
- How to prove a run live → `live-run-proof` when you need the full how.

## Check

Can an agent answer the four questions for this area from one file, then drive it without hunting?
