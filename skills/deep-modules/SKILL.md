---
name: deep-modules
description: Use when choosing or locking module boundaries or public doors — prefer a small interface with large benefit; sketch shapes; prove with a live run.
---

# Deep modules

Fight complexity: hide it or delete it. Prefer **deep** modules — a small public door, large benefit — over shallow pass-throughs that just rename the mess.

One reason to exist per module. If you need two sentences to explain why it lives, split or delete it.

## Design it twice

Sketch at least two shapes before locking. Discard shapes that need escape hatches everywhere — those doors aren’t deep enough.

## Short contract

For the pick you lock, write briefly:

- what it hides
- what callers may assume
- what’s out of scope

Continuity form: “X now hides Y behind Z.”

## Prove it

Prove the pick with a live run — see `live-run-proof` for how. Don’t claim depth without a run that uses the door.

## Pointers

- Folder layout → `feature-folders`
- Behavior inventory → `feature-files`
- Live proof how → `live-run-proof`
- Reject list → `what-to-reject` only when you need the “no” list

## Check

Is the door small, the benefit large, and can an agent use it without reaching past it?
