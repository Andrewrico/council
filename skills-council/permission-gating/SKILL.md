---
name: permission-gating
description: Propose explicit, scoped permission sets (ask/allow/deny, glob-scoped) for any recommended execution; never rely on an executor's defaults.
metadata:
  source-operator: opencode (james-b)
  selected-by: council-capability-matrix.md (Stage 2 SELECT, 2026-07-02)
---

# permission-gating

**Inherited from:** `opencode (james-b)` — selected as the best verified implementation of this
dimension in the Stage 2 capability matrix.

## What Council does with it (advisory-only)

- Every execution recommendation names its minimum toolset and an explicit deny list.
- Call out when a target executor's default would be broader than the proposal.

## Evidence (files actually read)

opensrc-verified: packages/opencode/src/permission/index.ts (fallback ask, wildcard scoping), tool/plan.ts (plan_exit gate). CAVEAT verified: default build agent ships "*": "allow" — advisory-first is opt-in.

> Council is DORMANT (PLAN_ONLY floor). This skill informs recommendations; it never
> authorizes execution. See ../../CONSTITUTION.md.
