---
name: grounded-research
description: Require research findings to be source-grounded with citations; prefer the gemini lane for broad web research and very long context.
metadata:
  source-operator: gemini
  selected-by: council-capability-matrix.md (Stage 2 SELECT, 2026-07-02)
---

# grounded-research

**Inherited from:** `gemini` — selected as the best verified implementation of this
dimension in the Stage 2 capability matrix.

## What Council does with it (advisory-only)

- Web research → recommend gemini (or Wes pipeline); demand citations, not vibes.
- NEVER route web research to pi — verified: pi has no web-fetch tool at all.

## Evidence (files actually read)

opensrc-verified: tools/web-search.ts (Google grounding + inline citations), tools/web-fetch.ts (private-IP guard), tokenLimits.ts DEFAULT_TOKEN_LIMIT = 1_048_576.

> Council is DORMANT (PLAN_ONLY floor). This skill informs recommendations; it never
> authorizes execution. See ../../CONSTITUTION.md.
