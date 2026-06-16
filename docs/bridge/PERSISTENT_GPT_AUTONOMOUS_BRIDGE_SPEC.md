# Persistent GPT Autonomous Bridge Spec

## Status

Draft architecture specification only. This file is a planning document. It does not modify workflows, deployments, billing, schemas, secrets, Drive canon, Sheets canon, Shopify settings, Vercel env, Supabase schema, governance, authority files, or production systems.

## Purpose

Define a governed bridge that lets Eden Skye and Auto Builder preserve continuity across GPT sessions using external runtime and storage.

The bridge is not an always-awake GPT. It is a controlled runtime layer that stores state, accepts tasks, records evidence, tracks approvals, registers assets, and produces recovery prompts for future GPT sessions.

## Core Architecture

```text
ChatGPT / Eden Skye / Auto Builder
  -> Vercel Bridge API
  -> Supabase persistence proposal
  -> GitHub branch and PR workflow
  -> Runway asset tracking ledger
  -> human approval gates
  -> audit log and recovery prompts
```

## Default Mode

Read-only inspection, validation, planning, prompt drafting, continuity logging, evidence logging, asset registration, and approval request creation.

## Approval Rule

No workflow, governance, source truth, billing, deployment, schema, Drive, Sheets, Shopify, Vercel env, Supabase, authority-file, or production mutation may occur without Jeremy explicitly authorizing that exact mutation in the current session.

## Approval Gate Levels

| Level | Scope | Examples | Human Approval |
| --- | --- | --- | --- |
| L0 | Read-only | inspect repo, list assets, review logs | Not required |
| L1 | Draft-only | draft prompts, specs, plans | Not required |
| L2 | Non-production docs branch | add docs, open draft PR | Exact scope required |
| L3 | Runtime code | API routes, job routing | Exact scope required |
| L4 | Sensitive systems | env vars, secrets, billing, schemas | Exact scope plus review required |
| L5 | Authority/source truth | governance, canon, approval matrix | Exact file and operation required |

## Continuity Memory

The bridge should preserve:

- current objective
- active phase and step
- verified facts
- inferred items
- could-not-verify items
- open tasks
- active blockers
- workaround path
- approvals granted in the current session
- next GPT instruction

## Task Queue

Each task should include:

- task id
- title
- description
- owner
- status
- priority
- required approval level
- source evidence
- expected output
- blocker notes
- next action

Suggested task statuses:

```text
new
triage
blocked
awaiting_human
approved
in_progress
needs_review
complete
rejected
cancelled
```

## Evidence Logging

Every operational update should separate:

```text
Verified:
Inferred:
Could Not Verify:
```

Evidence entries should point to repo files, PRs, commits, connector responses, asset URLs, screenshots, or manually provided context.

## Runway Asset Tracking

Runway assets should be logged as references, not as assumed canon. Track:

- asset id
- media type
- source image
- prompt
- negative prompt
- preview URL
- generation URL if available
- Eden identity anchor
- QC status
- rejection reason
- canon label

Allowed canon labels:

```text
EDEN_SKYE_CHARACTER_CANON
EDEN_SKYE_ALT_STYLE_REFERENCE
Rejected_Tests
EPOXY_ASMR_APPROVED
EPOXY_ASMR_REJECTED
```

## Eden Character Protection Rules

Protect Eden as a fictional AI avatar with:

- age 35 appearance
- warm tan skin
- long glossy dark brunette hair
- expressive brown eyes
- elegant lips
- natural soft glam makeup
- premium soft-luxury styling
- no celebrity likeness
- no real-person impersonation
- no teen-coded or childlike styling

## Epoxy ASMR Rule

```text
First frame = motion.
First sound = texture.
First second = satisfaction.
```

Reject video outputs if face changes, Eden appears younger, hands distort, resin looks cheap, camera moves too fast, voice talks too much, or the first second lacks scroll-stop value.

## Vercel API Proposal

Documentation-only route proposal:

```text
GET  /api/bridge/health
GET  /api/bridge/context/latest
POST /api/bridge/task/create
POST /api/bridge/task/update
POST /api/bridge/event/log
POST /api/bridge/approval/request
POST /api/bridge/approval/resolve
POST /api/bridge/assets/register
GET  /api/bridge/assets/recent
POST /api/bridge/recovery/create
GET  /api/bridge/recovery/latest
```

Runtime routes should not mutate production systems without a current approval token, exact mutation scope, actor identity, and audit-log entry.

## Supabase Data Model Proposal

Documentation-only table proposal:

```text
bridge_sessions
bridge_tasks
bridge_events
bridge_approvals
bridge_assets
bridge_connectors
bridge_evidence
bridge_prompts
bridge_logs
```

No schema migration is included in this PR.

## Audit Logging

Each bridge action should record:

- timestamp
- actor
- action
- target system
- target resource
- approval id if applicable
- result
- error if any
- rollback path

Logs should be append-only where possible.

## Recovery Prompt Template

```text
Rehydrate Eden Skye Persistent GPT Autonomous Bridge.

Current objective:
[objective]

Active phase / step:
[phase] / [step]

Verified:
[verified facts]

Inferred:
[inferred items]

Could Not Verify:
[unknowns]

Open tasks:
[tasks]

Approvals granted this session:
[approvals]

Blocks:
[blocks]

Workaround:
[workaround]

Next action:
[next action]

Do not mutate workflow, governance, source truth, billing, deployments, database schema, Drive canon, Sheets canon, Shopify, Vercel env, Supabase schema, or authority files unless Jeremy explicitly authorizes that exact mutation in the current session.
```

## Implementation Phases

### Phase 1: Documentation

- approve bridge architecture
- approve approval gate levels
- approve recovery prompt format

### Phase 2: Read-Only Runtime

- add health endpoint
- add context read endpoint
- add event logging endpoint

### Phase 3: Task and Approval Layer

- add task queue endpoints
- add approval request and resolve endpoints
- add audit logging

### Phase 4: Asset Registry

- add Runway asset registry
- add Eden canon labels
- add QC status tracking

### Phase 5: Controlled Execution

- connect approved runtime actions
- enforce approval gates
- test with non-production tasks only

## Rollback

Close this PR or revert the docs commit. No runtime or production rollback is needed because this PR is documentation-only.
