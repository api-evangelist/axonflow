---
generated: '2026-10-09'
method: generated
name: axonflow-gateway-precheck-and-audit
description: 'Gateway mode: pre-check a prompt against AxonFlow policy before calling your own LLM, then record the call in
  the audit trail.'
api: openapi/axonflow-agent-openapi.yml
operations:
- gatewayPreCheck
- auditLLMCall
source: 'Grounded in openapi/ (agent, orchestrator) for AxonFlow platform 11.1.0; every operationId verified verbatim in the
  spec. Docs: https://docs.getaxonflow.com/docs/orchestration/api-reference/'
---

# Gateway precheck and audit

Gateway mode: pre-check a prompt against AxonFlow policy before calling your own LLM, then record the call in the audit trail.

## Auth
HTTP Basic `org:license-key` (scheme `BasicAuth` in the spec) against the customer's self-hosted agent (default http://localhost:8080) or orchestrator (default http://localhost:8081). A community-mode deployment needs no credentials.

## Steps
1. `gatewayPreCheck` (POST /api/policy/pre-check) with required `query` and `client_id` (optional `user_token`, `data_sources`, `context`). If the response blocks, stop and surface the reason; do not call the LLM.
2. Call your LLM provider yourself.
3. `auditLLMCall` (POST /api/audit/llm-call) with required `context_id` (from step 1), `client_id`, `provider`, `model`, `token_usage`; add `latency_ms` and `response_summary` when known.

## Errors
Pre-check may return 400, 401, 402, 403, 429 or 503. Treat 403 as a governance verdict, not an outage; back off on 429.
