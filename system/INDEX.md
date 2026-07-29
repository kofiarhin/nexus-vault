# Nexus Vault System

## Authority

- `NEXUS.md` defines the overall operating model.
- `identity/` defines durable owner and product context.
- `registry/` provides deterministic discovery.
- `projects/<id>/` stores project truth.
- `planning/TODAY.md` stores the current selected plan.
- `templates/` defines reusable document contracts.

## Write Rules

- Read current content before replacing it.
- Use GitHub revisions and isolated branches for material changes.
- Update registries when canonical paths or lifecycle state change.
- Preserve useful history in changelogs or decisions.
- Never store secrets.
- Do not present generated content as verified fact.

## Naming

- Project IDs: lowercase kebab-case.
- Decisions: `YYYY-MM-DD-short-title.md`.
- Meetings: `YYYY-MM-DD-topic.md`.
- Daily notes: `YYYY-MM-DD.md`.
- Learnings: `YYYY-MM-DD-short-title.md`.
