# DeployPilot Brief

## One-line Summary

Inspect and generate deployment packages: Dockerfile, Docker Compose, GitHub Actions, environment checklist, health check, deployment README, and rollback guide.

## Category

DevOps Assistant

## Priority

Phase 3 support product

## Product Context

This project belongs to the public Cerebra Forge Labs / ForgeOps Labs product idea set. The public repository should present DeployPilot as an independent product that people can understand and use, while the deeper Cerebra MCP layer can be used internally for orchestration, review, testing, security, DevOps, and context governance.

## Product Concept

A tool for developers who can build apps but are less confident deploying them. It reviews a project and creates or checks the deployment package needed for safe operation.

## Why It Should Exist

It is a strong CerebraDevops demo, especially when paired with RepoDoctor or AgentForge.

The market need is practical: teams want AI-assisted systems that move beyond prompts and demos into repeatable workflows, validated outputs, and handoff-ready artifacts. DeployPilot should make that workflow explicit and useful from the first release.

## Target Users

application developers, solo builders, small teams, DevOps-light startups

## Primary Job To Be Done

When a user needs devops assistant work, they should be able to provide the minimum required context, run the workflow, inspect the result, and leave with a usable output package rather than vague advice.

## Inputs

repository path or URL, app type, runtime, deployment target, env vars, health endpoint

## Outputs

Dockerfile, docker-compose.yml, GitHub Actions workflow, env checklist, health check, rollback guide

## Core Capabilities

- repo/runtime detection
- Dockerfile generator
- compose generator
- CI workflow generator
- environment checklist
- health-check policy
- deployment README
- rollback guide

## Cerebra MCP Fit

Recommended Cerebra MCP capabilities:

CerebraDevops-mcp, CerebraSecurity-mcp, CerebraTesting-mcp, CerebraReview-mcp

Cerebra should be used as the behind-the-scenes quality layer for role selection, context composition, risk checks, review, testing, security, and delivery evidence. The public product should not require users to understand Cerebra internals before they can get value.

## MVP Experience

1. User creates a project or run.
2. User provides required inputs.
3. System validates missing or risky information.
4. System generates or audits the target artifact.
5. User reviews output, warnings, assumptions, and next steps.
6. User exports or saves the result.

## Differentiation

- Product-specific workflow, not a generic chatbot.
- Concrete outputs that can be committed, deployed, tested, or reviewed.
- Quality gates that make generated work safer to trust.
- Clear traceability from inputs to output.
- Practical public repo structure that invites adoption and contribution.

## Success Metrics

- First useful result is produced in under 10 minutes for a new user.
- At least 80 percent of MVP runs produce an exportable artifact.
- Generated outputs require fewer than three major manual corrections in normal use.
- Users can understand setup and usage from the README without private context.
- The project can be demonstrated publicly with safe sample data.

## Non-goals

- Do not expose private Cerebra internals as a requirement for public use.
- Do not automate destructive or external actions without explicit approval.
- Do not build broad marketplace features before the core workflow works.
- Do not ship AI output without assumptions, risks, and validation status.

## Recommended MVP Stack

CLI plus report UI, Docker, GitHub Actions, deployment target adapters

## Key Risks

unsafe deployment defaults, missing migrations, secret leakage, wrong health checks, rollback gaps

## Launch Recommendation

Ship the first version as a focused public repo with clear docs, sample input, sample output, and a small runnable path. Treat broader integrations as phase two unless they are essential to proving the product.
