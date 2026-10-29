# AxonFlow

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

AxonFlow is a runtime governance platform for AI agents. It gives every agent a mandate, limits and a paper trail: deterministic policies evaluated before an agent acts, human approvals, PII redaction, AI usage budgets, tamper-evident audit logs and decision records exportable for frameworks such as the EU AI Act, RBI, SEBI and MAS FEAT. It ships an open-source Community Edition on GitHub, an Evaluation licence and a paid production program, runs in the customer's own environment, and integrates via Python, TypeScript, Go, Java and Rust SDKs and plugins for LangChain, LangGraph, CrewAI, LiteLLM, n8n, Claude Code, Cursor and others, plus an optional Fraud & Risk Add-on for payment agents.

**Areas:** Company · AI Governance · AI Agents · Policy Enforcement · Audit Logging · Compliance · MCP · Open Source

## AxonFlow on APIs.io

Everything profiled for AxonFlow is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/axonflow/](https://apis.io/providers/axonflow/)** — or go straight to one of the APIs or properties below.

### APIs (54)

- [AxonFlow Agents API](https://apis.io/apis/axonflow/axonflow-agents-api/) — Agent configuration management (MAP 0.8). **Enterprise only** — the `/api/v1/agents` route family is registered only in Enterprise builds with a database…
- [AxonFlow Assessments API](https://apis.io/apis/axonflow/axonflow-assessments-api/) — FEAT Assessment lifecycle
- [AxonFlow Audit API](https://apis.io/apis/axonflow/axonflow-audit-api/) — Audit log search and retrieval
- [AxonFlow Audit Verification API](https://apis.io/apis/axonflow/axonflow-audit-verification-api/) — Non-repudiation verification of the signed decision chain (#2722). Read-only endpoints that re-verify per-record Ed25519 signatures and the prev_hash…
- [AxonFlow Bulk Operations API](https://apis.io/apis/axonflow/axonflow-bulk-operations-api/) — Import and export policies
- [AxonFlow Circuit Breaker API](https://apis.io/apis/axonflow/axonflow-circuit-breaker-api/) — Emergency circuit breaker for AI operations (EU AI Act Article 14). Instantly halt AI operations with two-person deactivation requirement.
- [AxonFlow Community SaaS API](https://apis.io/apis/axonflow/axonflow-community-saas-api/) — Self-registration on the hosted Community SaaS deployment (`DEPLOYMENT_MODE=community-saas` only).
- [AxonFlow Compliance API](https://apis.io/apis/axonflow/axonflow-compliance-api/) — The Compliance API from AxonFlow — 3 operation(s) for compliance.
- [AxonFlow Connectors API](https://apis.io/apis/axonflow/axonflow-connectors-api/) — Connector marketplace
- [AxonFlow Cost Controls API](https://apis.io/apis/axonflow/axonflow-cost-controls-api/) — Budget management and LLM usage tracking for cost optimization. Supports budgets at organization, team, agent, workflow, and user scopes. Provides usage…
- [AxonFlow Cost Management API](https://apis.io/apis/axonflow/axonflow-cost-management-api/) — The Cost Management API from AxonFlow — 2 operation(s) for cost management.
- [AxonFlow Decision & Execution Replay API](https://apis.io/apis/axonflow/axonflow-decision-execution-replay-api/) — Decision & Execution Replay API for debugging, auditing, and compliance. Captures every step of workflow execution with full input/output snapshots and…
- [AxonFlow Decision Mode API](https://apis.io/apis/axonflow/axonflow-decision-mode-api/) — Synchronous policy decision endpoint (ADR-056). Called by an infrastructure gateway acting as a Policy Enforcement Point (PEP); AxonFlow returns a verdict…
- [AxonFlow Decisions & Overrides API](https://apis.io/apis/axonflow/axonflow-decisions-overrides-api/) — Decision explainability (ADR-043) and session-scoped policy overrides (ADR-044). List recent governance decisions, explain a specific decision, and…
- [AxonFlow Dynamic Policies API](https://apis.io/apis/axonflow/axonflow-dynamic-policies-api/) — Legacy policy management on `/api/v1/policies`. Reads, tests and simulation are served; writes answer `409 LEGACY_POLICY_WRITE_FROZEN` in v11 (see the…
- [AxonFlow EU AI Act API](https://apis.io/apis/axonflow/axonflow-eu-ai-act-api/) — EU AI Act compliance endpoints for technical documentation export, conformity assessments (Article 43), and accuracy/bias tracking (Article 15). Enterprise…
- [AxonFlow EU AI Act (Proxied) API](https://apis.io/apis/axonflow/axonflow-eu-ai-act-proxied-api/) — EU AI Act compliance module (conformity assessments, accuracy monitoring, evidence exports). Served by the orchestrator and PROXIED through the agent…
- [AxonFlow Evidence Export API](https://apis.io/apis/axonflow/axonflow-evidence-export-api/) — The Evidence Export API from AxonFlow — 2 operation(s) for evidence export.
- [AxonFlow Gateway Mode API](https://apis.io/apis/axonflow/axonflow-gateway-mode-api/) — Pre-check and audit for SDK-managed LLM calls
- [AxonFlow Health API](https://apis.io/apis/axonflow/axonflow-health-api/) — Service health and readiness checks
- [AxonFlow HITL API](https://apis.io/apis/axonflow/axonflow-hitl-api/) — Human-in-the-Loop decision queue (EU AI Act Article 14). Route high-risk AI decisions for human review before execution.
- [AxonFlow Kill Switch API](https://apis.io/apis/axonflow/axonflow-kill-switch-api/) — Emergency system disable mechanism
- [AxonFlow LLM Providers API](https://apis.io/apis/axonflow/axonflow-llm-providers-api/) — LLM provider management
- [AxonFlow MAP API](https://apis.io/apis/axonflow/axonflow-map-api/) — The MAP API from AxonFlow — 1 operation(s) for map.
- [AxonFlow MCP Connectors API](https://apis.io/apis/axonflow/axonflow-mcp-connectors-api/) — Model Context Protocol data connector operations
- [AxonFlow MCP Server API](https://apis.io/apis/axonflow/axonflow-mcp-server-api/) — Streamable-HTTP MCP server (spec 2025-06-18) exposing AxonFlow governance as MCP tools (check_policy, check_output, audit_tool_call, list_policies,…
- [AxonFlow Media Governance API](https://apis.io/apis/axonflow/axonflow-media-governance-api/) — Multimodal image governance for LLM requests. Analyzes images for PII (via OCR), content safety, face/biometric detection, and document classification.…
- [AxonFlow Metrics API](https://apis.io/apis/axonflow/axonflow-metrics-api/) — Performance monitoring and observability
- [AxonFlow Multi-Agent Planning API](https://apis.io/apis/axonflow/axonflow-multi-agent-planning-api/) — LLM-powered task decomposition and execution
- [AxonFlow OJK Compliance API](https://apis.io/apis/axonflow/axonflow-ojk-compliance-api/) — OJK AI Governance + UU PDP compliance for Indonesian financial services. Audit export, retention/readiness checks, UU PDP Art. 46 breach-notification…
- [AxonFlow OpenAI Compatible API](https://apis.io/apis/axonflow/axonflow-openai-compatible-api/) — OpenAI-compatible gateway endpoint (Issue #2351). Accepts standard OpenAI Chat Completions requests, runs AxonFlow policy checks, forwards to the upstream…
- [AxonFlow OTLP Ingest API](https://apis.io/apis/axonflow/axonflow-otlp-ingest-api/) — OpenTelemetry OTLP/HTTP ingest for Claude Code (cowork) telemetry (#2832). **Enterprise only** — community builds mount the routes but return 501.…
- [AxonFlow Policies API](https://apis.io/apis/axonflow/axonflow-policies-api/) — Dynamic policy CRUD operations (Orchestrator)
- [AxonFlow Policy Simulation API](https://apis.io/apis/axonflow/axonflow-policy-simulation-api/) — The Policy Simulation API from AxonFlow — 3 operation(s) for policy simulation.
- [AxonFlow Processing API](https://apis.io/apis/axonflow/axonflow-processing-api/) — Main request processing pipeline
- [AxonFlow Proxy Mode API](https://apis.io/apis/axonflow/axonflow-proxy-mode-api/) — Full request interception and processing
- [AxonFlow RBI Compliance API](https://apis.io/apis/axonflow/axonflow-rbi-compliance-api/) — RBI FREE-AI Framework compliance for Indian banking institutions. Enterprise feature providing AI System Registry, Model Validation, Incident Management,…
- [AxonFlow Registry API](https://apis.io/apis/axonflow/axonflow-registry-api/) — AI System Registry management
- [AxonFlow SEBI Compliance API](https://apis.io/apis/axonflow/axonflow-sebi-compliance-api/) — SEBI AI/ML Guidelines compliance and DPDP Act 2023 audit exports. Enterprise feature for Indian financial services compliance.
- [AxonFlow Simulation API](https://apis.io/apis/axonflow/axonflow-simulation-api/) — Policy simulation, impact reports, and conflict detection. **Evaluation tier and above.**
- [AxonFlow Static Policies API](https://apis.io/apis/axonflow/axonflow-static-policies-api/) — DEPRECATED spelling of System Policies, served at `/api/v1/static-policies`. Every operation is the same handler as its `/api/v1/system-policies`…
- [AxonFlow System Policies API](https://apis.io/apis/axonflow/axonflow-system-policies-api/) — System policy management (ADR-019), served at `/api/v1/system-policies`. Pattern-based enforcement rules for SQL injection detection, PII detection and…
- [AxonFlow Templates API](https://apis.io/apis/axonflow/axonflow-templates-api/) — Policy templates for quick policy creation
- [AxonFlow Tenant Policies API](https://apis.io/apis/axonflow/axonflow-tenant-policies-api/) — Tenant policy CRUD via the ADR-024 `/api/v1/tenant-policies` surface (Orchestrator, proxied by the Agent). On create, update and import it accepts only…
- [AxonFlow Testing API](https://apis.io/apis/axonflow/axonflow-testing-api/) — Policy testing and validation
- [AxonFlow Typed Policy Authoring API](https://apis.io/apis/axonflow/axonflow-typed-policy-authoring-api/) — The ADR-065 typed policy authoring surface, available on EVERY edition (#3907). It is the write path a deployment without the Enterprise customer portal…
- [AxonFlow Unified Executions API](https://apis.io/apis/axonflow/axonflow-unified-executions-api/) — Unified execution tracking and real-time streaming for MAP plans and WCP workflows. SSE streaming provides real-time status updates. Community: 5 concurrent…
- [AxonFlow US Banking Compliance API](https://apis.io/apis/axonflow/axonflow-us-banking-compliance-api/) — US federal banking and Farm Credit examination evidence (ADR-063). One read: the examination-readiness summary. The evidence itself is produced by the…
- [AxonFlow US Insurance Compliance API](https://apis.io/apis/axonflow/axonflow-us-insurance-compliance-api/) — NAIC AI Systems Evaluation Tool exhibit evidence for US insurers, with the NYDFS Circular Letter No. 7 and Colorado Regulation 10-1-1 annexes. Read-only:…
- [AxonFlow US Securities Compliance API](https://apis.io/apis/axonflow/axonflow-us-securities-compliance-api/) — SEC adviser and FINRA broker-dealer examination evidence (ADR-064). One read: the examination-readiness summary. The evidence itself is produced by the…
- [AxonFlow Webhooks API](https://apis.io/apis/axonflow/axonflow-webhooks-api/) — Webhook subscription management for real-time event notifications. Subscribe to events like policy violations, workflow completions, budget alerts, etc.
- [AxonFlow Workflow Control Plane API](https://apis.io/apis/axonflow/axonflow-workflow-control-plane-api/) — Governance gates for external orchestrators (LangChain, LangGraph, CrewAI). "LangChain runs the workflow. AxonFlow decides when it's allowed to move…
- [AxonFlow Workflows API](https://apis.io/apis/axonflow/axonflow-workflows-api/) — Workflow execution engine
- [AxonFlow Auth ZEN API](https://apis.io/apis/axonflow/axonflow-auth-zen-api/) — The Auth ZEN API from AxonFlow — 1 operation(s) for auth zen.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [AxonFlow MCP Server](https://apis.io/servers/axonflow/axonflow-mcp-server/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Axonflow Agentic Access](https://apis.io/agentic-access/axonflow/axonflow-agentic-access/)

#### JSON Schema (24)

The data models the API reads and writes.

- [AISystemRegistry](https://apis.io/schemas/axonflow/axonflow-aisystem-registry/)
- [ApplyTemplateRequest](https://apis.io/schemas/axonflow/axonflow-apply-template-request/)
- [ApprovalResponse](https://apis.io/schemas/axonflow/axonflow-approval-response/)
- [AuditActionReport](https://apis.io/schemas/axonflow/axonflow-audit-action-report/)
- [AuditLogEntry](https://apis.io/schemas/axonflow/axonflow-audit-log-entry/)
- [ClientResponse](https://apis.io/schemas/axonflow/axonflow-client-response/)
- [CreatePolicyRequest](https://apis.io/schemas/axonflow/axonflow-create-policy-request/)
- [CreateRegistryRequest](https://apis.io/schemas/axonflow/axonflow-create-registry-request/)
- [DecideRequest](https://apis.io/schemas/axonflow/axonflow-decide-request/)
- [DecideResponse](https://apis.io/schemas/axonflow/axonflow-decide-response/)
- [FEATAssessment](https://apis.io/schemas/axonflow/axonflow-featassessment/)
- [ImpactReportResponse](https://apis.io/schemas/axonflow/axonflow-impact-report-response/)
- [KillSwitch](https://apis.io/schemas/axonflow/axonflow-kill-switch/)
- [MCPCheckInputResponse](https://apis.io/schemas/axonflow/axonflow-mcpcheck-input-response/)
- [MCPCheckOutputResponse](https://apis.io/schemas/axonflow/axonflow-mcpcheck-output-response/)
- [OJKAuditExportResponse](https://apis.io/schemas/axonflow/axonflow-ojkaudit-export-response/)
- [PolicyEvaluationResult](https://apis.io/schemas/axonflow/axonflow-policy-evaluation-result/)
- [PreCheckResponse](https://apis.io/schemas/axonflow/axonflow-pre-check-response/)
- [SimulatePoliciesResponse](https://apis.io/schemas/axonflow/axonflow-simulate-policies-response/)
- [StepGateResponse](https://apis.io/schemas/axonflow/axonflow-step-gate-response/)
- [TestPolicyResponse](https://apis.io/schemas/axonflow/axonflow-test-policy-response/)
- [UpdateAssessmentRequest](https://apis.io/schemas/axonflow/axonflow-update-assessment-request/)
- [UpdatePolicyRequest](https://apis.io/schemas/axonflow/axonflow-update-policy-request/)
- [UpdateRegistryRequest](https://apis.io/schemas/axonflow/axonflow-update-registry-request/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Axonflow Context](https://apis.io/jsonld/axonflow/axonflow-context/)

#### Overlays (4)

OpenAPI overlays, including conversational phrasing for each operation.

- [Axonflow Agent Overlay](https://apis.io/overlays/axonflow/axonflow-agent-overlay/)
- [Axonflow Masfeat Overlay](https://apis.io/overlays/axonflow/axonflow-masfeat-overlay/)
- [Axonflow Orchestrator Overlay](https://apis.io/overlays/axonflow/axonflow-orchestrator-overlay/)
- [Axonflow Policy Overlay](https://apis.io/overlays/axonflow/axonflow-policy-overlay/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [AxonFlow — axonflow rules](https://apis.io/rules/axonflow/axonflow-axonflow-spectral-rules/)
- [AxonFlow API Rules](https://apis.io/rules/axonflow/axonflow-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Axonflow Authentication](https://apis.io/security/axonflow/axonflow-authentication/)
- [Axonflow Domain Security](https://apis.io/security/axonflow/axonflow-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Axonflow Plans Pricing](https://apis.io/plans/axonflow/axonflow-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Axonflow Rate Limits](https://apis.io/rate-limits/axonflow/axonflow-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://docs.getaxonflow.com)
- [Getting started](https://docs.getaxonflow.com/docs/getting-started/)
- [API reference](https://docs.getaxonflow.com/docs/orchestration/api-reference/)
- [Pricing](https://getaxonflow.com/pricing/)
- [Changelog](https://docs.getaxonflow.com/docs/releases/)
- [Blog](https://getaxonflow.com/blog/)
- [Trust centre](https://getaxonflow.com/trust/)
- [Terms of service](https://getaxonflow.com/terms-of-service/)
- [Privacy policy](https://getaxonflow.com/privacy/)
- [GitHub](https://github.com/getaxonflow)

## API Evangelist rating

**Kin Score 71.3** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 63.4 |
| Contract governance | 35.6 |
| Operational transparency | 71.1 |
| Developer ergonomics | 68.5 |
| Access clarity | 84.2 |

**Agent readiness 42.8** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 29.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/axonflow/](https://apis.io/providers/axonflow/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for AxonFlow: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/axonflow/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
