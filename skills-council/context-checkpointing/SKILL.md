---
name: context-checkpointing
description: Recommend checkpoint/resume patterns for long or risky tasks: durable task context, reversible checkpoints, strict propose-vs-execute gating.
metadata:
  source-operator: cline
  selected-by: council-capability-matrix.md (Stage 2 SELECT, 2026-07-02)
---

# context-checkpointing

**Inherited from:** `cline` — selected as the best verified implementation of this
dimension in the Stage 2 capability matrix.

## What Council does with it (advisory-only)

- Long task → recommend checkpointed execution (shadow-git style) so any step is reversible.
- Propose a plan-mode pass (read-only tools) before any mutating pass.

## Evidence (files actually read)

opensrc-verified: ContextManager.ts + disk.ts (persisted task history), CheckpointTracker.ts (shadow-git checkpoints), ToolExecutor.ts PLAN_MODE_RESTRICTED_TOOLS (strict Plan/Act gate).

> Council is DORMANT (PLAN_ONLY floor). This skill informs recommendations; it never
> authorizes execution. See ../../CONSTITUTION.md.
