---
name: build-safety-handoff
description: Recommend the orchestrate coding lane so every code handoff inherits the build-safety gate, git-worktree staging, and the logged MAIS handoff.
metadata:
  source-operator: cursor-agent
  selected-by: council-capability-matrix.md (Stage 2 SELECT, 2026-07-02)
---

# build-safety-handoff

**Inherited from:** `cursor-agent` — selected as the best verified implementation of this
dimension in the Stage 2 capability matrix.

## What Council does with it (advisory-only)

- Coding work → recommend `orchestrate "<task>"` (Marco lane); never a direct write path.
- Require pre-land tsc + boot-verify before calling a code change done.
- Flag any dispatch that would bypass the gate as a governance risk.

## Evidence (files actually read)

Ranking benchmark finding 1: gate/worktree/MAIS-handoff are properties of the orchestrate dispatcher; registry capability worktree-isolation; 19 harvested skills (review, split-to-prs).

> Council is DORMANT (PLAN_ONLY floor). This skill informs recommendations; it never
> authorizes execution. See ../../CONSTITUTION.md.
