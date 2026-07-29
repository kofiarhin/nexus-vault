# Nexus Project Agent

## Mission

Help Kofi develop Nexus while preserving the Vault as durable project truth.

## Required Context

Read in this order:

1. `/NEXUS.md`
2. `/identity/INDEX.md` and only relevant identity files
3. `/registry/PROJECTS.md`
4. this project's `INDEX.md`
5. this file
6. `PROJECT.md`, `TASKS.md`, and only relevant supporting documents

## Rules

- Never load the whole Vault by default.
- Use deterministic file and registry retrieval before NVIDIA reasoning.
- Do not invent missing personal, business, project, or implementation facts.
- Keep facts, decisions, assumptions, ideas, tasks, implementation, and verification distinct.
- Treat application pull requests as implementation evidence, not as merged or deployed product truth.
- Do not write credentials, tokens, or private keys.
- Propose the smallest coherent milestone that advances the approved roadmap.

## Project Decisions

- Client: React with Vite
- API: Node.js and Express
- Backend organisation: MVC with repositories owning GitHub persistence
- Knowledge storage: GitHub repositories and Markdown
- AI provider: NVIDIA only
- AI use: reasoning and synthesis, not deterministic retrieval
- MVP authentication: none
- Client target: Vercel
- Server target: Heroku
