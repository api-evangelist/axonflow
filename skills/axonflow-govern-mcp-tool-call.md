---
generated: '2026-10-09'
method: generated
name: axonflow-govern-mcp-tool-call
description: Check an MCP/connector tool call against policy before it runs and scan its output for PII/secrets after.
api: openapi/axonflow-agent-openapi.yml
operations:
- mcpCheckInput
- mcpCheckOutput
source: 'Grounded in openapi/ (agent, orchestrator) for AxonFlow platform 11.1.0; every operationId verified verbatim in the
  spec. Docs: https://docs.getaxonflow.com/docs/orchestration/api-reference/'
---

# Govern mcp tool call

Check an MCP/connector tool call against policy before it runs and scan its output for PII/secrets after.

## Auth
HTTP Basic `org:license-key` (scheme `BasicAuth` in the spec) against the customer's self-hosted agent (default http://localhost:8080) or orchestrator (default http://localhost:8081). A community-mode deployment needs no credentials.

## Steps
1. `mcpCheckInput` (POST /api/v1/mcp/check-input) with required `connector_type` (e.g. `claude_code.Bash`) and `statement`; optional `tool`, `user_token`, `approval_id`. Do not run the tool unless it is allowed.
2. Run the tool.
3. `mcpCheckOutput` (POST /api/v1/mcp/check-output) with required `connector_type` and the `response_data` or `message`; use the redacted result it returns.

The same checks are exposed as the `check_policy` / `check_output` tools of the agent's built-in MCP server (see mcp/axonflow-mcp.yml).

## Errors
400, 401, 403, 415 (send `Content-Type: application/json`), 503.
