# Nexus

## Purpose

Nexus is Kofi's AI-native productivity and knowledge operating system. It combines a React client, an Express API, GitHub-backed Markdown knowledge, and NVIDIA reasoning while keeping deterministic retrieval separate from AI generation.

## Operating Model

```text
User
 ↓
React / Vite client on Vercel
 ↓
Express API on Heroku
 ↓
GitHub repositories
 ↓
Nexus Vault
 ↓
NVIDIA reasoning when required
```

## Source Of Truth

This repository is the canonical knowledge store. Markdown files are durable truth. Git history supplies revision history. The Nexus application reads the Vault through GitHub and must not silently replace deterministic retrieval with AI.

## Retrieval Order

1. `NEXUS.md`
2. `identity/INDEX.md` and relevant identity documents
3. `registry/`
4. the selected project `INDEX.md`
5. the selected project `AGENT.md`
6. relevant Markdown documents only
7. NVIDIA reasoning only when synthesis or generation is genuinely required

Never load the entire Vault by default.

## Core Principles

- GitHub is persistence for the MVP.
- Markdown remains portable outside the application.
- Retrieval is deterministic before it is intelligent.
- AI reasons over selected context; it does not invent missing facts.
- Decisions, assumptions, ideas, tasks, implementation, and verification remain distinct.
- Secrets and credentials never belong in the Vault.
- Project records are useful without Nexus running.

## Current State

The application repository is `kofiarhin/nexus`. Its Foundation MVP is currently represented by draft pull request #1 on branch `agent/foundation-mvp`.

This Vault foundation is being established in `kofiarhin/nexus-vault`.
