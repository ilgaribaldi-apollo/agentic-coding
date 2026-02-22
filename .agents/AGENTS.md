# Agentic Coding Registry

## File Index

### Routing
- [AGENTS.md](AGENTS.md): Knowledge base registry (this file)
- [AGENTS.md](../AGENTS.md): Repo root agent entrypoint

### Patterns — TypeScript / Frontend
- [typescript-stack.md](patterns/typescript-stack.md): TS monorepo foundations — Bun, Turborepo, naming, strict mode
- [nextjs-patterns.md](patterns/nextjs-patterns.md): Next.js 15 App Router — layouts, route groups, middleware, server/client
- [hono-api-routes.md](patterns/hono-api-routes.md): Hono API routes — two-file pattern, Zod validation, RPC, auth middleware
- [drizzle-schema.md](patterns/drizzle-schema.md): Drizzle ORM — schema declaration, relations, Neon clients, migrations
- [tanstack-query.md](patterns/tanstack-query.md): TanStack Query v5 — hooks, query keys, mutations, caching, invalidation
- [react-components.md](patterns/react-components.md): React component patterns — feature modules, state, forms, data tables
- [shadcn-ui.md](patterns/shadcn-ui.md): Shadcn/UI + Tailwind — CVA variants, theming, CSS variables, chart config
- [monorepo-packages.md](patterns/monorepo-packages.md): Monorepo packages — Turborepo config, Bun workspaces, internal packages
- [authentication.md](patterns/authentication.md): Auth (Clerk) — middleware, org-level multi-tenancy, product gating

### Patterns — Python / Backend
- [python-stack.md](patterns/python-stack.md): Python stack overview — Flask, uv, deployment, logging, CLI patterns
- [python-patterns.md](patterns/python-patterns.md): Python code patterns — psycopg2, SQLAlchemy, retry, parallel processing
- [data-science-patterns.md](patterns/data-science-patterns.md): Data science — xarray/Zarr, NumPy tensors, joblib, temporal ops

### Patterns — Cross-Platform
- [mobile-desktop.md](patterns/mobile-desktop.md): Mobile + Desktop — Expo Router, React Native, Electron IPC

### Patterns — Reference
- [documentation-links.md](patterns/documentation-links.md): Official doc URLs — 40+ technology links organized by category

### Agents
- [debugger.md](agents/debugger.md): Bug investigation, root cause analysis, fix verification
- [doctor.md](agents/doctor.md): Audit documentation against actual codebase
- [explorer.md](agents/explorer.md): Codebase search, architecture understanding
- [security-audit.md](agents/security-audit.md): OWASP Top 10 vulnerability assessment
- [react-expert.md](agents/react-expert.md): React/Next.js performance optimization (57 Vercel rules)

### Skills
- [SKILL.md](skills/hyperscan/SKILL.md): Hyperscan — deep codebase scan, compact context map
- [SKILL.md](skills/planning-with-files/SKILL.md): Planning with Files — file-based task planning with session recovery
- [SKILL.md](skills/vercel-react-best-practices/SKILL.md): Vercel React Best Practices — 57 perf rules with BAD/GOOD examples
- [SKILL.md](skills/agent-browser/SKILL.md): Agent Browser — browser automation for testing, forms, screenshots

### Templates
- [pattern.md](_templates/pattern.md): Template for new framework/convention patterns
- [library.md](_templates/library.md): Template for new library/framework quick references
- [agent.md](_templates/agent.md): Template for new sub-agent definitions

### Plans
- [active/](plans/active): In-progress implementation plans
- [archived/](plans/archived): Completed or abandoned plans

## Purpose
Master index for the agentic-coding knowledge base. All patterns, agents, skills, and templates are registered here. Read this to find the right file for any technology or task.

## Workflow
1. Identify what you need: a code pattern, a sub-agent, or a skill workflow.
2. Find the relevant file in the File Index above.
3. Load that file as context for your task.
4. To add content: copy a template from `_templates/`, fill it in, add an entry here.

## Quick Lookup by Technology

| Technology | Primary File | Also In |
|-----------|-------------|---------|
| Next.js | nextjs-patterns.md | typescript-stack.md |
| Hono | hono-api-routes.md | — |
| Drizzle | drizzle-schema.md | — |
| TanStack Query | tanstack-query.md | react-components.md |
| React | react-components.md | shadcn-ui.md |
| Shadcn/UI | shadcn-ui.md | — |
| Tailwind CSS | shadcn-ui.md | — |
| Clerk | authentication.md | hono-api-routes.md |
| Expo / React Native | mobile-desktop.md | — |
| Electron | mobile-desktop.md | — |
| Turborepo | monorepo-packages.md | typescript-stack.md |
| Bun | monorepo-packages.md | typescript-stack.md |
| Flask | python-stack.md | python-patterns.md |
| psycopg2 | python-patterns.md | — |
| SQLAlchemy | python-patterns.md | — |
| xarray / Zarr | data-science-patterns.md | — |
| NumPy | data-science-patterns.md | — |
| joblib | data-science-patterns.md | — |
| uv | python-stack.md | — |
| Zod | hono-api-routes.md | tanstack-query.md |
| React Hook Form | react-components.md | — |
| Recharts | shadcn-ui.md | — |

## Do / Don't

| Do | Don't |
|----|-------|
| Register every new file here | Add content without an index entry |
| Use templates from `_templates/` | Create docs from scratch |
| Keep entries in `[filename](path): description` format | Use verbose prose in the index |
| Use relative paths (repo is portable) | Hardcode machine-specific absolute paths |
