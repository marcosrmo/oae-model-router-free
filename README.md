# oae-model-router-free
Free multi-provider AI model routing, intelligent fallback and multi-agent orchestration for OpenCode and OAE Core.
# Model Router

**Intelligent Multi-Provider Model Routing and Fallback System**

Model Router is an independent engineering project designed to manage AI model selection, provider routing, automatic fallback, and multi-agent execution across development environments.

Its initial integration targets OpenCode, with OpenCode Free as the primary provider and NVIDIA as the fallback provider.

The architecture is designed to support future integration with OAE Core without creating a mandatory dependency between the projects.

## Vision

Build a reusable, provider-independent model routing system that prioritizes:

- Output quality and engineering reliability.
- Intelligent model selection.
- Provider availability and quota management.
- Automatic fallback and execution continuity.
- Multi-agent coordination.
- Traceability and operational transparency.
- Reusability across multiple software projects.

## Initial Architecture

### Primary Provider
**OpenCode Free**

The initial execution environment and primary source of free model access.

### Fallback Provider
**NVIDIA**

Secondary provider activated when the primary provider reaches applicable usage limits, becomes unavailable, or encounters recoverable failures.

### Initial Multi-Agent Team

| Agent | Responsibility |
|---|---|
| Architect | Architecture, planning and technical decisions |
| Developer | Code implementation |
| Auditor | Independent code review and risk identification |
| Validator | Test execution and result validation |

Initial model assignments will be validated through provider integration tests before being considered stable.

## Core Responsibilities

1. Model and provider registry.
2. Provider-specific adapters.
3. Routing policies.
4. Quota and availability handling.
5. Automatic fallback.
6. Execution continuity and context preservation.
7. Multi-agent model assignment.
8. Operational logs and traceability.
9. Manual provider selection and override.
10. Reusable OpenCode integration.

## Manual Commands

The initial operational interface will support:

- `USAR MODO GRATUITO`
- `USAR MODO NVIDIA`
- `VOLTAR AO MODO OPENCODE`

Provider switching must preserve the current task context whenever technically possible.

## Architectural Principles

- Provider independence.
- No mandatory dependency on OpenAI or Anthropic.
- No coupling to individual application repositories.
- Explicit routing policies.
- Safe fallback behavior.
- Independent validation.
- Minimal changes to existing environments.
- Compatibility with future OAE Core integration.

## Planned Integrations

- OpenCode
- NVIDIA API
- OAE Core (future integration)
- Additional providers and execution environments (future expansion)

## Development Roadmap

### Phase 0 — Foundation and Architecture
- Define project scope.
- Establish architectural principles.
- Document routing responsibilities.
- Define integration boundaries.

### Phase 1 — Provider Infrastructure
- Implement provider registry.
- Define provider adapter contracts.
- Validate OpenCode and NVIDIA connectivity.
- Establish model identification and configuration.

### Phase 2 — Routing and Fallback
- Implement routing policies.
- Handle quota exhaustion and recoverable errors.
- Implement provider switching.
- Validate execution continuity.

### Phase 3 — Multi-Agent Architecture
- Implement agent definitions.
- Configure model assignments.
- Establish independent auditing and validation.
- Control parallel execution.

### Phase 4 — OpenCode Integration
- Implement global reusable integration.
- Develop operational skills.
- Validate project-independent availability.

### Phase 5 — OAE Integration
- Define integration contract.
- Evaluate compatibility with OAE Core.
- Preserve OAE autonomy and provider independence.

## Non-Goals

The initial project will not:

- Modify OAE Core directly.
- Modify application repositories.
- Replace OpenCode.
- Replace existing MCP infrastructure.
- Require a specific model provider.
- Perform unauthorized deployments or repository modifications.

## Development Status

**Status:** Architecture and foundation planning.

No production implementation has been authorized yet.

## Project Governance

All architectural changes, provider integrations, and execution policies must be documented and validated before becoming part of the stable implementation.

---

**Model Router — Reliable AI Model Routing Across Development Environments.**
