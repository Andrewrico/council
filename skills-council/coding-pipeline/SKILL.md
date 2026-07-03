---
name: coding-pipeline
description: Map maintenance-class coding to the codex SSAS lane and know when the codex executor is the right fallback.
metadata:
  source-operator: codex
  selected-by: council-capability-matrix.md (Stage 2 SELECT, 2026-07-02)
---

# coding-pipeline

**Inherited from:** `codex` — selected as the best verified implementation of this
dimension in the Stage 2 capability matrix.

## What Council does with it (advisory-only)

- SSAS/maintenance coding → recommend `orchestrate --executor codex` (Diego).
- Reserve the codex lane for well-scoped mechanical work; contested design goes to Marco.

## Evidence (files actually read)

operators-mcp registry (capabilities: coding, planning, review); snapshot config.toml (ruflo MCP + hooks); memory orchestrate-codex-executor.

> Council is DORMANT (PLAN_ONLY floor). This skill informs recommendations; it never
> authorizes execution. See ../../CONSTITUTION.md.
