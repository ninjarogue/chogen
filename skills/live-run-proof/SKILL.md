---
name: live-run-proof
description: Use when proving a design isn’t paper-only — spikes, happy-path script, agent-as-proof, break-on-purpose, real path; tests alone are not enough.
---

# Live-run proof

A design on paper isn’t proven. Run these six. Unit tests green alone ≠ live proof — tests can bless a shallow wrapper.

## 1. Two throwaway spikes

Spike two alternate doors. Keep the one that keeps the caller dumb. Reject shapes that need `any`, casts, or one-off knobs to work.

## 2. Script the happy path

Script create → use → finish until it’s boring. No secret call order. No glue state the caller must remember.

## 3. Agent-as-proof

Hand an agent only the contract plus the feature folder. Redesign if it needs chat context or sprays escape hatches to finish.

## 4. Break on purpose

Empty input, double-submit, missing config. A deep door absorbs failures inside — the caller shouldn’t patch around them.

## 5. Drive the real path

Drive the real UI/product path once (or record it). Proof is whether the door makes that journey boring to automate.

## 6. Tests aren’t enough

Green unit tests alone do not count. They can pass on a shallow pass-through. Live proof needs a run through the door.

## Pointers

- Depth / doors → `deep-modules`
- Folder layout → `feature-folders`
- Behavior inventory → `feature-files`

## Check

Would an agent finish create→use→finish with only the contract and folder — no chat, no escape hatches, no secret glue?
