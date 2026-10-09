---
generated: '2026-10-09'
method: generated
name: axonflow-governed-workflow-step-gates
description: 'Run an external multi-step agent workflow under AxonFlow step gates: create the workflow, gate each step, mark
  it complete, close the workflow.'
api: openapi/axonflow-orchestrator-openapi.yml
operations:
- createControlPlaneWorkflow
- checkStepGate
- markStepCompleted
- completeControlPlaneWorkflow
- failControlPlaneWorkflow
source: 'Grounded in openapi/ (agent, orchestrator) for AxonFlow platform 11.1.0; every operationId verified verbatim in the
  spec. Docs: https://docs.getaxonflow.com/docs/orchestration/api-reference/'
---

# Governed workflow step gates

Run an external multi-step agent workflow under AxonFlow step gates: create the workflow, gate each step, mark it complete, close the workflow.

## Auth
HTTP Basic `org:license-key` (scheme `BasicAuth` in the spec) against the customer's self-hosted agent (default http://localhost:8080) or orchestrator (default http://localhost:8081). A community-mode deployment needs no credentials.

## Steps
1. `createControlPlaneWorkflow` (POST /api/v1/workflows) with required `workflow_name`.
2. For each step: `checkStepGate` (POST /api/v1/workflows/{workflow_id}/steps/{step_id}/gate) with required `step_type`. The `decision` is `allow`, `block` or `require_approval`; only run the step on `allow`.
3. After the step: `markStepCompleted` (POST .../steps/{step_id}/complete) with `output`, token counts, `cost_usd` and an `idempotency_key` so retries are safe.
4. `completeControlPlaneWorkflow` on success, or `failControlPlaneWorkflow` on failure.

## Errors
Gate: 400, 404, 409, 413. Completion: 400, 404, 409.
