---
generated: '2026-10-09'
method: generated
name: axonflow-review-hitl-approval
description: 'Work the human-in-the-loop queue: list pending decisions, inspect one, approve or reject it, and read its history.'
api: openapi/axonflow-agent-openapi.yml
operations:
- listHITLDecisions
- getHITLDecision
- approveHITLDecision
- rejectHITLDecision
- getHITLDecisionHistory
source: 'Grounded in openapi/ (agent, orchestrator) for AxonFlow platform 11.1.0; every operationId verified verbatim in the
  spec. Docs: https://docs.getaxonflow.com/docs/orchestration/api-reference/'
---

# Review hitl approval

Work the human-in-the-loop queue: list pending decisions, inspect one, approve or reject it, and read its history.

## Auth
HTTP Basic `org:license-key` (scheme `BasicAuth` in the spec) against the customer's self-hosted agent (default http://localhost:8080) or orchestrator (default http://localhost:8081). A community-mode deployment needs no credentials.

## Steps
1. `listHITLDecisions` (GET /api/v1/hitl/queue) to find pending items.
2. `getHITLDecision` (GET /api/v1/hitl/queue/{id}) to read the held request.
3. `approveHITLDecision` or `rejectHITLDecision` (POST /api/v1/hitl/queue/{id}/approve|reject). A human makes this call; an agent must not approve its own request.
4. `getHITLDecisionHistory` (GET /api/v1/hitl/queue/{id}/history) for the audit record.
