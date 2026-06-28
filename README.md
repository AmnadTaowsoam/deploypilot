# DeployPilot

Inspect and generate deployment packages: Dockerfile, Docker Compose, GitHub Actions, environment checklist, health check, deployment README, and rollback guide.

## Product Position

DeployPilot is a **DevOps Assistant** in the Cerebra Forge Labs / ForgeOps Labs public product set. It is designed as a public, useful tool while Cerebra MCP remains the orchestration and governance factory behind the scenes.

## Why This Project Matters

It is a strong CerebraDevops demo, especially when paired with RepoDoctor or AgentForge.

The goal is not to publish a shallow demo. The repository should become a buildable product foundation with clear requirements, delivery gates, and enough implementation detail for a developer or AI coding agent to start from zero and ship a usable MVP.

## Target Users

application developers, solo builders, small teams, DevOps-light startups

## Core Workflow

1. Capture the user's intent and required inputs.
2. Validate the inputs against the product-specific quality bar.
3. Generate or inspect the target artifact.
4. Show findings, assumptions, risks, and next actions.
5. Export or hand off the result in a format that is useful outside the app.

## Documentation

- [Project brief](docs/brief.md)
- [Requirements](docs/requirements.md)
- [Architecture](docs/architecture.md)
- [Roadmap](docs/roadmap.md)
- [Delivery checklist](docs/delivery-checklist.md)

## Recommended First Build

Build one complete happy path first, then add integrations and automation. The MVP should prove that DeployPilot can deliver its core output reliably before broadening scope.

## License

MIT
