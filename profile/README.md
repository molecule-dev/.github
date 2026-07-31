<div align="center">

# Molecule.dev

**An AI-first, composable package ecosystem for building full-stack apps that scale.**

[molecule.dev](https://molecule.dev) · [Packages](https://github.com/molecule-dev/molecule)

</div>

---

## Code is cheap. Scaling is not.

Code generation is now the easy part. The last 10%, the part that separates a toy prototype from a business that grows on hard data, is where Molecule lives.

Every app needs the same integrations: payments, uploads, notifications, auth, search, and more. Most AI tools regenerate them from scratch every time. Molecule already has them, battle-tested and composable, so your tokens go toward what really matters.

## What it is

- **A composable package ecosystem.** A growing catalog of `@molecule/*` packages that connect through abstract interfaces and machine-readable docs, covering the parts every real app needs.
- **An AI harness.** Synthase, the harness inside [molecule.dev](https://molecule.dev), assembles, runs, and deploys full-stack apps from those packages, on a new project or your existing repo.
- **Real, decoupled architecture.** Not throwaway prototypes. Code seasoned teams can own, audit, and scale, composed from tested, maintained packages instead of one-off generated code.

## The bond pattern

Your code targets an interface, not a provider. Swap the implementation without rewriting your app.

```typescript
import { bond } from '@molecule/api-bond'
import { provider } from '@molecule/api-database-postgresql'
import { findMany } from '@molecule/api-database'

bond('database', provider)

// Same call, whichever provider you wire in.
const users = await findMany('users')
```

Switch to SQLite, MySQL, or anything else by changing the import. [Read more.](https://github.com/molecule-dev/molecule#the-bond-system)

## Everything a real app needs

Auth and OAuth, two-factor, payments, databases, caching, AI and agents, email, search, realtime, background jobs, scheduling, uploads, analytics, logging and monitoring, notifications, localization, accessibility, testing, CI/CD, and more. Each one a complete, tested package, built from the ground up for AI to understand and wire together.

## Built like the best teams

Typed, tested, CI/CD, migrations, monitoring, logging, analytics, rate limiting, security, no lock-in. The discipline serious teams expect, plus the instrumentation to scale on hard data, not hunches.

## Open source, no lock-in

Everything is open source under Apache-2.0. You own the real, readable code, swap any provider, export it, and self-host anything. Deploy with us and pay only for the metered AI and infrastructure you use, or run it entirely yourself.

## The stack

TypeScript and Node on the backend, your choice of frontend (React, Vue, Svelte, and more), plus React Native for mobile. The architecture isn't tied to any one stack, so the list keeps growing, and we can add a new language or framework fast at any request.

## Explore

The full ecosystem lives in **[molecule](https://github.com/molecule-dev/molecule)**: the composable `@molecule/*` packages, each with machine-readable docs.

## Get started

Describe what you need at **[molecule.dev](https://molecule.dev)**, and Synthase takes it from there. Or browse the packages and wire them in yourself with the bond pattern.

<div align="center">

---

Apache-2.0 · Built to scale.

</div>
