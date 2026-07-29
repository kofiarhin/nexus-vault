# Working Style

## How Kofi Works

Kofi develops products through iterative shared understanding. He is comfortable starting from a broad vision, but expects the vision to be translated into explicit architecture, repository structure, scope boundaries, and an executable milestone before implementation.

## Collaboration Pattern

- Explore the product concept deeply enough to expose hidden assumptions.
- Convert agreed ideas into durable requirements and technical contracts.
- Challenge vague implementation requests instead of silently choosing a large interpretation.
- Use sensible defaults when the direction is clear.
- Keep the user informed during multi-step execution.
- Report blockers honestly rather than claiming success from authored but unexecuted work.

## Decision Style

Kofi favours decisions that preserve portability, inspectability, and future optionality. For Nexus, this led to GitHub and Markdown as the knowledge foundation, deterministic retrieval before AI, and a staged MVP rather than an oversized initial release.

## Engineering Style

- Prefer clear folders and responsibilities.
- Keep repository persistence behind repository abstractions.
- Minimise middleware and unnecessary infrastructure.
- Make environment requirements explicit.
- Build read paths before mutation paths.
- Use tests and readback as evidence, but do not confuse authored tests with executed verification.

## Communication

Concise, direct recommendations are preferred. Material trade-offs should be stated clearly, especially where a shortcut creates future coupling or where verification is incomplete.
