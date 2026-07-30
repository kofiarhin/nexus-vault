# Nexus

## Snapshot

Nexus is an AI-native productivity and knowledge operating system designed around user-owned Markdown, GitHub history, deterministic retrieval, and selective NVIDIA reasoning.

## Current State

- `kofiarhin/nexus` has been bootstrapped.
- Draft pull request #1 contains the authored Foundation MVP on `agent/foundation-mvp`.
- The application implementation has not been merged or deployed.
- Executable npm installation, tests, linting, and build remain unverified because the available npm mirror returned package-resolution errors during implementation.
- `kofiarhin/nexus-vault` is being established through this branch and pull request workflow.

## Current Focus

Create a substantive Vault that the Foundation MVP can read deterministically, then verify the application and Vault together before advancing to write operations or AI reasoning.

## Decisions

- The system uses separate application and knowledge repositories.
- Markdown in the Vault is canonical knowledge.
- The application reads the Vault through GitHub.
- Retrieval order is explicit and bounded.
- NVIDIA is the sole AI provider.
- AI is not used for exact project listing or document lookup.
- The Foundation MVP is read-only and has no authentication.
- Project records follow a consistent contract.

## Assumptions

- GitHub remains sufficient persistence for the owner-only MVP.
- A stable Markdown table is sufficient for the first project registry parser.
- Authentication can be deferred while the API remains read-only and access is appropriately controlled during deployment.

## Open Questions

- Which NVIDIA model should be the default for reasoning?
- What approval and conflict model should govern future Vault writes?
- When should authentication become mandatory?
- Should future search remain repository-native or add a derived index?

## Next Actions

1. Review and merge the Vault foundation after verification.
2. Resolve npm dependency installation for the Nexus application.
3. Execute application tests, linting, and client build.
4. Verify `GET /api/v1/projects` against the real Vault registry.
5. Define the controlled Vault write milestone.
