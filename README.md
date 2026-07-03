# Roger (the harness council) — Ensemble Special Operator

Council is Mission Control's ensemble **SPECIAL OPERATOR**, manufactured through the
Agent Build Framework (HARVEST → SELECT → BLUEPRINT → SCAFFOLD) and distilled from the
verified best capability of each of the 9 Mission Control operators.

- **Status:** LIVE, full parity (President-approved, Task `a583ddb7`)
- **Engine:** `claude -p`, model pinned `claude-sonnet-4-6`, subscription auth
  (`ANTHROPIC_API_KEY` unset)
- **Capabilities:** write-capable, EXECUTE floor; `deploy` + `migration` classes remain
  blocked (route through the Orchestrator's migration-first + boot-verify protocol)
- **Home:** `/root/.council` · snapshot `mission-control/operators/council/`

## CLI

```
council "Cross-check this plan and execute the safe parts"
council --advisory "Which operator should take this task?"   # read-only poll
council --file task.md
```

Every run injects the Protocol Preamble + Council's operator identity, logs a traceable
handoff on the MAIS bus (OR-16), executes on the Council engine, resolves the handoff,
and writes a run log under `runs/`.

## Install

From the private repo (npm ≥ 9, needs repo access):

```
npm install -g Andrewrico/council
```

or from a local checkout:

```
npm install -g /root/.council
```

Both place `council` on the PATH (the host also keeps `/usr/local/bin/council`).

## Layout

| Path | Purpose |
| --- | --- |
| `IDENTITY.md` / `VAC_IDENTITY.md` | operator identity (VAC_* = operator-home parity names) |
| `CONSTITUTION.md` / `VAC_CONSTITUTION.md` | operating law snapshot |
| `cli-config.json` | engine/runtime config (class, floor, tools, provenance) |
| `mcp.json` | MCP server access |
| `skills-council/` | 9 inherited skills, one per capability-matrix winner |
| `agents/` | operator-home agents dir (parity with other operator homes) |
| `bin/council` | the CLI dispatcher (npm bin + `/usr/local/bin/council`) |
| `runs/` | dispatch run logs (gitignored) |

Inherited-from map: orchestration-fanout←claude, build-safety-handoff←cursor-agent,
coding-pipeline←codex, governance-escalation←hermes, permission-gating←opencode,
context-checkpointing←cline, grounded-research←gemini, lean-dispatch←pi,
channel-acp-interop←openclaw. Selection evidence:
`mission-control/drive/documentation/system-architecture/council-capability-matrix.md`.
