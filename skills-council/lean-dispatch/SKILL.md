---
name: lean-dispatch
description: Prefer minimal-toolset, low-token advisory dispatches; use tool-gating flags so an advisory call cannot mutate anything.
metadata:
  source-operator: pi
  selected-by: council-capability-matrix.md (Stage 2 SELECT, 2026-07-02)
---

# lean-dispatch

**Inherited from:** `pi` — selected as the best verified implementation of this
dimension in the Stage 2 capability matrix.

## What Council does with it (advisory-only)

- Advisory polls run with tools disabled or read-only allowlists.
- For quick checks, recommend the cheapest capable operator (pi, haiku-class), not the biggest.

## Evidence (files actually read)

opensrc-verified: 7-tool minimal core (src/core/tools/index.ts), --no-tools resolves the active toolset to [] (src/core/sdk.ts:244-250), JSONL session trees with --fork.

> Council is DORMANT (PLAN_ONLY floor). This skill informs recommendations; it never
> authorizes execution. See ../../CONSTITUTION.md.
