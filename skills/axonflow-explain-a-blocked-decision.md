---
generated: '2026-10-09'
method: generated
name: axonflow-explain-a-blocked-decision
description: Find a governance decision, explain why it was made, and pull the matching audit records.
api: openapi/axonflow-orchestrator-openapi.yml
operations:
- listDecisions
- explainDecision
- searchAuditLogs
source: 'Grounded in openapi/ (agent, orchestrator) for AxonFlow platform 11.1.0; every operationId verified verbatim in the
  spec. Docs: https://docs.getaxonflow.com/docs/orchestration/api-reference/'
---

# Explain a blocked decision

Find a governance decision, explain why it was made, and pull the matching audit records.

## Auth
HTTP Basic `org:license-key` (scheme `BasicAuth` in the spec) against the customer's self-hosted agent (default http://localhost:8080) or orchestrator (default http://localhost:8081). A community-mode deployment needs no credentials.

## Steps
1. `listDecisions` (GET /api/v1/decisions), or take the decision ID from a block reason.
2. `explainDecision` (GET /api/v1/decisions/{id}/explain) for the full DecisionExplanation (same as the `explain_decision` MCP tool).
3. `searchAuditLogs` (POST /api/v1/audit/search) filtered by `session_id`, `user_email`, `client_id` and a time window; page with `limit`/`offset`.

## Errors
400, 401, 403, 404, 429, 500. On Enterprise, results are role-scoped by the caller's per-user token.
