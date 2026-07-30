# Preferences

## Architecture

- Prefer simple, explicit system boundaries over hidden framework behavior.
- Use React with Vite for the Nexus client.
- Use Node.js and Express with an MVC-oriented backend structure.
- Keep GitHub repositories as the MVP persistence layer.
- Use NVIDIA as the sole AI provider for Nexus reasoning.
- Keep deterministic retrieval independent from AI.
- Avoid loading the full knowledge base when selected context is sufficient.

## Delivery

- Define scope, out-of-scope boundaries, acceptance criteria, and verification before implementation.
- Work in isolated branches and review through pull requests.
- Treat implementation, verification, merge, deployment, and completion as separate states.
- Prefer a focused first milestone over pretending to implement an entire product at once.

## Knowledge

- Markdown should remain readable and useful without the application.
- Preserve decisions and assumptions separately.
- Prefer concise indexes that route to detailed documents.
- Do not fabricate missing identity or project facts.

## Current MVP Constraints

- No authentication.
- No vector database.
- No AI for project listing or document retrieval.
- No Vault writes from the public API during the Foundation MVP.
