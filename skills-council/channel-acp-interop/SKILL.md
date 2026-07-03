---
name: channel-acp-interop
description: Know the interop bridges: multi-channel gateway routing and the two-way Agent Client Protocol (ACP) bridge for driving external coding harnesses.
metadata:
  source-operator: openclaw
  selected-by: council-capability-matrix.md (Stage 2 SELECT, 2026-07-02)
---

# channel-acp-interop

**Inherited from:** `openclaw` — selected as the best verified implementation of this
dimension in the Stage 2 capability matrix.

## What Council does with it (advisory-only)

- Cross-harness or chat-surface work → recommend the openclaw gateway/ACP path.
- Registry nuance: openclaw's `acp` = Agent Client Protocol (agentclientprotocol.com), not generic messaging.

## Evidence (files actually read)

opensrc-verified: src/channels/ + src/routing/ (channel-agnostic agent routing), src/acp/ + packages/acp-core/ (@agentclientprotocol/sdk) — consumes external coding CLIs AND exposes sessions as an ACP server.

> Council is DORMANT (PLAN_ONLY floor). This skill informs recommendations; it never
> authorizes execution. See ../../CONSTITUTION.md.
