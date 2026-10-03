<div align="center">
  <a href="https://www.molecule.dev"><picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/molecule-dev/molecule/main/docs/assets/how-molecule-works-dark.svg">
    <img src="https://raw.githubusercontent.com/molecule-dev/molecule/main/docs/assets/how-molecule-works-light.svg" alt="How Molecule works: describe an app, Synthase composes it from open-source @molecule packages, bonds make every provider swappable, and the result is plain TypeScript you own." width="100%">
  </picture></a>

# Molecule.dev

**Describe an app. Get real, tested, full-stack TypeScript you own.**

[molecule.dev](https://www.molecule.dev) · [Packages](https://github.com/molecule-dev/molecule) · [How it works](https://how-molecule-works.apps.mlcl.dev) · [Status](https://status.molecule.dev)

</div>

---

## What it is

- **1,000+ composable `@molecule/*` packages** on npm, Apache-2.0. Auth, payments, databases, email, AI, search, realtime, uploads, analytics, i18n and more, for Express APIs and React, Vue, Svelte, Solid, Angular and React Native apps.
- **Synthase**, the AI developer agent in [molecule.dev](https://www.molecule.dev). It picks packages, wires them, runs the app in a live sandbox, type-checks and tests it, and deploys it.
- **150+ flagship templates** to start from a working app instead of a blank prompt.
- **A CLI and an MCP server** so your own coding agent (Claude Code, Codex, Cursor and others) can search, scaffold, add and swap packages with structured tools.

## Why it's different

Your code calls an interface, never a vendor SDK. A **bond** wires the provider at startup, so swapping Postgres for MySQL, or one payments provider for another, changes one import.

```typescript
import { pool, store } from '@molecule/api-database-postgresql'
import { setPool, setStore } from '@molecule/api-database'

setPool(pool)
setStore(store)

// Swap to MySQL or SQLite by changing the import above.
// Application code keeps calling @molecule/api-database.
```

Every package has a README generated from its source, so an AI agent can wire it correctly in one pass, even on smaller models.

## Built in, not bolted on

Typed, linted and tested before it reaches you, with unit, integration and E2E tests shipped in the project. Auth, migrations, i18n, logging, error tracking, analytics and user feedback are included, and an `AGENTS.md` teaches any coding agent the project's conventions.

## No lock-in

Export the project code, a database dump and your `.env` files at any time, and run it anywhere. Deploy with us and pay for the metered AI and infrastructure you use, or self-host everything.

## Repositories

| Repo | What's in it |
| --- | --- |
| [**molecule**](https://github.com/molecule-dev/molecule) | The `@molecule/*` package library. Start here. |
| [**how-molecule-works**](https://github.com/molecule-dev/how-molecule-works) | The interactive walkthrough, built and deployed with Molecule itself. |

## Get started

Describe what you need at **[molecule.dev](https://www.molecule.dev)**, or browse the [packages](https://github.com/molecule-dev/molecule) and wire them in yourself.

<div align="center">

---

Molecule Dev, Inc. · Apache-2.0

</div>
